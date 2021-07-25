# script-envio-email

https://scoop.sh/

1. PASSO:

Set-ExecutionPolicy RemoteSigned -scope CurrentUser

ou

iwr -useb get.scoop.sh | iex

2. PASSO:

Invoke-Expression (New-Object System.Net.WebClient).DownloadString('https://get.scoop.sh')

3. PASSO:

https://github.com/muquit/mailsend-go/releases/tag/v1.0.10

https://github.com/muquit/mailsend-go#downloading-and-installing

Features
Add a mail body
Support Multiple Attachments
Supports ESMTP Authentication
Supports StartTLS and SSL
Send mail to a list of users
Show SMTP server info
Fixes issues of mailsend

# Teste de Conexão SMTP:

mailsend-go -info -smtp smtp.gmail.com -port 587




