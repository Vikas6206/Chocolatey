# Chocolatey
How to install multiple software's at once via chocolatey ?

1] Navigate to chocolatey site and and copy the chocolatey installation commands:

                                        OR
                                        
Copy and paste the chocolatey command in command prompt.Make sure the command prompt is opened in the Administrator mode].

@"%SystemRoot%\System32\WindowsPowerShell\v1.0\powershell.exe" -NoProfile -InputFormat None -ExecutionPolicy Bypass -Command "iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))" && SET "PATH=%PATH%;%ALLUSERSPROFILE%\chocolatey\bin"

2] Now create a config file. For example package.config. This config file contains the XML which is used to pass the software name along with the version name (this is optional) & other parameters (which are also optional).

NOTE:- You can't provide any kind of XML comments in the config files. Also, note that the only sofware whose packages are there in the chocolatey can be installed.

3]In this project, package.config contains the list of software which needs to be installed on your machine.
Download this project and Open command prompt & navigate to the directory where the config file is present. Type the following command to install the softwares present in the config files.

    choco install package.config -y
    
  Here "-y" is used to bypass the installation prompts (Ex:- Are you sure you want to install this software ? [Y]es [N]o)
  
Syntax to install the softwares via config files:

 choco install <path of the config file> <optional parameters>
  
  






