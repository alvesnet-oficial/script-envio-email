# script-envio-email

https://scoop.sh/

1. PASSO:

Set-ExecutionPolicy RemoteSigned -scope CurrentUser

ou

iwr -useb get.scoop.sh | iex

2. PASSO:

Invoke-Expression (New-Object System.Net.WebClient).DownloadString('https://get.scoop.sh')


