## Setting Up Your Programming Assignment Environment

The Machine Learning course includes several programming assignments which you’ll need to finish to complete the course. The assignments require the Octave or MATLAB scientific computing languages.

* Octave is a free, open-source application available for many platforms. It has a text interface and an experimental graphical one.
* MATLAB is proprietary software, but a free trial license to MATLAB Online is being offered for the completion of this course.

## FAQ

### Does it cost money?

While you’re taking the course, both software packages are available free of charge. Octave is distributed under the GNU Public License, which means that it is always free to download and distribute. MATLAB Online licenses are available for completing the programming assignments in the course only. For any other purposes (like your own work after you complete the course), MATLAB can be licensed to individuals or companies from Mathworks directly.

### Is there a difference in quality?

There are several subtle differences between the two software packages. MATLAB may offer a smoother experience (especially for Mac users), contains a larger number of functions, and can be more robust to failure. However, the functions used in this course are available in both packages, and many students have successfully completed the course using either.

### How do I install one of them?

To install Octave, see installation instructions for Windows, Mac OS X (10.10 Yosemite and 10.9 Mavericks), other Mac OS X, or GNU/Linux. Instructions are found in the next section.

* Accessing the free MATLAB Online trial
* Downloading the exercise files for MATLAB Online and newer versions of MATLAB desktop

## Access the MATLAB Online Trial and the Exercise Files for MATLAB Users

### Access MATLAB Online

Access to MATLAB Online is being provided by MathWorks to Machine Learning students for the duration of the course. MATLAB Online is the online version of the MATLAB desktop program. It provides most features of the original program in a web-based interface. No download or installation is required, and the program can be accessed from any computer running a common web browser.

### Follow the steps below to access MATLAB Online

1. If you do not already have one, create a MathWorks account.

2. Click on the MATLAB Online license link and provide your MathWorks account credentials (if requested).

3. Click on the blue 'Access MATLAB Online' button, and log-in to MATLAB Online with your MathWorks account credentials.

4. Confirm that you have access to MATLAB Online. For help with MATLAB Online access or technical issues, see the MATLAB Help discussion forum.

Bookmark https://matlab.mathworks.com/ for quicker access to MATLAB Online in the future.

## Access the Updated Exercise Files for MATLAB Online and MATLAB Desktop version R2019b and later

The original programming exercise files cannot be used with MATLAB Online and MATLAB Desktop beginning with version R2019b. The files below have been modified specifically for MATLAB Online and MATLAB R2019b+ users. Octave users and MATLAB Desktop users running earlier versions of MATLAB should use the original exercise files which are posted at the end of certain weeks.

#### Download the updated exercise zip file:

To add the programming exercise files to MATLAB Online, first download them files as a zip file to your desktop using the link below, then rename the file to: `machine-learning-ex.` Note that Coursera adds extra characters to the filename upon download that must be removed.

        machine-learning-ex.zip

### To add the exercise files to MATLAB Online: 

1. Open MATLAB Online and click the 'Upload' button in the 'Home' tab.

2. Use the folder browser window to find and select the 'machine-learning-ex.zip' file, then click 'Open'. You should see the file in MATLAB Online after upload is complete.

3. Unzip the file by entering the command: unzip machine-learning-ex.zip at the command line.

Note that you can access your files even after your MATLAB Online license expires through MATLAB Drive. MATLAB Desktop R2019b+ users can download and unzip the files to a folder of your choice.

## Completing the programming exercises using the updated exercise files

There are eight programming exercises in the course, the first is posted at the end of Week 2. When you reach a programming exercise page in the course, do not download the exercise files, as the necessary files for all exercises are included in the zip folder above. `Make note of your assignment token listed on the exercise page, however, you will need it to submit your solutions.`

Instructions for completing the exercises and tips for troubleshooting common problems are found in the included `README.mlx` file. Before attempting your first programming exercise, read the instructions in `README.mlx`. These instructions differ slightly from the instructions and video demonstration provided later, which only apply to Octave users and MATLAB Desktop users running older versions of MATLAB.

## Installing Octave on Windows

### Installing Octave on Windows

`Use this link to install Octave for windows:`
http://wiki.octave.org/Octave_for_Microsoft_Windows

`Octave on Windows can be used to submit programming assignments` in this course but will likely need a patch provided in the discussion forum. Refer to https://www.coursera.org/learn/machine-learning/discussions/vgCyrQoMEeWv5yIAC00Eog? for more information about the patch for your version.

`Warning` - Do not install Octave 4.0.0; checkout the "Resources" menu's section of "Installation Issues".

## Installing Octave on Mac OS X (10.10 Yosemite and 10.9 Mavericks)

