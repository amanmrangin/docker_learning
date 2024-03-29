# docker_learning

## Installation
 - In Windows machine, Downlaod and install [WSL](https://learn.microsoft.com/en-us/windows/wsl/install). Requires restarting of machine to continue setting up a new user account/password to access the install Linux Distro.  
   ![image](https://user-images.githubusercontent.com/129334520/231916581-2c8c40c5-6a78-42f1-b93d-42e1bcc0aa60.png)
 - Install [Git Client](https://git-scm.com/downloads). 
 
    ![image](https://user-images.githubusercontent.com/129334520/231916957-d1eeec87-9426-4574-a87a-1fa889de0a75.png)
    
 - Install [Docker Desktop for Windows which includes Kuberetes](https://www.docker.com/products/docker-desktop) using the [Guide](https://docs.docker.com/docker-for-windows/install).
   - Create an account at Docker.com and _Sign In_ from installed 'Docker Desktop' application.
   - After login, navigate to _Settings_-> _Kubernetes_ -> select _Enable Kubernetes_ and clikc on 'Apply & Restart' button.
   ![image](https://user-images.githubusercontent.com/129334520/231917516-8647ab4f-eff6-4046-87aa-24399da7f122.png)

 - Verify the installation by launching any Terminal (GitBash or CMD) window, run `docker version`
 - Optional: Download and Install lightweight Editor (e.g.: [Visual Studio Code](https://code.visualstudio.com)) of **User Installer** edition rather than **System Installer**
 - Optional: Install [JSON Formatter](https://chrome.google.com/webstore/detail/json-formatter/bcjindcccaagfpapjjmafapmmgkkhgoa), a Chrome browser extension
 
 ## Notes
 
  **WHAT:**
   - A platform Written in **GO** language, Used for stable and consistent delivery of Application(s) as a single distributable unit (Container Image) that can run on any machine with the support of Docker software.
   - _Docker_ follows BORA (**B**uild a containerImage **O**nce and **R**un on **A**ny machine that has Docker software installed) like _Java_ follows WORA (**W**rite code and compile **O**nce and **R**un **A**nywhere that has JVM).
   - Docker allows to manage the _Infrastructure_ separately from the _Application(s)_ that enables developers to Develop, Package/Ship, Test, and Deploy both _Infrastructure_ and _Applications_ as a single distributable unit (**Container**) into a targeted environment.
   - **Docker Container Image** is a portable, independent, and executable software that consists of all (compiled or non-compiled source code, scripts, libraries, binaries, tools, infrastructure details, Environment Variables, settings, properties, certificates, monitoring agents etc.) to run an application independently and consistently anywhere.
   - Docker solves the traditional problem (Machine Parity) that the Developers faced such as 'It worked in my machine but not in others, not sure what went wrong.
   
  **HOW:**
   - **Isolation** and **Security** allows the Docker to install/run multipe Containers on a single host ignoring the underlying details of Host machine. The **Isolation** is acheived through **namespace**.
   - As **Docker CLI**, AKA _Docker Client_, is used for all the interaction with Docker software, practice rigorusly and remember the command and syntax for various operations/functions
   
  **WHERE:**
   - Runs on any popular Operating System, installed in **/var/lib/docker**

  **Terminology:**
   - **Docker Desktop**: Easy-to-install software consists of many of the following components of Docker.
   - **Docker Client**: A command based tool, CLI, to interact with **Docker Host**
   - **Docker Host**: A software, acts as a server, listens to Docker Client requests.  It consists of many components such as _Docker Daemon_, _Images_, _Containers_

     - **Docker Daemon**: A service/listener for all the requests and manages the _Containers_, _Images_, _attached Stoage Volumes_, _Networks_.
     - **Docker Object - Image(s)**: A text file (Dockerfile) with set of instructions/commands to build an **Image** consising of different layers software (E.g. its own File System, Operating System, Environment variables, Webservers, JDK, Tomcat, SpringBoot, Database libraries etc..) that require to run a custom software (e.g. Web Application).
     
      - **Docker Build** process reads the instructions of **Dockerfile** in a sequence and produces an output, **Image**.
     - **Docker Object - Container**: A runnable instance of **Image** that can be started, stopped, and deleted using CLI and API. Each **Container** is _isolated_ from other Containers and from the Host machine. Uses _kernal namespaces and cgroup_ of OS to get the Isolation. 
   - **Docker Registry**: A storage place of Docker Images. A corporation can have it's own custom/dedicated/internal registry to prevent from using unlicensed, vulnerable software images.
   - **Docker Hub**: A public registry for public images that anyone can use, Docker is configured by default to search and pull the public images from here. 

## Practice Commands
- To **Download/pull the pre-defined Docker Image and Run in local machine as a Container**: `docker run <IMAGE_NAME_ID>` OR `docker run [OPTIONS] IMAGE [COMMAND] [ARG....]`
  - Example: `docker run getting-started`
- To **see all the existing Docker Images of local machine**: `docker images`t
- To **Run NGINX container in a default internal port (80) and expose/accessible through local machine port 8080 in a Detached (d) mode**: `docker run -p 8080:80 -d nginx`, access http://localhost:8080 to see Nginx Welcome screen in your local machine browser, not in nginx server
- To **see the existing running docker containers**: `docker ps`
- To **see the Logs of a container**: `docker logs <container id>`
- To **Stop the running docker container**: `docker stop <container id>`
- To **run a command in a running container**: Use `docker exec`
    -   To List the files of a directory from running container, and pipes the output back to terminal console: `docker exec -it <container id> ls /usr/share/nginx/html`
    -   To see the bash prompt of container on console: `docker exec -it <container id> bash`

## 


## Additional Materials
- [Docker Get Started](https://docs.docker.com/get-started)
- [Docker commands](https://docs.docker.com/engine/reference/commandline/docker/)
