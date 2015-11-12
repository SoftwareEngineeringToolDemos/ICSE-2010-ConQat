#### Contents:

1. **Vagrantfile** - This is the file which is used to provision the VM and it also has commands which are run in the shell in order to install the required dependencies for the tool. This is done automatically via the Vagrantfile.

###Steps in order to start the VM:
1. Copy the Vagrantfile to the host on which the VM needs to be installed. 

2. In the folder with the Vagrantfile, execute the following command:
``` vagrant up ```.Note: Virtual box must be installed on the VM.

3. Wait for the VM to be started. Now the script automatically executes the commands required to install JDK 1.8 onto the VM. This happens in the shell.
Note: SSH Authentication must be enabled and functioning. 

4. Once the execution in the shell is completed, use the following command in the shell to verify the installation of java:
``` java -version ```

#### Requirements:
1. [Vagrant](https://www.vagrantup.com/downloads.html).

2. [VirtualBox](https://www.virtualbox.org/wiki/Downloads).

#### Username and Password

* username: *vagrant*
* password: *vagrant*

### Acknowledgments
* https://docs.vagrantup.com/v2/provisioning/shell.html

