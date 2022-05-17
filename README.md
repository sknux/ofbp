# Open Frida By PID

If you have the problem below, you can try to use a latest version of frida server and client and identify if stay the problem or you can execute this tool.
### Failed to spawn: unexpectedly timed out while waiting for app to launch

The purpose of this tool is to identify and open an application with frida by PID.

*Frida is required*

Installing:
```html
git clone https://github.com/sknux/ofbp.git
cd ofbp && chmod +x ofbp

Ensure that your device is connected with the frida server and:

./ofbp appname
```

Example if your app is already open:
```bash
┌──(root㉿kali)-[/home/kali/]
└─# ./ofbp appname
Getting the PID and executing frida:

   . . . .   Connected to iOS Device (id=2b...1b1)
Attaching...                                                                                                                                     
[iOS Device::PID::3277 ]->                                       
```
-------------------------------------------------------

Example if your app is closed:
```bash
┌──(root㉿kali)-[/home/kali/]
└─# ./ofbp appname
Please, open the app and then press enter

Getting the PID and executing frida:

   . . . .   Connected to iOS Device (id=2b...1b1)
Attaching...

[iOS Device::PID::3294 ]->
```
