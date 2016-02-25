##Data Flow Diagram Dictionary

###Tim and Al's Data Dictionary - ISQA 3420 Group Project
Note: We may need to split this up by first naming one process, then naming the data flows, externals, and data stores associated with in before moving to another process. If we do this, we might want to have some way to note when we are referring to the same instance of something that gets hit in multiple processes. For example, if Process A and B both query the same Data Store, we would either want to note that we are using something like "Data Store 2 - Risk DB" for both, so that there is no thinking the two instances of the Risk DB are different ones. An alternative would be to just note it the first time we hit it, and not do that again for other processes that hit it. Just depends on how Germonprez would like it

####Processes
1. Label : Manage Code Streams
 * Description : Placeholder Process - will be split up into two processes later on
2. Label : Manage CPE Information (Daily Job)
 * Description :
3. Label : Manage Project Information
 * Description :

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

####Data Flows
1. Label : File
 * Description : 
2. Label : Package
 * Description : 
3. Label : Package Query
 * Description : 
4. Label : CPE Information
 * Description : 
5. Label : Package and CPE Information
 * Description : 
6. Label : CPE Request
 * Description : 
7. Label : CPE Response
 * Description : 
8. Label : CPE File 
 * Description : 
9. Label : Project Info Request
 * Description : 
10. Label : Project Info Response
 * Description : 
11. Label : Package Information Request
 * Description : 
12. Label : Package Information Response
 * Description : 
