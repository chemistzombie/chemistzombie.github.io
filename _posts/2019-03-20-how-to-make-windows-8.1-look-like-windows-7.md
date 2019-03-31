---
layout: default
title: How to make Windows 8.1 look like Windows 7
---	
![](/images/8.1AeroStart.png)

If you're tired of Windows 8.1's terrible interface, miss Windows 7's look and feel or if you decide to upgrade to 8.1 (and [avoid Windows 10 until 2023](/2019/03/10/what-to-do-when-windows-7-support-ends.html)) to anticipate Windows 7's end of support that would happen in the next few months but want to keep nice Aero visual style, you can make it look almost exactly like Windows 7 with some third-party tweaks.

Please note that you should only try this if you know what you're doing, as these tweaks might break your system if done improperly.

## Install the Aero Glass theme

## Get rid of that terrible Start screen with StartIsBack+

## Disable the lock screen and change the log on screen background to resemble Windows 7's (optional)
If you want to go all-out and tweak every single bit of the UI elements possible to resemble Windows 7, then do this one too.

<ol>
<li>Download this Windows 7 <a href="/images/windows7/windows_7_logon.png" target="_blank">logon screen background</a></li>
<li>Press Windows key + R and type regedit, hit Enter</li>
<li>Go to <strong>HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\Windows\Personalization</strong></li>
<li>Right click in the right pane, create a new <strong>DWORD</strong> value named NoLockScreen</li>
<li>Set this NoLockScreen value to 1</li>
<li>Right click in the right pane again and create a new <strong>string</strong> value named LockScreenImage</li>
<li>Set this value to the location of the logon screen background</li>
<li>Restart and the changes should now take effect</li>
</ol>