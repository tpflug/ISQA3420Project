#Sample Policy Documents

###Policy 1

####Context

The following policy will be applied when examining the risks attached to code involved in the backend processes for projects in the organization. That is, this policy applies to packages of code which have lower levels of exposure and criticality within our system, or are otherwise less often utilized by the system. 

####Threshold

| CVEE Rating   | Score Threshold | Pass/Fail  |
| ------------- |:-------------:|:---------:|
| None      | 0.0      | Pass |
| Low       | 0.1-3.9  | Pass |
| Medium    | 4.0-6.9  | Pass |
| High      | 7.0-8.9  | Fail |
| Critical  | 9.0-10.0 | Fail |

####Response

For source which meets the passing criteria in this test (CVEE Score of 0.0-6.9), the code is approved to move to the next step of implemention, and its usage will be monitored and recorded for any unforseen issues resulting from vulnerabilities.

For code that is rejected by this policy (CVEE Score of 7.0 and above), the Corporate Manager checking the policy will inform the developer and the organziation that the code is unacceptable for use within the organization. The manager will detail which specific vulnerabilities led to the high overall risk, and give any recommendations on potential alternative external source, or whether an in house coding of the process can be considered to avoid these vulnerabilities. 

---

###Policy 2

####Context 

This policy applies to external source which may be implemented in order to handle client sales, customer data, and transaction based processes within our system. This category of information has a higher exposure level, as well as more sensitive informaiton. As such, the tolerable level of vulnerabilities is more strict in this policy, so it is more likely that the organization will reject the use of code in this context if it is deemed to be too much of a risk to implement. 

####Threshold

| CVEE Rating   | Score Threshold | Pass/Fail  |
| ------------- |:-------------:|:---------:|
| None      | 0.0      | Pass |
| Low       | 0.1-2.9  | Pass |
| Medium    | 3.0-5.9  | Pass |
| High      | 6.0-7.9  | Fail |
| Critical  | 8.0-10.0 | Fail |

####Response

For source which meets the passing criteria in this test (CVEE Score of 0.0-5.9), the code is approved to move to the next step of implemention, and its usage will be monitored and recorded for any unforseen issues resulting from vulnerabilities.

For code that is rejected by this policy (CVEE Score of 6.0 and above), the Corporate Manager checking the policy will inform the developer and the organziation that the code is unacceptable for use within the organization. The manager will detail which specific vulnerabilities led to the high overall risk, and give any recommendations on potential alternative external source, or whether an in house coding of the process can be considered to avoid these vulnerabilities. 

