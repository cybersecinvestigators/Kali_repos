# Kali_repos
Install kali tools in your linux distro

SET UP

1. sudo nano /etc/apt/sources.list

2. Scroll to the bottom of the list

3. Paste the below repo source in your sources.list
    
    deb http://http.kali.org/kali kali-rolling main non-free contrib

4.ctrl+s

5.ctrl+x

6.sudo apt-get update #(you will get an GPG error)


***************************Do not upgrade the system with this sourse enabled. This will surely crash your current os.********************


7.sudo apt-key adv --keyserver hkp://keys.gnupg.net --recv-keys 7D8D0BF6 #(this will fix the GPG error)
If this is not working, try this: <br>
wget -q -O - https://archive.kali.org/archive-key.asc | apt-key add 

8.sudo apt-get update

9.now you can install any kali tool in your linux distro.

10.sudo apt-get install sublist3r

11.sudo apt-get install metasploit-framework


***************************Keep in mind to comment the kali sourse added to the sources.list just after installing the kali tools.***************


12.sudo nano /etc/apt/sources.list

13.Enter a # before the kali repos to comment it.
    #deb http://http.kali.org/kali kali-rolling main non-free contrib

14.sudo apt-get update

15.sudo apt-get upgrade
