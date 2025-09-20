The Duke's — Landing (Splash) + Menu PDF
=========================================

Contenu du dossier :
- index.html   → page d'accueil (logo + redirection automatique)
- logo.png     → logo affiché en grand
- menu.pdf     → votre carte (PDF) ouverte après 2,5 s

Hébergement (3 options simples) :
1) Netlify Drop (le plus simple)
   - Ouvrez https://app.netlify.com/drop
   - Glissez le dossier 'dukes-landing' sur la page
   - Netlify vous donne une URL publique (ex. https://votre-site.netlify.app)

2) GitHub Pages
   - Créez un dépôt vide, uploadez index.html, logo.png, menu.pdf
   - Dans Settings → Pages, sélectionnez 'Branch: main' et 'root'
   - L’URL publique est générée en quelques secondes

3) Votre hébergeur / FTP
   - Uploadez le dossier tel quel sur votre hébergement
   - L’URL publique sera similaire à https://votredomaine/dukes-landing/

Générer un QR code :
- Utilisez l’URL publique de la page index.html (pas celle du PDF).
- Exportez le QR en PNG 300 dpi ou en SVG pour l’impression grand format.

Astuces :
- Pour changer le délai, modifiez DELAY_MS dans index.html (ex. 1500 pour 1,5 s).
- Pour un fond différent, remplacez la variable CSS --dukes dans <style>.
- Pour afficher un bouton seulement (sans redirection auto), supprimez le script dans <head>.
