CONTENTS OF THIS FILE
---------------------

1.INTRODUCTION
2.REQUIREMENTS
3.INSTALLATION
4.RUNNING AN EXAMPLE
5.UNDERSTANDING THE OUTPUT
6.LICENSE

1. INTRODUCTION
------------
1.ConQat is a tool used mainly for Software Quality Analysis. Its capabilities vary from different aspects of quality analysis such as Architecture conformance to Clone Detection in the code. The main functionality which we demonstrate in this VM is the Architecture Conformance. System architecture is a method to divide the different aspects of the system into smaller independent components which interact with each other. This division of the code helps in understanding each small component individually and design better and efficient systems. 

2.Using ConQat we can provide our architecure to the tool along with the implementation and ConQat maps the different components and generates a model based on the dependencies. Then it compares this model against the implmentations and identifies the violations and the percentage of conformance. In this README, we provide instructions on how to generate a conformance report for the example architecture given with the ConQat tool. 

2. REQUIREMENTS	
------------
In order to run ConQat, JDK 1.8 or higher is required. On this VM Oracle JDK 1.8 has been installed. 

3. INSTALLATION
------------
1.The tool has already been installed on this VM. But for interested people, the tool can be downloaded from this link. (https://www.cqse.eu/download/conqat/conqat-2015.2-linux-gtk-x86_64.tar.gz)
2.Once the tar.gz id downloaded, untar it to any location on disk and open the folder.
3.Run the eclipse binary inside the folder. This setsup the tool on the system. 

4. RUNNING AN EXAMPLE
------------------
Once this VM is switched on, the tool is opened for the user automatically. In order to see an example of the architecture conformance feature, the user simple needs to perform the following actions in eclipse:

1.Importing Examples - The project has already been imported in this VM. But in order to do it manually if required, go to File->New->Example. Select ConQat Examples->ConQat Example Project. Press Next and Finish. This imports the existing examples into the workspace. 

2.Running a configuration - In order to test the given Junit architecure, in the conQat-examples project, open the architecture-example-junit.cqr configuration file, then click on "Launch ConQat Analysis"
option in the run block. 

3.Checking the architecture output - Once this configuration has been run, it generates the output in two different locations, one as an assessment file which we can view in the architecure editor of ConQat and the other as a static HTML file in the output folder which we can open in the browser. Note that this output folder was not present previously. To open the architecure-assessment.xml file in the editor, open the file and click on mode to switch the editor mode. You might have to click once or twice for this to open. Now once the file explorer is opened, navigate to ~/Desktop/Conqat/Conqatworkspace/conqat-examples/output/architectureanalysis/junit/ folder and select the dependencies.xml file.
4.In order to view the output in the HTML file, open the workspace directory in your terminal and navigate to "conQat-Examples->output->architectureanalysis->junit". Here open the index.html file using the following command in the terminal - "sudo firefox index.html". Since we removed unnecessary softwares, default firefox profile is not present for the vagrant user. 

UNDERSTANDING THE OUTPUT
------------------------
In the figure given in the ouput, red lines indicate that the dependency is present between the wrong components and the a green line indicates that the architecure is correct for those components.

REFERENCES
----------
All the credit for the code, the content and the installation instructions goes solely to the authors - Florian Deissenboeck, Lars Heinemann, Benjamin Hummel, Elmar Juergens. All the installation instructions have been followed from the website - https://www.cqse.eu/en/products/conqat/install/
























