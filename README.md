Je vous propose 2 solutions afin d'accéder à votre alarme Somfy Protéxiom après l'arret des serveurs Somfy prévu le 31 mars 2027:

Solution n°1
Récupérer l'adresse IP externe de votre box internet en cliquant sur le lien suivant, puis notez le "Hostname".
https://browserleaks.com/ip
Dans votre box, créez une une redirection des ports comme suit:
• Protocole : TCP
• Port externe : 80
• Port interne : 80
• Adresse IP de destination : L'adresse IP locale de votre centrale Somfy (ex: 192.168.X.X)
- Attention il faut que la centrale soit sur IP fixe -

Depuis un navigateur, saisissez le host name, vous attérirez directement sur l'interface de votre centrale Somfy.
Si vous utilisez l'appication Alarme Somfy, aller sur le petite roue dentée sur le premier écran de l'application ALARME SOMFY puis > 2 Connexion à distance , saisir le nom d'hôte dans le champ http:// 
- Attention ne cochez pas l'otion Connexion rapide -

Solution n°2
Configurez un serveur VPN afin d'éaccéder à vos appaereils locaux à distance.
Cette solution est payante sauf si vous êtes chez Free.
Accédez à votre interface de gestion Freebox en tapant 192.168.1.254 dans votre navigateur, depuis un ordinateur connecté au WiFi de votre Freebox
Saisissez vos identifiants Freebox
Cliquez sur mode avancé en haut, puis sur l'icône "Serveur VPN".
Dans la partie configuration, cliquez sur "Utilisateurs", puis sur "+ Ajouter un utilisateur" 
• Login : Saissiez un nom d'utisateur
• Typed de serveur: Wireguard
IP fixe: IP dynamique
Mot de passe: Saisissez un mot de passe
