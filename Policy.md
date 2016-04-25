##Sample Policy Document

Some possible resources  on this doc:

https://nvd.nist.gov/cvss.cfm , https://www.first.org/cvss/cvss-based-patch-policy.pdf , https://www.first.org/cvss/specification-document , https://www.first.org/cvss/cvss-v30-examples_v1.1.pdf

In short, the policy is what we would apply to the results
	This can be ‘made up’ by you but know where it is going to apply
	This will include context, thresholds, and response

###Context

Our company plans to utilize files and/or packages of source code written outside of the organzation. As such, established policies are in place which dictate the allowable level of vulnerabilities in external code. For any source brought into the organization, the company follows set procedures for researching any existing known vulnerabilities related to the source, scoring the impact of those vulnerabilities, and determining whether or not the code is appropriate for use in our organization. The Common Vulnerability Scoring System (CVSS) is the tool in place to determine the numerical score of CVE risks. The CVSS is defined by the National Institute of Standards and Technology (NIST). More specific details regarding the scoring standards used by CVSS can be found at https://www.first.org/cvss/specification-document.

###Threshold
What are the minimum values (CVE) that need to be passed? 
The following table details the scoring standards for assessing vulnerability severity and acceptability of external code.

| CVEE Score    | Risk Severity | Response  |
| ------------- |:-------------:| ---------:|
| col 3 is      | right-aligned |           |
| col 2 is      | centered      |           |
| zebra stripes | are neat      |           |

###Response
If this doesn’t pass, what do you do? 
