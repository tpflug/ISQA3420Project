##Data Flow Diagram Dictionary

###Tim and Al's Data Dictionary - ISQA 3420 Group Project
Note: We may need to split this up by first naming one process, then naming the data flows, externals, and data stores associated with in before moving to another process. If we do this, we might want to have some way to note when we are referring to the same instance of something that gets hit in multiple processes. For example, if Process A and B both query the same Data Store, we would either want to note that we are using something like "Data Store 2 - Risk DB" for both, so that there is no thinking the two instances of the Risk DB are different ones. An alternative would be to just note it the first time we hit it, and not do that again for other processes that hit it. Just depends on how Germonprez would like it

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
 * Description : Internal employee of the corporation who owns this system. 
2. Label : Corporate Manager
 * Description :  
3. Label : National Vulnerability Database
 * Description : 
 
####Data Stores
1. Label : NIST CPE Information
 * Description :
2. Label : Risk DB
 * Description :
2. Label : Policy DB
 * Description :

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
 * Description : 
11. Label : Package Information Request
 * Description : 
12. Label : Package Information Response
 * Description : 
13. Label : CPE Request
 * Description : 
14. Label : CPE Response
 * Description : 
15. Label : CPE File
 * Description : 
16. Label : Project Vulnerability Information
 * Description : 
17. Label : Policy Pass/Fail Response
 * Description : 
18. Label : Poicy Info Query
 * Description : 
19. Label: Policy Info Response
 * Description :
