

## xdg-open
        xdg-open .
        xdg-open http://github.com/the404
<hr>
## root
        su passwd root
        su root
<hr>
## exec a file
        ./sublime_text
<hr>
## tar
        .bz2 j
        .gz  z
        xf   extra tar
        cf   create tar
        .tar.xz   xz -d *.xz

        tar -jxf *.tar.bz2
        tar -zxf *.tar.gz
        1.xz -d *.xz => *.tar 2.tar -xf *.tar => d

## dpkg
        sudo dpkg - i *.deb    
        sudo dpkg -P *.deb
<hr>

## .rpm -> .deb
        sudo apt-get install alien    
        alien *.rmp
        sudo dpkg -i *.deb
<hr>
## node
sudo apt-get install nodejs-legacy
sudo apt-get install npm
node -v
npm -v
<hr>
##vscode
        create a new file named vscode in /usr/bin/vscode 
        cp /usr/bin/subl  change the path to code install location;
        
## /bin,/sbin ,/usr/bin,/usr/sbin difference
        /bin是系统的一些指令。bin为binary的简写主要放置一些系统的必备执行档例如:cat、cp、chmod df、dmesg、gzip、kill、ls、mkdir、more、mount、rm、su、tar等。
          
        /sbin一般是指超级用户指令。主要放置一些系统管理的必备程式例如:cfdisk、dhcpcd、dump、e2fsck、fdisk、halt、ifconfig、ifup、 ifdown、init、insmod、lilo、lsmod、mke2fs、modprobe、quotacheck、reboot、rmmod、 runlevel、shutdown等。
        
        /usr/bin　是你在后期安装的一些软件的运行脚本。主要放置一些应用软体工具的必备执行档例如c++、g++、gcc、chdrv、diff、dig、du、eject、elm、free、gnome*、 gzip、htpasswd、kfm、ktop、last、less、locale、m4、make、man、mcopy、ncftp、 newaliases、nslookup passwd、quota、smb*、wget等。

        /usr/sbin   放置一些用户安装的系统管理的必备程式例如:dhcpd、httpd、imap、in.*d、inetd、lpd、named、netconfig、nmbd、samba、sendmail、squid、swap、tcpd、tcpdump等。

## query
        whereis vscode && whereis subl 
        find /usr/bin -name vscode && find /usr/bin -name subl
        locate vscode && locate subl
        

## what is installed
    2017/4/9 17:00
        sublime
        vscode
        node
        npm
        rar
        unrar

        