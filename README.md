# BrowserStackAssignment1


### Key features- 
1. Live streaming of logs
2. The feeds will refresh in every 1 sec.
3. Multiple users can access the logs at the same time. (synchronization)
4. The previous logs will not be lost ,if new logs are added

### Instructions for deployment-
1. Extract the folder LogReader.rar
2. Open the LogReader->target, Copy the LogReader.war file.
3. Open Tomcat->webapps, paste the war file here.
4. Open conf folder in tomcat.
5. Paste the sysLogs.log and temp.txt files here.
6. Open catalina.properties, paste these 2 lines there,
    - spring.config.location=C:/Tomcat 8.0 - COGS/conf/sysLogs.log
    - tempFile.location=C:/Tomcat 8.0 - COGS/conf/temp.txt
      Here change the path to that of your tomcat.
7. Open bin folder in tomcat. Run startup.bat to run the server.
8. On the browser hit the url
    - http://{server}:{port}/LogReader/rest/service/landing

You can see the streaming of logs here.
Change the sysLogs.log file and save to see the changes on browser.

Note: Refresh time is set as 1 sec.
