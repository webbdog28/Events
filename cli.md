# OpenShift CLI
## 1.	Easy Method
There is a jump server that has provisioned that you can SSH into that has all of the tools you’ll need to complete the labs.  Linux/Mac users will be able to use SSH directly in the command line. Windows users can use WSL or can download Putty for ssh.

The information should be contained in the email you received after you registered and should look like this:
ocvm.westus.cloudapp.azure.com

 
## 2.	Involved Method

### Step 1 
For all OSes, navigate to the following URL and download the client tools package: https://goo.gl/kdAaF5

### Step 2 
For Linux and OSX users, decompress the zip file and copy the binary to the /usr/local/bin directory, or one of the paths listed in the PATH environment variable

For Windows users, go to http://git-scm.com/download/win to download git bash for Windows (during installation you need to specify in the selection to integrate with the command prompt). Then, unzip the OpenShift client tools compressed file and add the file path into the PATH environment variable. 

Homebrew Install for Mac (Alternative)
•	brew install openshift-cli
 
## CLI basic configuration
The easiest way to initially setup the OpenShift CLI is to use the oc login command. It’ll interactively ask you a server URL, username and password. The information is automatically saved in a CLI configuration file that is then used for subsequent commands.

To login to the server use:

$ oc login https://master.ocp.cloudvillage.in:8443/
