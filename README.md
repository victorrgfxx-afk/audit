# Audit Instagram & TikTok — S&V Agency

Formularul prin care un client cere auditul conturilor lui de Instagram și TikTok.
E o singură pagină statică (`index.html`), găzduită pe GitHub Pages.

## Ce se întâmplă cu răspunsurile

1. Clientul completează formularul și, opțional, pune capturi din statisticile lui.
   Capturile se micșorează în telefonul lui înainte de trimitere.
2. Răspunsurile ajung în aplicația agenției de pe Vercel (`/api/audit`), care le
   ține doar temporar.
3. De acolo sunt urcate în Google Drive, în folderul `SV-Agency / Audituri Instagram & TikTok`,
   câte un folder pe client: documentul de audit (cu răspunsurile lui deja puse în
   șablon) și capturile.
4. După ce au ajuns în Drive, copia temporară se șterge.

În pagina asta nu există nicio parolă sau cheie — doar adresa publică la care se trimite.

## De schimbat

- adresa la care se trimite: constanta `ADRESA` din `index.html`
- întrebările și variantele: obiectul `ALEGERI` din `index.html`
