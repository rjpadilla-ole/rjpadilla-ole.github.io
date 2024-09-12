# Package Managers

## Objectives

* Learn about Package Managers
* Install the required Package Managers

## What are Package Managers?
Downloading software through GUI install wizards, or compiling by source is inefficient in the software engineer industry. Knowing how to manage software is a powerful skill in order to become a competent software developer. This is where Package Managers come in. 

Package Managers help us to add, remove, and update installed software from a centralized repository. Software installed by a package manager are bundled in **packages**. Packages contain the software you wanted to install **plus** any other software that is needed for you program to work. These added pieces of software are known as **dependencies**. 

Here is a list of some well-know package managers you may encounter in your career:

|||
|-|-|
|apt |Debian and related Linux distros package manager|
|yum |Package manager for Red Hat Linux systems|
|APK|Package manager for Alpine Linux|
|Homebrew |Package Manager for macOS systems|
|Chocolatey |Open-source package manager for Windows systems|
|pip |Package manager for Python modules|
|npm |Package manager for Node.js environment|

In this internship you would be mostly using npm and your operating system of choice package manager(choco, apt, or brew).

## Installing your OS package manager
**NOTE**: If you are using a Linux Debian distro like Ubuntu, you can skip to the next step.

### Windows
Install `chocolatey` by following the instructions at https://community.chocolatey.org/courses/installation/installing?method=installing-chocolatey#cmd

### macOS
Install the `homebrew` package manager using 
```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```
## Installing node
The npm package manager comes installed with node as a dependency. So lets install node on our machine.

We can use the official installer from Node's website https://nodejs.org/en/download/ but since we are aspiring developers we'll need some practice using our machine's package manager to install software.

On Windows, use the `choco` package manager to install node with the command:
```
choco install nvs
```

On Debian and Ubuntu based Linux distros, use:
```
curl -fsSL https://deb.nodesource.com/setup_current.x | sudo -E bash -
sudo apt-get install -y nodejs
```

On MacOS systems, use `brew` to install node using the command:
```
brew install node
```

## Verify installation

In the terminal, paste:
```
echo -e "node version $(node -v) \nnpm version $(npm -v)"
```
If you see both the node and npm version then you have successfully installed node.

---
#### Return to [First Steps](firststeps.md#Step_3_-_Software_Tutorial)
