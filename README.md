# moka_to_genapp

 This script is designed to be called by MOKA and run from a trust machine (using the python executable on the S drive).

The script takes an argument -g GEL Participant ID 

eg 

`S:\Genetics_Data2\Array\Software\Python\python.exe ssh_n_run.py -g 12345678`

Using the paramiko module it then ssh's into the server using the host, username and password provided in the host.txt password.txt and username.txt files.

Using the full path to the python executable found within the pyODBC conda environment the gel_report.py script is called, passing the GEL participant ID as an argument.

The stderr and stdout are printed.

Not included in this repo are three text files, username.txt, password.txt and host.txt which all contain a single line containing either the password, username or hostname (IP address).

See 'Generating GEL reports' on barista for instructions for installation of dependancies/python packages
