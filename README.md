# Linux-essentials
A quick reference guide for essential Linux commands, designed to help beginners and advanced users alike. It covers file management, process control, networking, and more, with examples for easy use. Ideal for simplifying workflows and boosting productivity. (These are the most common commands used). 


Basic Navigation and File Management

pwd
Description: Prints the current working directory.
Usage:
pwd


ls [options] [directory]
Description: Lists files and directories in the specified directory.
Usage:
ls -l /home/user/Documents


cd [directory]
Description: Changes to the specified directory.
Usage:
cd /var/www/html


cd ..
Description: Moves up one level in the directory structure.
Usage:
cd ..

mkdir [directory_name]
Description: Creates a new directory.
Usage:
mkdir new_folder


rmdir [directory_name]
Description: Removes an empty directory.
Usage:
rmdir old_folder


touch [file_name]
Description: Creates an empty file.
Usage:
touch newfile.txt

cp [source] [destination]
Description: Copies files or directories.
Usage:
cp file.txt /backup/


mv [source] [destination]
Description: Moves or renames files or directories.
Usage:
mv oldname.txt newname.txt


rm [file_name]
Description: Deletes a file.
Usage:
rm unwantedfile.txt


rm -r [directory_name]
Description: Recursively deletes a directory and its contents.
Usage:
rm -r old_directory

Viewing and Editing Files


cat [file_name]
Description: Displays the contents of a file.
Usage:
cat file.txt


more [file_name]
Description: Views file contents one page at a time.
Usage:
more longfile.txt


less [file_name]
Description: Views file contents with navigation options.
Usage:
less largefile.txt


head -n [number] [file_name]
Description: Displays the first n lines of a file.
Usage:
head -n 10 file.txt


tail -n [number] [file_name]
Description: Displays the last n lines of a file.
Usage:
tail -n 5 logfile.txt


nano [file_name]
Description: Opens a file in the Nano text editor for editing.
Usage:
nano config.conf


vim [file_name]
Description: Opens a file in the Vim text editor.
Usage:
vim script.sh


File Permissions and Ownership


chmod [permissions] [file_name]
Description: Changes the file permissions for user, group, and others.
Usage:
chmod 755 script.sh


chown [owner]:[group] [file_name]
Description: Changes the ownership of a file or directory.
Usage:
chown root:admin config.conf


chmod u+x [file_name]
Description: Grants execute permission to the file’s owner.
Usage:
chmod u+x run_me.sh


System Information


uname -a
Description: Displays system information, including kernel version and machine details.
Usage:
uname -a


df -h
Description: Displays disk space usage in a human-readable format.
Usage:
df -h


du -h [directory]
Description: Displays disk usage of a directory in a human-readable format.
Usage:
du -h /home/user


top

Description: Displays real-time system resource usage, including CPU, memory, and process info.
Usage:
top


ps aux
Description: Lists all running processes with detailed information.
ps aux


free -h
Description: Displays memory usage in a human-readable format.
free -h


uptime
Description: Displays how long the system has been running.
Usage:
uptime


Networking

ifconfig
Description: Displays network interfaces and their IP addresses.
Usage:
ifconfig


ping [host]
Description: Pings a remote host to check network connectivity.
Usage:
ping google.com


netstat -tuln
Description: Displays active network connections.
Usage:
netstat -tuln


wget [URL]
Description: Downloads a file from a URL.
Usage:
wget http://example.com/file


curl -O [URL]
Description: Downloads a file using curl.
Usage:
curl -O http://example.com/file


ssh [user]@[host]
Description: Connects to a remote machine via SSH.
Usage:
ssh user@192.168.1.1


Searching and Finding Files


find [directory] -name [file_name]
Description: Searches for a file by name within a directory.
Usage:
find / -name config.conf


locate [file_name]
Description: Quickly finds a file by name using the pre-built locate database.
Usage:
locate bashrc


grep "[pattern]" [file_name]
Description: Searches for a pattern inside a file.
Usage:
grep "error" /var/log/syslog


grep -r "[pattern]" [directory]
Description: Recursively searches for a pattern inside files within a directory.
Usage:
grep -r "404" /var/www/html


Package Management (Ubuntu / Debian)


sudo apt update
Description: Updates the list of available packages and their versions.
Usage:
sudo apt update


sudo apt upgrade
Description: Upgrades all installed packages to their latest versions.
Usage:
sudo apt upgrade

sudo apt install [package] (usually indicated by the OS)
Description: Installs a package.
Usage:
sudo apt install vim


sudo apt remove [package]
Description: Removes a package from the system.
Usage:
sudo apt remove vim


dpkg -i [package.deb]
Description: Installs a .deb package manually.
Usage:
sudo dpkg -i package.deb


(If you don't know how some commands work, you can always just man the command) 
(Ex: man chmod) 




Continue generating