### Installing Octave on Mac OS X (10.10 Yosemite and 10.9 Mavericks)

Mac OS X has a feature called Gatekeeper that may only let you install applications from the Mac App Store. You may need to configure it to allow the Octave installer. Visit your System Preferences, click Security & Privacy, and check the setting to allow apps downloaded from Anywhere. You may need to enter your password to unlock the settings page.

2. Download the Octave 3.8.0 installer or the latest version that isn't 4.0.0. The file is large so this may take some time.

3. Open the downloaded image, probably named GNU_Octave_3.8.0-6.dmg on your computer, and then open Octave-3.8.0-6.mpkg inside.

4. Follow the installer’s instructions. You may need to enter the administrator password for your computer.

5. After the installer completes, Octave should be installed on your computer. You can find Octave-cli in your Mac’s Applications, which is a text interface for Octave that you can use to complete Machine Learning’s programming assignments.

Octave also includes an experimental graphical interface which is called Octave-gui, also in your Mac’s Applications, but we recommend using Octave-cli because it’s more stable.

Note: If you use a package manager (like MacPorts or Homebrew), we recommend you follow the package manager installation instructions.

`Warning` - Do not install Octave 4.0.0"; checkout the "Resources" menu's section of "Installation Issues".

## Installing Octave on Mac OS X (10.8 Mountain Lion and Earlier)

### Installing Octave on Mac OS X (10.8 Mountain Lion and Earlier)

If you use Mac OS X 10.9, we recommend following the instructions above. For other Mac OS X versions, the Octave project doesn’t distribute installers. We recommend installing Homebrew, a package manager, using their instructions.

`Warning` - Do not install Octave 4.0.0"; checkout the "Resources" menu's section of "Installation Issues".

## Installing Octave on GNU/Linux

### Installing Octave on GNU/Linux

We recommend using your system package manager to install Octave.

On `Ubuntu`, you can use:

* sudo apt-get update && sudo apt-get install octave

On `Fedora`, you can use:

* sudo yum install octave-forge

Please consult the Octave maintainer’s instructions for other GNU/Linux systems.

`Warning` - Do not install Octave 4.0.0"; checkout the "Resources" menu's section of "Installation Issues".

## More Octave/MATLAB resources

### Octave Resources

At the Octave command line, typing `help` followed by a function name displays documentation for a built-in function. For example, `help plot` will bring up help information for plotting. Further documentation can be found at the Octave documentation pages.

### MATLAB Resources

At the MATLAB command line, typing help followed by a function name displays documentation for a built-in function. For example, help plot will bring up help information for plotting. Further documentation can be found at the MATLAB documentation pages.

### Introduction to MATLAB with Onramp

Made for MATLAB beginners or those looking for a quick refresh, the MATLAB Onramp is a 1-2 hour interactive introduction to the basics of MATLAB programming. `Octave users are also welcome to use Onramp` (requires creation of a free MathWorks account). To access Onramp:

1. If you don’t already have one, create a MathWorks account at: https://www.mathworks.com/mwaccount/register

2. Go to: https://matlabacademy.mathworks.com/ and click on the MATLAB Onramp button to start learning MATLAB!

### MATLAB Programming Tutorials

These short tutorial videos introduce MATLAB and cover various programming topics used in the assignments. Feel free to watch some now and return to reference them as you work through the programming assignments. Many of the topics below are also covered in MATLAB Onramp. `*Indicates content covered in Onramp`.

#### Get Started with MATLAB and MATLAB Online

* What is MATLAB?*
* MATLAB Variables*
* MATLAB as a Calculator*
* MATLAB Functions*
* Getting Started with MATLAB Online
* Managing Files in MATLAB Online

#### Vectors

* Creating Vectors*
* Creating Uniformly Spaced Vectors*
* Accessing Elements of a Vector Using Conditions*
* Calculations with Vectors*
* Vector Transpose

#### Visualization

* Line Plots*
* Annotating Graphs*
* Multiple Plots*

#### Matrices

* Creating Matrices*
* Calculations with Matrices*
* Accessing Elements of a Matrix*
* Matrix Creation Functions*
* Combining Matrices
* Determining Array Size and Length
* Matrix Multiplication
* Reshaping Arrays
* Statistical Functions with Matrices

#### MATLAB Programming

* Logical Variables*
* If-Else Statements*
* Writing a FOR loop*
* Writing a WHILE Loop
* Writing Functions
* Passing Functions as Inputs

#### Troubleshooting

* Using Online Documentation*
* Which File or Variable Am I Using?
* Troubleshooting Code with the Debugger
