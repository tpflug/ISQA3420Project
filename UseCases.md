#Use Cases

##This project will have 3 Use cases

### Use Case #1

* Title: Developer commits code to be examined for vulnerabilities 
* Primary Actor: Developer
* Goal in Context: Gather vulnerability information for all external source code that is used by developers
* Stakeholders: Developer / Manager
* Preconditions: Developer is able to check in external source code to vulnerability system. NIST vulnerability database is up to date. 
* Main Success Scenario: Developer checks in code and vulnerability information is recorded to the Risk DB. 
* Failed End Conditions: Developer is unable to check in code. Checked in code is not checked for vulnerabilities, failing to update Risk DB. 
* Trigger: Code check in 

### Use Case #2

* Title: Apply policy against the vulnerability of the package 
* Primary Actor: Manager
* Goal in Context: To determine whether the external source code's risks exceeds the allowed level of vulnerability set by the policys governing this.
* Stakeholders: Developer / Manager
* Preconditions: Vulerability information has been appropirately gathered and stored. Policy database is up to date.
* Main Success Scenario: Manager sends project vulnerability information to be checked against policy and recieves a valid response detailing whether or not the project passes policy.
* Failed End Conditions:  Manager is unable to pull valid project and vulnerability information. Manager cannot access policy database. Policy check returns false positive result.
* Trigger: Project information recieved by Manager.

### Use Case #3

* Title: Store package and CPE information into the Risk database 
* Primary Actor: Developer
* Goal in Context: Store this information so that the manager can make an informed decision based on the risk of the package. 
* Stakeholders: Developer / Manager
* Preconditions: The developer submits a valid file and or package. NIST CPE Information returns valid CPE and Package CVE's. The Analyze Code Stream CVE Impact process does not impact the data in a harmful manner. 
* Main Success Scenario: The Analyze Code Stream CVE Impact process does not impact the data in a harmful manner. 
* Failed End Conditions: The developer does not submit a proper file and or package. The NIST CPE Information does not return proper data. The Analyze Code Stream CVE Impact process impacts the data in a harmful way. 
* Trigger: Corporate developer submits a package and or file.

