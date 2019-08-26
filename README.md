# Windows-WSL-Ubuntu-LAMP-Wordpress

Download stack file to windows download folder.

#### Open powershell from powerusers menu.

Press `WIN+X` to open powerusers menu.

Select `Windows Powershell (Admin)`.

Choose `YES` at prompt.

#### Enable Windows Optional Feature Microsoft-Windows-Subsystem-Linux.

Run `Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux`

#### Install Ubuntu for WSL Windows Store App.

Run `Invoke-WebRequest -Uri http://tlu.dl.delivery.mp.microsoft.com/filestreamingservice/files/c4a0955e-2d68-4c61-8c19-4c4ffbff7b55?P1=1565144663"&"P2=402"&"P3=2"&"P4=aHQzGh1lof5aA4KIcP2Q0ovQrSrRpoT45Lr%2f6qfonT1YDCkavQTnD7UFnTrXAJkiBq4P%2bwqzPMOkicZBQhWXSg%3d%3d -OutFile ubuntu.appx -UseBasicParsing`

Run `Add-AppxPackage .\ubuntu.appx`

#### Start Ubuntu, access windows download directory, run stack.sh.

Run `ubuntu`

Run `cd /mnt/c/users/brett/downloads/`

Run `sudo bash stack.sh`