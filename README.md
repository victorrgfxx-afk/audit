# Audit Instagram & TikTok — S&V Agency

Formularul prin care un client cere auditul conturilor lui de Instagram și TikTok.
E o singură pagină statică (`index.html`), găzduită pe GitHub Pages.

## Ce se întâmplă cu răspunsurile

1. Clientul alege platforma (Instagram sau TikTok) și încarcă doar capturi de ecran:
   profilul (1-3), ultimele 10 postări, cele mai bune 3-5 și cele mai slabe 3-4.
   De scris are doar numele și emailul. Capturile se micșorează în telefonul lui
   și urcă una câte una, cu bară de progres.
2. Răspunsurile ajung în aplicația agenției de pe Vercel (`/api/audit`), care le
   ține doar temporar.
3. De acolo sunt urcate în Google Drive, în folderul `SV-Agency / Audituri Instagram & TikTok`,
   câte un folder pe client: documentul de audit (cu răspunsurile lui deja puse în
   șablon) și capturile.
4. După ce au ajuns în Drive, copia temporară se șterge.

În pagina asta nu există nicio parolă sau cheie — doar adresa publică la care se trimite.

## De schimbat

- adresa la care se trimite: constanta `ADRESA` din `index.html`
- câte capturi pe grup: `GRUPURI` din `index.html` (și aceleași limite în `api/audit.js` din aplicație)
- textele cu instrucțiuni pe platformă: `TEXTE` din `index.html`
