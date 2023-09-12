# Talkgroup-cell-padding
Python script to add user defined digit and pad the talkgroup field to 7 digits for use with Ham radio DMR hotspot software custom configuration.

Script written for Windows environment since most DMR radios only have windows apps for codeplug manipulation. 
Written by Ed, KE8TES
Frustrated to have to pad out TG cells again I wrote this quick script. 

This will work on all talkgroup lists to pad out the Talkgroup number to 7 digits for Custom network configuration. 

You will be asked to input the number you want as first digit while script is running.

When creating this script I realized TGIF has some talkgroups with 7 digits already and some of those did not have 4 as their leading digit.
So I pulled out those with 7 which did not start with the desired leading digit; saving them to error file so they did not corrupt your codeplug in case they were overlooked.

I did not add header row to the output files as you typically are just pasting the files together anyway.

Please use and modify as you see fit.

73, Ed
