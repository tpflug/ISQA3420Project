##Data Flow Diagram Dictionary

-----------------------

####Processes
1. Label : Get CPE File/Package Info
 * Description : Coporate Developer sends external file or packaged code to process which sorts out the correct CPE information to query the NIST CPE database. It then sends that query off to NIST.
2. Label : Analyze Code Stream CVE Impact
 * Description : Recieves back the CPE information as well as it's related CVEs from the NIST query. Determines the project information for a manifest and its related risks for the manifest and the Risk database.
3. Label : Create Project Manifest
 * Description : Recieves project and risk informaiton from Analyze Code Stream CVE impact and formulates the project manifest for the Corporate Manager and any other downstream users.
4. Label : Manage Project Information
 * Description : Receives queries from both developers and managers, gathers project risk information from the Risk database, creates a project informaiton response to be sent back to the requester.
5. Label : Manage CPE Information (Daily Job)
 * Description : When NIST updates their vulnerability database, this process handles the task by receiving CPE information from NIST and creating a CPE file to be sent to the DB.
6. Label : Check Project Against Policy
 * Description : Recieves project vulnerability information from the Corporate Manager to determine the level of vulnerability accebtability. Queries the Policy database for the policy matching the project information, determines the pass/fail results, and sends it back to the manager.

####Externals
1. Label : Corporate Developer
 * Description : Internal employee of the corporation who owns this system. Manages internal development of corporate systems and integration of external code into the company.
2. Label : Corporate Manager
 * Description : Internal employee of the corporation who owns this system. Manages the overall process of integrating external code into the corporations system by checking vulnerabilities against set policies and passing project information downstream to the correct people.
3. Label : National Vulnerability Database
 * Description : Large external corporation who handles the updating of a national code vulnerability database for general use. 
 
####Data Stores
1. Label : NIST CPE Information
 * Description : Contains known CPE and CVE information from NIST
2. Label : Risk DB
 * Description : Stored project risk information for the corporation which allows for developers and managers to view and assess vulnerability and policy checks.
2. Label : Policy DB
 * Description : Stores the actual policys for the corporation for checking against external code and determining the code's pass/fail status and level of vulnerability.

####Data Flows
1. Label : File
 * Description : 
2. Label : Package
 * Description : 
3. Label : CPE Query
 * Description : 
4. Label : CPE Information
 * Description : 
5. Label : Package CVEs
 * Description : 
6. Label : Project and Risk Information
 * Description : 
7. Label : Code Stream Risk Information
 * Description : 
8. Label : Policy Manifest Information
 * Description : 
9. Label : Project Info Request
 * Description : 
10. Label : Project Info Response
 * Description : Contains information about the project
11. Label : Package Information Request
 * Description : Contains information about the project
12. Label : Package Information Response
 * Description : Contains information about the package
13. Label : CPE Request
 * Description : Contains CPE information
14. Label : CPE Response
 * Description : Contains CPE information
15. Label : CPE File
 * Description : Contains actual CPE file 
16. Label : Project Vulnerability Information
 * Description : Contains vulnerability information about the project
17. Label : Policy Pass/Fail Response
 * Description : A pass or fail based on the response
18. Label : Poicy Info Query
 * Description : Query containing policy information
19. Label: Policy Info Response
 * Description : Query containing policy information
