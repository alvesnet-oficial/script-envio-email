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

# Usando SSL. Nota porta e diferente:

mailsend-go -info -smtp smtp.gmail.com -port 465 -ssl

# Use as configurações padrão para provedores de e-mail conhecidos

Não se preocupe com as configurações de -smtp, -port e -ssl para provedores de e-mail bem conhecidos. Isso funciona para gmail, yahoo, outlook, gmx, zoho e aol.

mailsend-go -info -use gmail

# Enviado email como uma Mensagem de texto:

Observe que "auth" é um comando e recebe os argumentos -user e -pass. "body" também é um comando e aqui tomou -msg como argumento. O comando "corpo" não pode se repetir, se especificado mais de uma vez, será utilizada a última.

    mailsend-go.exe -sub "teste" -smtp smtp.gmail.com -port 465 auth -user suporte@alvesnet.com.br -pass xxxxxxx* -from suporte@alvesnet.com.br -to suporte@alvesnet.com.br body -msg "hello" attach -file c:\ScriptBackup\Logs\Terca\Desktop_Bkp.txt
    

5. PASSO:

https://docs.microsoft.com/pt-br/office/vba/language/reference/user-interface-help/msgbox-function

https://www.ti-enxame.com/pt/windows/comando-do-windows-cmd.exe-para-exibir-uma-caixa-de-mensagens-com-tempo-limite/1043772657/

# 48	Exibe o ícone Mensagem de Aviso:

mshta "javascript:var sh=new ActiveXObject( 'WScript.Shell' ); sh.Popup( 'Backup para HD Externo Iniciado!', 10, 'Backup HD Externo!', 48 );close()"

# 64	Exibe o ícone Mensagem Informativa.

mshta "javascript:var sh=new ActiveXObject( 'WScript.Shell' ); sh.Popup( 'Backup para HD Externo Concluído!', 10, 'Backup HD Externo!', 64 );close()"

# 16	Exibe o ícone Mensagem Crítica.

mshta "javascript:var sh=new ActiveXObject( 'WScript.Shell' ); sh.Popup( 'Backup para HD Externo Falhou!', 10, 'Backup para HD Externo!', 48 );close()"



