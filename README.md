# docker_learning

## Installation
 - Install [Git Client](https://git-scm.com/downloads)
 - Install [Docker Desktop for Windows which includes Kuberetes](https://www.docker.com/products/docker-desktop) using the [Guide](https://docs.docker.com/docker-for-windows/install)
 - Verify the installation by launching any Terminal (GitBash or CMD) window, run `docker version`
 - Optional: Download and Install lightweight Editor (e.g.: [Visual Studio Code](https://code.visualstudio.com)) of **User Installer** edition rather than **System Installer**
 - Optional: Install [JSON Formatter](https://chrome.google.com/webstore/detail/json-formatter/bcjindcccaagfpapjjmafapmmgkkhgoa), a Chrome browser extension
 
 ## Notes
 
  **WHAT:**
   - Used for stable and consistent delivery of Application(s) as a single distributable unit (image)
   - _Docker_ follows BORA (**B**uild a containerImage **O**nce and **R**un on **A**ny machine) like _Java_ follows WORA (**W**rite code and compile **O**nce and **R**un **A**nywhere that has JVM).
   - Docker allows to manage the _Infrastructure_ separately from the _Application(s)_ that enables developers to Develop, Package/Ship, Test, and Deploy both _Infrastructure_ and _Applications_ as a single distributable unit (**Container**) into a targeted environment.
   - **Docker Container Image** is a portable, independent, and executable software that consists of all (compiled or non-compiled source code, libraries, tools, infrastructure details, settings, properties, certificates, monitoring agents etc.) to run an application independently and consistently anywhere.
   - Docker solves the traditional problem (Machine Parity) that the Developers faced such as 'It worked in my machine but not in others, not sure what went wrong.
   
  **HOW:**
   - **Isolation** and **Security** allows the Docker to install/run multipe Containers on a single host ignoring the underlying details of Host machine.
   - As **Docker CLI** is used for all the interaction with Docker software, practice rigorusly and remember the command and syntax for various operations/functions
   
  **WHERE:**
   - Runs on any popular Operating System

## Additional Materials
- [Docker Get Started](https://docs.docker.com/get-started)
