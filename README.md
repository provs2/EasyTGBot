# Benvenuto nell'installazione di EasyTGBot!
_Prima di tutto, specifichiamo che per utilizzare EasyTGBot bisogna avere una conoscienza almeno minima di PHP_
test 3
## Requisiti:
1. Avere PHP7
2. Avere HTTPS Attivo
3. Avere un WebServer

## Installazione:
_Ora procediamo all'installazione di EasyTG! La guida deve essere seguita passo passo._ 
* Creare una cartella ed inserire i file di EasyTG (La cartella deve essere accessibile dal web.)
* Avviare [questo](https://t.me/EasyTGBot) bot e cliccare su "Genera Key"
* Salvare momentaneamente la key in un file.
* Aprire il file index.php nella cartella di EasyTG e modificare la stringa "FPAM" con la key ricevuta dal bot.

## Settare il webhook:
**_A cosa serve il webhook?_**
_Il webhook serve a telegram per comunicarci tutti gli update che il bot deve ricevere_
**_Per settare il webhook dobbiamo fare una richiesta alle HTTP API di telegram_**

* {TOKEN} = Token del nostro bot
* {Dominio} = Potrebbe essere anche mattiabl.it
* {Directory} = directory che conduce alla index.php 
* {KEY} = Key data dal bot che abbiamo salvato in precendeza

https://api.telegram.org/bot{TOKEN}/setwebhook?url=https://{DOMAIN}/{DIRECTORY}?fpam={KEY}%26token={TOKEN}
