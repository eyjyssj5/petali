# Petali - gioco m'ama, non m'ama

15 fiori, ciascuno con il suo significato. Scegli un fiore, togli i petali uno alla volta
e scopri il risultato, con il messaggio del fiore.

## Prova nel browser

Apri `www/index.html` con il browser. Tutto funziona senza installare niente.

## Test automatici

    npm test

## APK Android

Serve Node.js (versione LTS) e Android Studio, come per il progetto precedente.

1. Nella cartella del progetto:

       npm install
       npx cap add android
       npx cap sync android
       npx cap open android

2. In Android Studio, aspetta la fine di Gradle, poi scegli
   **Build > Build APK(s)**.
3. Il file si trova in `android/app/build/outputs/apk/debug/app-debug.apk`.

Dopo ogni modifica a `www/`, esegui di nuovo `npx cap sync android`.

## Dove modificare

- `www/fiori.js`: nomi, colori, significati e messaggi dei 15 fiori.
- `www/styles.css`: colori e grafica.
- `www/app.js`: come vengono disegnati i fiori e come si svolge il gioco.

## Nota

I significati dei fiori sono quelli della tradizione del linguaggio dei fiori. Il gioco è un passatempo, non una previsione.
