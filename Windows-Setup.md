Windows Setups
=========

## 

## Software Installed

- Office2019
- edge
- vivado
- wechat
- QQ
- winrar
- abobe flash player
- sunlogin

## VMWare Windows 10 ftp set up

[referrence](https://www.windowscentral.com/how-set-ftp-server-windows-10)

### install the FTP server components on Windows 10

- control panel --> programs --> Turn Windows features on or off --> Internet Information Services --> check FTP server
- Check the Web Management Tools option with the default selections, but making sure that the IIS Management Console option is checked.

### configure an FTP server site on Windows 10

- control panel --> System and Security --> Administrative Tools --> Internet Information Services (IIS) Manager --> right-click Sites --> Add FTP Site 
>> no ssl
>> basic without anonymous

### Configuring firewall rules
- Windows Defender Security Center --> Firewall & network protection --> Allow an app through firewall --> Change settings -->  FTP Server

### Set up static ip
- cmd netsh interface ....
