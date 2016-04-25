#Sample Policy Documents
---
###Policy 1

####Context

Our company plans to utilize files and/or packages of source code written outside of the organzation. As such, established policies are in place which dictate the allowable level of vulnerabilities in external code. Depending on the context within our organization that the external code stands to affect, these policies apply differently and require varying responses. The following policy will be applied when examining the risks attached to code involved in backend tasks for projects. That is, this policy applies to packages of code which have lower levels of exposure and criticality within our system. 

This policy utilitizes the Common Vulnerability Scoring System (CVSS), a standard tool for determining a numerical score of CVE risks. The CVSS is defined by NIST. More specific details regarding the scoring standards used by CVSS can be found at https://www.first.org/cvss/specification-document and https://nvd.nist.gov/cvss.cfm.

####Threshold

The following table details the scoring standards for assessing vulnerability severity and acceptability of external code related to performing backend funcitons within our organization.

| CVEE Rating   | Score Threshold | Pass/Fail  |
| ------------- |:-------------:|:---------:|
| None      | 0.0      | Pass |
| Low       | 0.1-3.9  | Pass |
| Medium    | 4.0-6.9  | Pass |
| High      | 7.0-8.9  | Fail |
| Critical  | 9.0-10.0 | Fail |

####Response
If this doesn’t pass, what do you do? 

---

###Policy 2

####Context 

This policy applies to external source which is being imported to help handle client sales, and therefore has a higher exposure level. As such, the tolerable level of vulnerabilities is more strict in this policy, so it is more likely that the organization will reject the use of code than in the previous context. 

####Threshold

| CVEE Rating   | Score Threshold | Pass/Fail  |
| ------------- |:-------------:|:---------:|
| None      | 0.0      | Pass |
| Low       | 0.1-2.9  | Pass |
| Medium    | 3.0-5.9  | Pass |
| High      | 6.0-7.9  | Fail |
| Critical  | 8.0-10.0 | Fail |

####Response

.

