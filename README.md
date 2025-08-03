# ScreenLock
Transparent screen saver with password

F4CIO.ScreenLock is a transparent screen lock for Windows. When you step away from your computer, it automatically locks your keyboard and mouse, ensuring your privacy. However, you can still see everything happening on your screen, like movies, your company advertisement, or long processing tasks. This feature is known as "kiosk" mode, allowing you to keep an eye on your activities while keeping your computer secure.

## Features
- Customizable screen lock message and timeouts (idle, dim, and lock)
- Supports power actions like Standby, Hibernate, Shutdown, Reboot, etc. 
- Profile-based settings (Plugged In, On Battery or Playing Video) 
- Can work side-by-side with standard Windows power options 
- Free

## Security considerations
- Initial default password is 123. 
- If you forget password or get locked out for any reason just power off or restart your computer (by holding power button or plugging out). Auto-startup is not enabled initially and you will be able to continue.
- Password is stored as plain text and anyone with access to your files can see it. Therefore it is recommended to use different password from your secure windows password. This will be improved in next version.
- Don't use this software in serious environments where you need real safety and security.

## Minimum System Requirements
- Windows operating system (Windows 10 or newer recommended)
- .NET Desktop Runtime 6 (most newer Windows versions already have it. You can install it from
-- official page (https://dotnet.microsoft.com/en-us/download/dotnet/6.0) or directly for x86 from https://dotnet.microsoft.com/en-us/download/dotnet/thank-you/runtime-desktop-6.0.36-windows-x86-installer or for x64 from https://dotnet.microsoft.com/en-us/download/dotnet/thank-you/runtime-desktop-6.0.36-windows-x64-installer
- Must "run as Administrator" (locking keyboard or mouse globally in windows require this)
- ~140 Mb disk space

## Troubleshooting
- IT WON"T START OR FILE DISAPPEARED --> CHECK ANTI-VIRUS: For locking screen this software blocks keyboard and mouse globally. That is, by most antivirus software, seen as suspicious and they block, delete or quarantine such software automatically. You need to add .exe of this software file to exclusion list in your antivirus or temporarily disable antivirus until you find problem cause.
- IT WON'T START --> ADMIN RIGHTS: This software requires to run with admin privileges. If you are already logged in with administrator account type it will try to launch itself as admin but in some cases you must manually right-click and select "Run as administrator". 
- IT WON'T START --> FOLDER PERMISSION: This software requires write permission on folder where you placed it (its .exe file). By successfully running as administrator this permission is usually obtained automatically but in some cases you need to right click on folder, go to properties and allow full access to everyone or at least give write permissions to that folder for current account. Sometimes its enough to right click, go to properties and clear Read-only checkbox.
- IT WON'T START --> UNBLOCK EXE FILE: For most downloaded files windows mark them as unsafe or blocked. In some cases you need to right click downloaded .exe file, go to properties and check Unblock checkbox.
- IT WON'T RUN AFTER BOOT --> CHECK TASK SCHEDULER: software uses task scheduler to tell windows to run it on boot. In your start menu type taskschd.msc and in task scheduler you should see F4CIO.ScreenLock task. Insure its pointing to right exe file and is set to run with highest privileges. 
- OTHER ISSUES --> SEE .LOG FILE: software creates and starts writing to .log file immediately on run . Log file is beside .exe file. It can help you see if there is any error or track down other issues.
- OTHER ISSUES --> SEE WINDOWS EVENT LOG: in your start menu type eventvwr.exe and in Event Viewer go to WindowsLogs>Applications. Search for any error especially mentioning .NET.

## License
License Summary:
- Free for personal and commercial use
- You can freely distribute this software
- Author is not responsible for any damage it may cause

