Talkgroup-cell-padding
Python script to add user defined digit and pad the talkgroup field to 7 digits for use with Ham radio DMR hotspot software custom configuration.

Script written for Windows environment since most DMR radios only have windows apps for codeplug manipulation. 

Written by Ed, KE8TES

Frustrated to have to pad out TG cells again I wrote this quick script. 

This will work on all talkgroup lists to pad out the Talkgroup number to 7 digits for Custom network configuration. 

You will be asked to input the number you want as first digit while script is running.

When creating this script I realized TGIF has some talkgroups with 7 digits already and some of those did not have 4 as their leading digit. ***** Note:I use 4 as my TGIF custom configuration. This script will work with whatever digit you want from 1 - 9. *****
So I pulled out those with 7 which did not start with the desired leading digit; saving them to error file so they did not corrupt your codeplug in case they were overlooked.

This script opens a file browser dialog box so you can select your file through the interface and asks on the command line what leading number you want to use. From there the script runs and saves you outout file(s) to the directory your original file was in. Files are named TG_x_List.csv and TG_x_Errorlog.csv
The error log file only is created if talkgroups exist in original list equal to 7 digits then they are processed to see if any with 7 have same first digit as your leading digit and if so they are added back into the TG_x_List.csv file and the other 7 digit ones written to TG_x_Errorlog.csv

I did not add header row to the output files as you typically are just pasting the files together anyway.

Please use and modify as you see fit.

73s, Ed
