#Use Cases

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

* Title: Manager updates/creates risk policy information 
* Primary Actor: Manager
* Goal in Context: The manager provides evaulation on risk policy information and establishes the appropriate policy by updating an existing policy or creating a new policy.  
* Stakeholders: Developer / Manager
* Preconditions: Risk and policy database is up to date. 
* Main Success Scenario: Manager receives risk policy information and either updates an existing policy or creates a new policy based on the information received. 
* Failed End Conditions: Manager is unable to receive risk policy information and is unable to make a change or create a new policy. 
* Trigger: Risk policy information received by the developer. 

