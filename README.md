## profilestopkg

This tool wraps up OS X profiles into pkgs. It also has the ability to import the packages to your munki repo.

## Usage: 
profilestopkg --mobileconfig filename [--packagename value] [--version value] [--importtomunki]

Options:

  -h, --help            show this help message and exit

  -m MOBILECONFIG, --mobileconfig=MOBILECONFIG
                        The Mobileconfig file you would like to have packages.
                        You must use the absolute Path. Required

  -p PACKAGENAME, --packagename=PACKAGENAME
                        Define a output package name.

  -i, --importtomunki   import the package direcrly into munki.

  -v VERSION, --version=VERSION
                        Set package version 

## Thanks

Profiletopkg makes use of Greg Neagle's wonderful FoundationPlist lib. FoundationsPlist.py is a tool to generate and parse MacOSX .plist files.