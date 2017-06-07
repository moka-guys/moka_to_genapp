# moka_to_genapp

 This script is designed to be called by MOKA and run from a trust machine (using the python executable on the S drive).

The script takes an argument -g <GEL Participant ID>

It then ssh's into the server provided in the host.txt file using the username and password provided in the password and username files.

Using the path to the python executable found within the environment the python script is called, passing the GEL participant ID as an argument.

The stderr and stdout are printed.

Not included in this repo are three text files, username.txt, password.txt and host.txt which all contain a single line containing either the password, username or hostname (IP address).
