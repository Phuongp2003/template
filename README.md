# HOW TO USE

1. Download Extension Pack for Java, Community Server Connectors in vscode market place.
2. Download maven.
3. In Explorer (Ctrl+Shift+E), look at tag "Server", add your tomcat server (use server on disk) or download a new server.
4. launch task "maven: clean install" by ctrl + shift p and choosing "Task: run task" to build a classes path.
5. Right click on the project (src/main/webapp) and choose "Run on server" to deploy the project on the server.

- Choose server -> your server
- Add params -> no
- Project name -> your project name (it will be your slug to view the project on the browser)

5. Open your browser and go to http://localhost:8080/(<your-project-name>)

# NOTE

## 1. Change output port

- On tag Server, right click on your server and choose "Server Actions..."
- Choose "Edit Configuration File"
- Choose conf/server.xml
- Find "Connector port=" and change the port to your desired port.
- Restart/start your server.

## 2. Simple way to deploy with your project name

- When adding a project to the server, you keep project name empty, your slug will be http://localhost:8080/webapp
- If you want to change the slug, you can change the webapp folder name to your desired name.

## 3. Builded folder of maven (target)

- You can run the project by right click on the .war and choose "Run on server" without building the project by yourself, but it's doesn't have hot reload.

- You can delete this folder, it will not affect your project.
