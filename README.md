# Java-Servlet
This repository demonstrate how to run Apache Tomcat Server on linux:

Steps are:

    Download Apache Tomcat from https://tomcat.apache.org/download-80.cgi
    Make xyz folder in apache-tomcat/webapps
    Change permission on bin of sh files to allow execting program.
    Open terminal and start server by running sh startup.sh in terminal. Check in web-browser by visiting localhost:8080, which starts the Apache-TomCat Server.
    From bin extract servlet.tar file to location where you put your java file (in xyz folder).
    Compile java file and paste it's class file in webapps/examples/web-inf/classes.
    Update xml file(/webapps/examples/web-inf) by adding:

     <servlet-name>balia</servlet-name>
     <servlet-class>myClass</servlet-class> 
     
    </servlet>
    <servlet-mapping>
     <servlet-name>balia</servlet-name>
     <url-pattern>/bc</url-pattern> <!-- add the url pattern to form action--->
    </servlet-mapping> ``` 

    Restart the server if reqired.
    Enter http://localhost:8080/xyz/add.html to run the servlet.
