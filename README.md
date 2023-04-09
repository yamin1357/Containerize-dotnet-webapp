# Containerize-dotnet-webapp
Containerize a .NET webapp


After Clone This Project From Git

CD to Containerize-dotnet6-webapp And Build Docker Image by Bellow Command

>> docker build -t mywebapp-image -f Dockerfile .

Then Run Bellow Command for Run Conyainer from mywebapp-image

>> docker run -d --name mywebapp-container -p 5000:5000 mywebapp-image

By executing the above commands, the program is ready to serve on port 5000
Now you can enter the address http://localhost:5000 in the browser and view the site.

For Delete Running Container Execute Bellow Command

>> docker stop //\$(docker ps -q -a --filter "name=webapp-container") && docker rm //\$(docker ps -q -a --filter "name=webapp-container")
 
