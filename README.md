# May R be with you: how you can revolutionise your research workflow
This repository contains files, instructions and data for the R workshop given in the ÉcoLac autumn workshop 2018, organised by the Groupe de recherche interuniversitaire en limnologie en environnement aquatique (GRIL).

## About
The ÉcoLac workshop takes place every year in autumn at the Station biologique de Laurentides (SBL) close to Montréal. It provides undergraduate, graduate students and postdocs the opportunity to attend several workshops they are interested in. This year, I will provide a workshop covering the power of R - not the statistical power but how one can use R to optimise a research workflow.

## Conference abstract
Have you experienced never ending weekends fiddling in your excel sheets? Copy and pasting, or even going back to your raw data because you have figured a "stupid" mistake after months of data analyses? It's frustrating. In a world of science that moves towards transparency, reproducibility and sharing, you will learn to call R your best friend. Commonly known as an open-source statistical software, the power of R goes beyond pure statistics. During this workshop, we will explore how you can use the software to save precious time (and frustration) and organise your analyses so you can focus on the more important things in science. Note that the content covered in the presentation and workshop will be suitable for both beginners and advanced users.

## Workshop abstract
The workshop will be provided for beginners and more advanced participants. Beginners, will start with an introduction into the R language and basic commands to organise your data. Advanced participants who already speak R, we will directly dig into the coding of loops, enabling you to automatise data extraction from raw files. An example dataset will be provided for the participants to create a script to automatise data analysis, from data extraction to plotting your data using ggplot.

**Important:** participants who wish to attend the workshop must bring their own laptop and make sure to install R and R studio in advance. Please follow the instructions provided below.

---
 
## Pre-workshop: Installation of R and R studio
### Base R
#### - Windows users
1. Open internet browser and open www.r-project.org
2. Click the "download R" link in the middle of the page in the section "Getting started"
3. Choose a CRAN-mirror (e.g. Canadian mirror from the University of Toronto http://cran.utstat.utoronto.ca/)
4. Choose "Download R for Windows" at the top of the page.
5. Click on "install R for the first time" link at the top of the page
6. Click "Download R for Windows" and save the executable file on your PC.
7. Double-click on the .exe file and follow the installation instructions
8. You are all set for base R, continue with installing R studio

#### - Mac users
1. Open internet browser and open www.r-project.org
2. Click the "download R" link in the middle of the page in the section "Getting started"
3. Choose a CRAN-mirror (e.g. Canadian mirror from the University of Toronto http://cran.utstat.utoronto.ca/)
4. Choose "Download R for (Mac) OS X" at the top of the page.
5. Go to the section "Latest releases"
6. Check your OS version and if you have OS X 10.11 (El Capitan) and higher,click on the latest .pkg file and download (If you have an older OS version, select an appropriate .pkg file as indicated on the page and download)
7. Save the .pkg file, double-click and follow the installation instructions
8. You are all set for base R, continue with installing R studio

#### - Linux users
It's easiest if you refer to your Linux package management system (i.e. Software center) but often it is not the most current version, therefore I recommend to download R Base directly from a Cran server. The following instructions are for Ubuntu but you can find tutorials for any other distributions online:

1. Open terminal
2. Add R repository: add a line to your /etc/apt/source.list file. 
```
sudo echo "deb http://cran.rstudio.com/bin/linux/ubuntu bionic-cran35/" | sudo tee -a /etc/apt/sources.list
```
   Note the "bionic-cran35" refers to Ubuntu 18.04 if you have a different version just change it (e.g. 16.04 = "xenial").   You can find the names for each distribution and version here: https://cloud.r-project.org/ > "Download R for Linux" > click on your distribution
  
3. Add R to Ubuntu keyring
```
gpg --keyserver keyserver.ubuntu.com --recv-key E084DAB9
gpg -a --export E084DAB9 | sudo apt-key add -
```
4. Install R-Base
```
sudo apt-get update
sudo apt-get install r-base r-base-dev
```
5. You are all set for base R, continue with installing R studio

### R Studio
R studio is a user friendly platform that makes working with R easier. Therefore, I highly recommend it, especially for someone being new to R. We will mainly work in R studio in the workshop, so if you only install base R the first thing I will tell you is to install it.
1. Go to https://www.rstudio.com/products/rstudio/download/#download
2. Navigate to the "Installers for Supported Platforms" section
3. Choose an installer for your OS (Windows, Mac, Ubuntu etc.), click and save
4. Double-click on your .exe (Windows), .dmg (Mac) or .deb (Ubuntu) file and follow installation instructions
