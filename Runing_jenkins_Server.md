# Jenkins: 
- open source Continuous Integration server
- tool for DevOps practitioner
- can be used to automate all sorts of tasks related to building, testing, and delivering or deploying software

# Setting Up Jenkins 
  1. **Pull the jenkins image to the local registry:** ``docker pull jenkins``
  2. **Verify that the jenkins image is downloaded:** ``docker images``
  3. **Create a container:** ``docker run --name jencon -p 8080:8080 -p 50000:50000 -v /Desktop/jenkins:/var/jenkins_home jenkins``
        - ``--name jencon``: names the container thus created as **jencon**
        - ``-p 8080:8080`` : **maps the container port 8080 to host's machine 8080**
        - ``-v /Desktop/jenkins:/var/jenkins_home``: **Mounts the folder located at *Desktop/jenkins* of host's machine** to **/var/jenkins_home** inside the container.
 4. Open the broswer and open the url ``http://localhost:8080/``
 
 **Note:** It is good practice to mount the folders from the host's machine to container rather than creating a folder inside the container.
        
