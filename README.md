# msfinstaller
Metasploit Framework Installer from source

Originally created by DarkOperator [https://github.com/darkoperator]. 
Forked for updates to installing Metasploit, Ruby, and Armitage on a base Ubuntu install.

Usage:
msfinstaller -i -p <password> -r [-h]
* -i Installs Metasploit Framework with Armitage
* -p Initital password for postgresql database of Metasploit
* -r Install latest Ruby RVM (Metasploit requires ruby version => 2.0
* -h Help Message

Examples:
msfinstaller -i -p msf -r

***Current Bugs***
You will need a restart. Ruby isn't sourcing bashrc correctly and requires you to bounce the box.

If you get:
"Could not find XXXX in any of the sources
Run `bundle install` to install missing gems."
Then do the following:
#>cd /usr/local/share/metasploit-framework/
#>bundle install

You may need to logout and log back in to properly set your bashrc settings.

All Credit goes to Dark Operator for original script

## another

1、安装msf

1.1、打开终端，进入安装目录（你想放在哪就进哪

cd /opt

curl https://raw.githubusercontent.com/rapid7/metasploit-omnibus/master/config/templates/metasploit-framework-wrappers/msfupdate.erb -o msfinstall

1.2、chmod 755 msfinstall

1.3、./msfinstall

1.4 msfconsole
	....?	yes
