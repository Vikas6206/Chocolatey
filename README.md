# Chocolatey
How to use multiple software's at once via chocolatey ?

1] Navigate to chocolatey site and and copy the chocolatey installation commands:
                                        OR
Copy and paste the chocolatey command in command prompt.Make sure the command prompt is opened in the Administrator mode].

@"%SystemRoot%\System32\WindowsPowerShell\v1.0\powershell.exe" -NoProfile -InputFormat None -ExecutionPolicy Bypass -Command "iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))" && SET "PATH=%PATH%;%ALLUSERSPROFILE%\chocolatey\bin"

2] Now create a config file. For example package.config. This config file contains the XML which is used to pass the software name along with the version name (this is optional) & other parameters (which are also optional).







