![image](https://github.com/user-attachments/assets/fe7923da-3f26-4d91-b45c-c4d8834fea8c)



This repo contains the entire project, including resources and pom.xml files etc. 
The client program is in the client repo, and the server program is in the server repo. They are independent of each other.

To compile and run both programs, you can use maven as the pom.xml files are included.
before packging and running the programs, you should set the application.properties file in both according to your setup (located under src/main/resources).
two example files - application.properties.properties are included in each resources folder to help you set those settings up.

In the client the application.properties file only includes the server address and port, so if you run it on your computer it should include the:
address as 127.0.0.1 or localhost,
port as whatever port your server will run on (in the example file it's 44444).
Now your client is all set up.

In the server - you should first download mysql, create a mysql connection and create in it a schema.
If you want it to be in accordance to the example properties file, you should set your mysql credentials to:
username - root
password - abc123
mysql port - 3306
schema name - chessio

keep all of the other settings the same as they are important for running the server correctly.
you may change your server port in this file as said before, in the example file it is set to 44444.

and that's it! Now just make sure that you can connect to the mysql schema and that mysql is running in the background, and the server + client should work.
again maven should be used for the compilation.
