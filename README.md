# uninstall_expressvpn.Ps1
I created this to uninstall preloaded Express VPN bloatware on Windows systems. The app can, of course, be uninstalled through the "add/remove" menu on Windows, but that does not help at scale. 
The install is not an MSI, and the remove-package Cmdlet does not work for it. If look for the uninstall string in the registry, it will show a different path on different computers (possibly due to versioning or due to purposeful obfuscation. ) This script will loop through the possible directories and run the silent uninstall. This was written with RMMs in mind, but should work however it is deployed.
