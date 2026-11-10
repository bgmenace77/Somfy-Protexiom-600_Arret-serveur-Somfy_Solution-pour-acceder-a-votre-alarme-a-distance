# Tutoriel (2 solutions) pour accéder à votre alarme Somfy Protéxiom après l'arret des serveurs Somfy prévu le 31 mars 2027

## Solution n°1
- Récupérer l'adresse IP externe de votre box internet en cliquant sur le lien suivant: https://browserleaks.com/ip
- Notez le "Hostname"

Dans l'interface de gestion de votre box internet, créez une redirection des ports comme suit:
- Protocole : TCP
- Port externe : 80
- Port interne : 80
- Adresse IP de destination : L'adresse IP locale de votre centrale Somfy (ex: 192.168.X.X)
#### Attention il faut que la centrale soit sur une IP fixe!

Depuis un navigateur, saisissez le hostname, puis l'interface de la centrale Somfy va apparaitre. 

Si vous utilisez l'appication Alarme Somfy:
- Aller sur la petite roue dentée sur le premier écran de l'application ALARME SOMFY
- Cliquez sur "Connexion à distance"
- Saisir le nom d'hôte dans le champ http:// 
#### Attention, ne cochez pas l'otion "Connexion rapide"

## Solution n°2
Configurez un serveur VPN afin d'éaccéder à vos appaereils locaux à distance.
Cette solution est payante sauf si vous êtes chez Free.
Accédez à votre interface de gestion Freebox en tapant 192.168.1.254 dans votre navigateur, depuis un ordinateur connecté au WiFi de votre Freebox
Saisissez vos identifiants Freebox
Cliquez sur mode avancé en haut, puis sur l'icône "Serveur VPN".
Dans la partie "Configuration", cliquez sur "Utilisateurs", puis sur "+ Ajouter un utilisateur" 
• Login : Saissiez un nom d'utisateur
• Typed de serveur: Wireguard
IP fixe: IP dynamique
Mot de passe: Saisissez un mot de passe
Dans la partie "Configuration", cliquez sur "Wireguard"
Cocher la case "Activer", ne touchez pas aux numéros de Port et MTU.
Dans la partie "Fichiers de configuration", photographiez le QR code.
Installez Wireguard sur votre téléphone
Ouvrez Wireguard, cliquez sur le bouton "+", puis cliquez sur "Créer à partir d'un code QR"
Scannez le code QR, la configuration est faite.
Lancez le VPN, et saisissez l'adress IP de votre centrale dans le navigateur pour accéder à la cponsoel de gestion Somfy.
