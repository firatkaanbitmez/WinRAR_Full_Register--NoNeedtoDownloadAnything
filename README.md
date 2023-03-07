# WinRAR Full Register (W/no need to download anything)

#Type (Windows Powershell) in the Windows search bar, right-click on the program that appears. Run it as administrator. Then copy and paste the code below. And press enter ok, now Winrar will be full version.




```

New-Item -ItemType file -Path "C:\Program Files\WinRAR\rarreg.key"
Set-Content -Path "C:\Program Files\WinRAR\rarreg.key" -Value "RAR registration data
Administrator
Enhanced Corporate
UID=ffd17c293f42b94c3b28
64122122503b281646f59a96b629958adcc52afe077f0682246ae5
54958b9c467ab240e5a9608a7f3372a80923a74c55e23fa85f410f
986b55ba1f344cb54742558c4674bec2f3f44597a594b865433801
d13141516c4c47c869c2b76309785d3d05606909687ce7e79c91d7
050a8254ed73508f5ca65007653492ae03ae96f7b77dafdce6140c
bfebaaa0c3514f197a99b9c3590b2d0d110aa2ba37d8a72160ada7
54fd3db8746dc7706cb36e57a5777074d497fa6d53592378887116"

```


#Other Method


```
if not "%1"=="am_admin" (powershell start -verb runas '%0' am_admin & exit /b)


@echo off
title C.By ARTHH
:Start
color 0A
cls


cd %userprofile%\Downloads


taskkill /f /im winrar.exe

curl -L "https://raw.githubusercontent.com/firatkaanbitmez/WinRAR_Full_Register--NoNeedtoDownloadAnything/main/rarreg.zip" -o rarreg.zip


timeout 2


powershell -command "Expand-Archive rarreg.zip"



timeout 2
copy "%userprofile%\Downloads\rarreg\rarreg.key" "C:\Program Files\WinRAR"  /Y




pause

exit


```
