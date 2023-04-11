# docker_learning

## Installation
 - Install [Git Client](https://git-scm.com/downloads)
 - Install [Docker Desktop for Windows which includes Kuberetes](https://www.docker.com/products/docker-desktop) using the [Guide](https://docs.docker.com/docker-for-windows/install)
 - Verify the installation by launching any Terminal (GitBash or CMD) window, run `docker version`
 - Optional: Download and Install lightweight Editor (e.g.: [Visual Studio Code](https://code.visualstudio.com)) of **User Installer** edition rather than **System Installer**
 - Optional: Install [JSON Formatter](https://chrome.google.com/webstore/detail/json-formatter/bcjindcccaagfpapjjmafapmmgkkhgoa), a Chrome browser extension
 
 ## Notes
 
  **WHAT:**
   - Written in **GO** language, Used for stable and consistent delivery of Application(s) as a single distributable unit (Container Image).
   - _Docker_ follows BORA (**B**uild a containerImage **O**nce and **R**un on **A**ny machine that has Docker software installed) like _Java_ follows WORA (**W**rite code and compile **O**nce and **R**un **A**nywhere that has JVM).
   - Docker allows to manage the _Infrastructure_ separately from the _Application(s)_ that enables developers to Develop, Package/Ship, Test, and Deploy both _Infrastructure_ and _Applications_ as a single distributable unit (**Container**) into a targeted environment.
   - **Docker Container Image** is a portable, independent, and executable software that consists of all (compiled or non-compiled source code, scripts, libraries, binaries, tools, infrastructure details, settings, properties, certificates, monitoring agents etc.) to run an application independently and consistently anywhere.
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
     - **Docker Object - Image(s)**: A text file (Dockerfile) with set of instructions/commands to build an **Image** consising of different layers software (E.g. Ubuntu, RedHad Linux, Apache Webserver, JDK, Tomcat, SpringBoot, Database libraries etc..) that require run a custom software (e.g. Application).
     
      - **Docker Build** process reads the instructions of **Dockerfile** in a sequence and produces an output, **Image**.
     - **Docker Object - Container**: A runnable of instance of **Image** that can be started, stopped, and deleted using CLI and API. Each **Container** is _isolated_ from other Containers and from the Host machine. uses _kernal namespaces and cgroup_ of OS to get Isolation. 
   - **Docker Registry**: A storage place of Docker Images. 
   - **Docker Hub**: A public registry for public images that anyone can use, Docker is configured by default to search and pull the public images from here. 
   -    

## Additional Materials
- [Docker Get Started](https://docs.docker.com/get-started)
