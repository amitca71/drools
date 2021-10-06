drools dmn sample
=======================
1) boot drools and kie
docker run -p 8080:8080 -p 8001:8001 -d --name drools-workbench jboss/drools-workbench-showcase:latest 
docker run -p 8180:8080 -d --name kie-server --link drools-workbench:kie-wb jboss/kie-server-showcase:latest

2) login http://localhost:8080/business-central (admin/admin)
3) design -> import project -> https://github.com/amitca71/drools
![image](https://user-images.githubusercontent.com/5821916/136241458-9e0756f5-e597-4c58-b585-c53fe30e2247.png)
