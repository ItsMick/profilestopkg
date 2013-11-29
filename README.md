## profilestopkg

This tool wraps up OS X profiles into pkgs.

This script can also import the packages to your munkirepo, via munkiiport. It will automatically create the necessary keys; installcheck_script, uninstall_Script, name, and minimum OS Version(10.7).

## Examples

### Minimum required to create a flat package from a mobileconfig file.

profilestopkg -m /path/to/com.myorg.cong.mobileconfig

### Create a package and import it directly to munki

profilestopkg -m /path/to/com.myorg.cong.mobileconfig -i


## Usage:

profilestopkg --mobileconfig <filename> [--packagename <name>] [--version <value>] [--importtomunki]

Options:

  -h, --help            show this help message and exit

  -m MOBILECONFIG, --mobileconfig=MOBILECONFIG
                        The Mobileconfig file you would like to have packages.
                        You must use the absolute Path.

  -p PACKAGENAME, --packagename=PACKAGENAME
                        Define a output package name.

  -i, --importtomunki   import the package direcrly into munki.

  -v VERSION, --version=VERSION
                        Set package version.


## Thanks

Profiletopkg makes use of Greg Neagle's FoundationPlist lib.
