# Wlan-Profiles
Aplicación Wlan Profiles hackear contraseñas de wifi
Cómo ver la contraseña de una red WiFi a la que estás conectado en Windows 
Es muy fácil saber la contraseña de la red WiFi a la que estás conectado en Windows, te explicamos cómo.
Si ya te has conectado con tu PC o portátil Windows a una red con contraseña, y ahora quieres conectar 
también tu smartphone o alguien te pregunta la clave y no la recuerdas, es muy fácil “recuperarla” desde tu ordenador.
![](https://3.bp.blogspot.com/-oPb9wuB5nUk/WjRqB56LuCI/AAAAAAAAI3A/wonBBPq85QEbBQmgxkGoWDTxBNlMa6_mwCLcBGAs/s200/lpericena%2Bwifi.png)
https://lpericena.blogspot.com/2019/03/importar-perfiles-wlan-con-powershell.html
```
(netsh wlan show profiles) | Select-String “\:(.+)$” | %{$name=$_.Matches.Groups[1].Value.Trim(); $_} | %{(netsh wlan show profile name=”$name” key=
clear)}>>wifi.txt
```
![](https://1.bp.blogspot.com/-MklkR5Po3Lk/XIvsQU3GKCI/AAAAAAAAOI4/2-lJrvpaGRYGL0DGn2JOuJJaBx722ITDACLcBGAs/s1600/powershell.png)
```
$url="https://www.jesusninoc.com/2017/01/24/hackear-wifi-con-powershell-script-codificado-en-base64/"
$result = Invoke-WebRequest $url
[String]$execute=$result.AllElements | Where class -eq 'crayon-pre' | %{$_.innerText}
Invoke-Expression "powershell -encodedcommand $execute"
```
![](https://4.bp.blogspot.com/-ShOocj2HPUM/XIuW5KbQhdI/AAAAAAAAOHc/pUdjWkNLFachuykLCPACzlIQGt-YYvtaACLcBGAs/s1600/Screenshot_94.png)
### Otros comandos 
- información del interfas del sistema.
Get-NetAdapter
- Para ver información de la interfaz de red WiFi.
Get-NetAdapter -Name Wi-Fi
- Mostrar cmdlets relacionados con el adaptador de red.
gcm -Noun netadapter | select name, modulename
- Utilizando netsh.
netsh wlan show networks mode=bssid

- https://lpericena.blogspot.com/2019/03/importar-perfiles-wlan-con-powershell.html

Sigueme en las redes Sociales:
- 🌎Blogger          https://lpericena.blogspot.com/
- 💡 Github            https://github.com/Pericena
- 🐤 twitter             https://twitter.com/LPericena
