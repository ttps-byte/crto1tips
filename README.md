![Image](https://github.com/user-attachments/assets/472360ea-1a35-4845-b4f9-b038313446c8)

# CRTO I great commands

In this repo, i share all things that you need to pass in CRTO I in a easy way. So, follow these steps to have sucessfull. good luck!  

# Setup 
Modify C2 Profile to add amsi bypass above http-get (We need do this to get informations about 1° flags).  
``vi /opt/cobaltstrike/c2-profiles/normal/webbug.profile``  
Inside of the "webbug.profile" file, you need leet this document exactly like this (below).  
``` 
Post-ex {
set amsi_disable "true";
set obfuscate "true";
set smartinject "true"; set spawnto_x64 "%windir%\\sysnative\\dllhost.exe"; set
spawnto_x86 "%windir%\\syswow64\\dllhost.exe";
}
```
