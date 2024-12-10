__________
| .basrc |
----------
alias squeuemy='squeue -u $(whoami) -o "%i %j %t %M %D %R"'
alias lsmy='ls -ltrh'	# Show files with most recent at the bottom and human-readable format
alias catlast='cat "$(ls -t | head -n 1)"'	# Print most recent file content
alias nanolast='nano "$(ls -t | head -n 1)"'	# Read most recent file content

__________________
| Monitor System |
------------------
top [-u -s 10] (running porcesses, memory usage and similar)  
htop (like above, more readable info)  
iostat (I/O per terminal, device and SPU summary statistics)  
vm_stat (Mac virtual memory statistics)  
df (drive space used and free)    
diskutil list (like above)  
w (who is logged in, what are doing and system load)  
iStats (temperature stats)  
du -ks * (disk space all folders below current directory are using)  


______________
| Monitor Net|
--------------
nettop (updated information about the network)  
ifconfig (network interface and IP protocol details)  
ipconfig (like above)  
nmap -sP 192.168.1.* (list all the devices connected to home network with theri IPs)  


________
| Both |
--------
fs_usage [-f network] (file activity for both diks and network)  
	fs_usage -w (changes the output so that it's not dependent on window size)  
	fs_usage [process name] (shows only results that contain the specified process)  
	fs_usage pid [process ID] (find out the process ID)  
	fs_usage | grep [any search term] (only include lines that match the search term typed in)  
glances (like htop, but also with network info)  


___________
| General |
-----------
cd (enter directory)  
ls [-la] (show everything with details in current directory)  
pwd (print current directory)  
clear (clear terminal screen)  
rm (remove directory)  
cp (copy)  
mkdir (make directory)  
man (manual for everything, ex. man top)  
touch (create file)  
open (open file)  
grep (match word in lines)  
	Examples: grep 'word' filename; grep 'word' file1 file2 file3; cat otherfile | grep 'something'  


________________
| Text editors |
----------------
vim (press esc and save with :x when in insert mode, otherwise exit with :q)  
	vim -c 'starstarttinsert' file.txt (to enter insert mode)  
cat  


________________
|     Media    |
----------------
youtube_dl (download YouTube videos in multiple formats as well as quality audio at high speed)  



________________
|  Directories |
----------------
rsync -avzh SOURCE DESTINATION (file transfer program capable of efficient remote update  
via a fast differencing algorithm. Can synchronize both local and remote directories)  
