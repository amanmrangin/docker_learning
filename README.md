# docker_learning

## Installation
 - Install [Git Client](https://git-scm.com/downloads)
 - Install [Docker Desktop for Windows which includes Kuberetes](https://www.docker.com/products/docker-desktop) using the [Guide](https://docs.docker.com/docker-for-windows/install)
 - Verify the installation by launching any Terminal (GitBash or CMD) window, run `docker version`
 - Optional: Download and Install lightweight Editor (e.g.: [Visual Studio Code](https://code.visualstudio.com)) of **User Installer** edition rather than **System Installer**
 - Optional: Install [JSON Formatter](https://chrome.google.com/webstore/detail/json-formatter/bcjindcccaagfpapjjmafapmmgkkhgoa), a Chrome browser extension
 
 ## Notes
 
  **WHAT:**
   - Used for stable and consistent delivery of Application(s) as a single distributable unit (Container Image)
   - _Docker_ follows BORA (**B**uild a containerImage **O**nce and **R**un on **A**ny machine that has Docker software installed) like _Java_ follows WORA (**W**rite code and compile **O**nce and **R**un **A**nywhere that has JVM).
   - Docker allows to manage the _Infrastructure_ separately from the _Application(s)_ that enables developers to Develop, Package/Ship, Test, and Deploy both _Infrastructure_ and _Applications_ as a single distributable unit (**Container**) into a targeted environment.
   - **Docker Container Image** is a portable, independent, and executable software that consists of all (compiled or non-compiled source code, libraries, tools, infrastructure details, settings, properties, certificates, monitoring agents etc.) to run an application independently and consistently anywhere.
   - Docker solves the traditional problem (Machine Parity) that the Developers faced such as 'It worked in my machine but not in others, not sure what went wrong.
   
  **HOW:**
   - **Isolation** and **Security** allows the Docker to install/run multipe Containers on a single host ignoring the underlying details of Host machine.
   - As **Docker CLI**, AKA _Docker Client_, is used for all the interaction with Docker software, practice rigorusly and remember the command and syntax for various operations/functions
   
  **WHERE:**
   - Runs on any popular Operating System

  **Pouplar Terms:**
   - **Docker Desktop**: Easy-to-install software consists of all the following components of Docker.
   - **Docker Client**: A command based tool, CLI, to interact with **Docker Host**
   - **Docker Host**: A software, acts as a server, listens to Docker Client requests.  It consists of many components such as _Docker Daemon_, _Images_, _Containers_
     - **Docker Daemon**: A service/listener for all the requests and manages the _Containers_, _Images_, _attached Stoage Volumes_, _Networks_
     - **Docker Objects - Images**: A file with set of instructions version of any software (E.g. Ubuntu, RedHad Linux, Apache Webserver, JDK, Tomcat, NodeJS etc..y) that can be collected and concustomized to build another Docker Image. Example: A Image can be a software built using collection many software products such as of 'Ubuntu OS', 'Apache WebServer', 'JDK11', 'Tomcat', 
         

## Additional Materials
- [Docker Get Started](https://docs.docker.com/get-started)
