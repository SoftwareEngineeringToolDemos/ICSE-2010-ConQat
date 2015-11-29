<h1>Instructions to install Conqat using scripts in this build-vm folder</h1>

#### Contents:
1. **Vagrantfile** - This is the file which is used to provision the VM and it also has commands which are run in the shell in order to install the required dependencies for the tool. This is done automatically via the Vagrantfile.
2. **README.txt** - A readme file which has instructions on how to run the tool in the VM. This file needs to be downloaded since it will be copied into the VM.
3. **Installation.txt** - This file has instructions on installing the tool from scratch if required. 
4. **eclipse.desktop** - Desktop file to start eclipse upon reload.
5. **youtube.desktop** - A direct link to the demo video on youtube.
6. **License.txt** - License file containing terms for the use of the tool.

###Prerequisites to be installed before the running the script:
1. In order to install required softwares, vagrant needs to be reloaded during provisioning. This can be done by using the following plug-in for vagrant - [Vagrant Plugin](https://github.com/aidanns/vagrant-reload).
2. Install this plug-in and then follow the beloew steps to start the VM. Note: This plugin is a prerequisite to ensure the proper installation of the tool. Else manual vagrant reload will be required.

###Steps in order to start the VM:
1. Copy the build-vm folder to the host on which the VM needs to be installed by cloning the repository or forking it.

2. Go to [this](https://drive.google.com/a/ncsu.edu/file/d/0B4wr6DTFw-HOcVBwQU5mTUkzZHM/view?usp=sharing) google drive link and download the tar file into the build-vm folder.

3. In the folder with the Vagrantfile, execute the following command:
``` vagrant up ```. Note: Virtual box must be installed on the VM.

4. Wait for the VM to be started. Now the script automatically executes the commands required to install JDK 1.8 onto the VM. This happens in the shell.
Note: SSH Authentication must be enabled and functioning. 

5. Once the execution in the shell is completed, open the README.txt file in the VM for further instructions.

#### Requirements:
1. [Vagrant](https://www.vagrantup.com/downloads.html).

2. [VirtualBox](https://www.virtualbox.org/wiki/Downloads).

3. [Vagrant Plugin](https://github.com/aidanns/vagrant-reload).

4. [Conqat tar file](https://drive.google.com/a/ncsu.edu/file/d/0B4wr6DTFw-HOcVBwQU5mTUkzZHM/view?usp=sharing)

#### Username and Password
* username: *vagrant*
* password: *vagrant*

### Acknowledgments
* https://docs.vagrantup.com/v2/provisioning/shell.html

