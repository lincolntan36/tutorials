How to install RStudio in an apt (Ubuntu) container on Vanilla OS 22.10 Kinetic

#Initializing an apt container:
`apx enter apt`
This command will enter the apt (Ubuntu) container on Vanilla OS. Next paste the following command.

#Installing common software properties:
`sudo apt install --no-install-recommends software-properties-common dirmngr`
This command will install common software properties needed. If this is your first time initializing an apt container, these will need to be installed. Next paste the following command. When prompted type y then enter or type yes then enter.

Installing libasound2:
`sudo apt install libasound2`
This command will install libasound2. Next paste the following command. When prompted type y then enter or type yes then enter.

Installing libnss3:
`sudo apt install libnss3`
This command will install libnss3. Next paste the following command.

Updating & Upgrading:
`sudo apt update && sudo apt upgrade -y`
This command will update and upgrade.

Downloading RStudio Desktop .DEB:
Before we install R, we want to download the RStudio Desktop. This download file can be downloaded at this link here:

https://posit.co/download/rstudio-desktop/

Installing RStudio Desktop .DEB:
Once you have downloaded the required .DEB file for RStudio Desktop, we will need to install this into our apt (Ubuntu) container. This can be done very easily be simply, pasting the following command in your previously opened Console/Terminal window.

`cd Downloads`
This command will make the Console/Terminal window be navigated into your Downloads folder. Next paste the following command.

`ls`
This command will list all the files in your Downloads folder. Next, copy the name of the RStudio file by holding Ctrl + Shift then pressing c. RStudio should be labeled similar to this “rstudio-2023.06.2-561-amd64.deb”. Once you have copied the file name of RStudio. Type the following command into your Console/Terminal.

`sudo dpkg -i`
Once you have typed this part into your Console/Terminal window, add one space. Then paste the file name of RStudio that you previously copied. This command will install RStudio Desktop from the .deb file.

Example: `sudo dpkg -i rstudio-2023.06.2-561-amd64.deb`

If any issues become prominent, such as this error “error processing package rstudio (–install)” Paste the following command. Enter y or type yes when prompted.

`sudo apt --fix-broken install`
Now that we have fixed the installation simply repeat the step above, with the “sudo dpkg -i rstudio-2023.06.2-561-amd64.deb” command.

Installing R:
Lastly, installing R is very simple. The official installation guide can be viewed here:

https://cran.rstudio.com/

First, we need to add the R repository to our apt (Ubuntu) container by pasting the following command. Press enter when prompted.

`sudo add-apt-repository "deb https://cloud.r-project.org/bin/linux/ubuntu $(lsb_release -cs)-cran40/"`
This command will add the repository needed. Next paste the following command.

`wget -qO- https://cloud.r-project.org/bin/linux/ubuntu/marutter_pubkey.asc | sudo tee -a /etc/apt/trusted.gpg.d/cran_ubuntu_key.asc`

This command will add the public key for the repository. Next paste the following command. Type y or yes when prompted and press enter.

`sudo apt install r-base r-base-dev`
This command will install the R base required for RStudio. Once this is completed, refer to “Updating & Upgrading” to double-check there are no missing updates that need to be upgraded.

Utilizing RStudio:
RStudio and R are now installed and can be used via the apt (Ubuntu) container at any time. If your Console/Terminal window is still open simply paste the following command.

`rstudio`
This command will open RStudio in the apt container. If your Console/Terminal window isn’t open. You can simply access RStudio by opening either the Console or Terminal. Then typing “apx enter apt” then typing “rstudio”.

Useful Commands:
Some useful commands to take note of if this is your first time using a Terminal/Console window for running applications are listed below.

Command	Function
`exit`	Exit’s the current directory or window
`rstudio`	Runs the rstudio program
`R –version`	Displays the current R version installed
`apx enter apt`	Enters the apt (Ubuntu) container
`sudo apt update`	Pulls any updates
`sudo apt upgrade`	Upgrades any updates
