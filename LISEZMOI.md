# Niveau de lame : web app Bluetooth (tablette Android)

## 1. Mettre la web app sur GitHub Pages (une seule fois, environ 10 minutes)
1. Créer un compte gratuit sur https://github.com (si tu n'en as pas).
2. En haut à droite, cliquer sur **+** puis **New repository**.
   - Nom : `niveau-lame`
   - Cocher **Public**, puis cliquer sur **Create repository**.
3. Cliquer sur le lien **uploading an existing file**, puis glisser les 5 fichiers suivants :
   `index.html`, `sw.js`, `manifest.webmanifest`, `icon-192.png`, `icon-512.png`
   → cliquer sur **Commit changes**.
4. Aller dans **Settings** → **Pages** → Source : **Deploy from a branch** → Branch : **main** / **(root)** → **Save**.
5. Attendre 1 à 2 minutes. L'adresse sera : `https://TON-NOM.github.io/niveau-lame/`

## 2. Installer sur la tablette (avec Internet, une seule fois)
1. Ouvrir l'adresse dans **Chrome** (pas un autre navigateur).
2. Menu ⋮ → **Installer l'application** (ou **Ajouter à l'écran d'accueil**).
3. Ensuite, l'icône « Niveau lame » fonctionne **sans Internet** dans la cabine.

## 3. Utilisation
- Bluetooth de la tablette activé. La première fois, accepter « Appareils à proximité ».
- Appuyer sur **CONNECTER UNE MACHINE**, puis choisir **PENTE-LAME** (259D3) ou **PENTE-D5K**.
- La première connexion charge l'écran de la machine (quelques secondes). Il est ensuite gardé dans la tablette.
  Si tu changes le programme de l'ESP32, la tablette recharge l'écran toute seule.
- Les fois suivantes : **RECONNECTER PENTE-…**, ou la reconnexion se fait toute seule.
- Petit badge vert en haut à droite = Bluetooth connecté. Appuyer dessus pour changer de machine.
- Perte du Bluetooth : écran gris « PAS DE SIGNAL » et reconnexion automatique.
- La page Wi-Fi (http://192.168.4.1) fonctionne encore en secours, ainsi que la page CAN.

## 4. Mise à jour de la web app
Remplacer les fichiers dans GitHub (Add file → Upload files). La tablette prend la nouvelle version
à la prochaine ouverture avec Internet.
