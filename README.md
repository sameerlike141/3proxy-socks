3proxy install script for Debian / Ubuntu VPS (ver 0.8.10)
======================================================

**HOW TO :**

Download, make executable and run with these lines :

    wget --no-check-certificate https://raw.github.com/h1777/3proxy-socks/master/3proxyinstaller.sh
    chmod +x 3proxyinstaller.sh
    ./3proxyinstaller.sh

For servers with multiple IP's use these lines to download the correct config file for multiple ip's:

    wget --no-check-certificate https://raw.github.com/h1777/3proxy-socks/master/3proxy_installerX.sh
    chmod +x 3proxy_installerX.sh
    ./3proxy_installerX.sh
    
After install : CHANGE DEFAULT USERNAME AND PASSWORD !!! 

    nano /etc/3proxy/.proxyauth
	
Example change line inside .proxyauth

    johndoe:CL:johndoepassword123

You can also change the port, default is 3128 (OPTIONAL)

    nano /etc/3proxy/3proxy.cfg
    

Once you've change the username / password you can start the proxy 
(or reboot the VPS as 3proxy has been added to the init scripts and will autostart)

    /etc/init.d/3proxyinit start
	
For Uninstall Download, make executable and run with these lines :

	wget --no-check-certificate https://raw.github.com/h1777/3proxy-socks/master/3proxyuninst.sh
	chmod +x 3proxyuninst.sh
	./3proxyuninst.sh

**Script last tested on April 2018 on the following fresh VPS install distros :**

- Ubuntu 16.04 64bit (AWS)


**Script will run on :**
- ?
