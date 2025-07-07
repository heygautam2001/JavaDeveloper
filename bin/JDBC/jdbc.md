
# JAVA DATABASE CONNECTIVITY (JDBC)

   - JDBC --> JAVA DATABASE CONNECTIVITY ---> IT REFERS TO THE CONNECTION BETWEEN JAVA WITH THE DATABASE EITHER WITH SQL , MONGODB ETC..
   - IT IS USED TO ESTABLISH THE CONNECTION BETWEEN JAVA AND DATABASE THROUGH A DATABASEE QUERY LANGUAGE..
   - HERE WE USE JDBC API 
   - STEPS FOR DATABASE CONNECTION
   
     1. LOAD AND REGISTER DRIVER. --> Class.forName("com.mysql.cj.jdbc.Driver"); sql8 , download & add mysql.connector.jar(mandatory)
     2. CREATE / ESTABLISH THE CONNECTION.---> DriverManager.getConnection("url","username" , "password");
         url : jdbc:mysql://localhost:3306/db.name
         un : root
         pass : root
         Connection con 
     3. CREATE STATEMENT. ---> PreparedStatement ps = con.prepareStatement("sqlquery");
     
     4. EXECUTE SQL STATEMENT ---> ps.executeQuery(); // select query // returns value is Result set
                              ---> ps.executeUpdate(); // insert , update , delete query // returns value in integer
                              ---> ps.close();
                              
     5. PROCESS THE RESULT    ---> 
     
     6. CLOSE THE CONNECTION  ---> con.close();

