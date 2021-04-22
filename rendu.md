# Projet Infra/Si

## Installation

### Step 1: GNS3


- En premier installer GNS3
- Télécharger ISO GNS3 VM pour VirtualBox
- Créer une VM en important l’ISO télécharger 
- Sur GNS3 Cliquer sur “Edit” ensuite “**Preferences**” puis “**GNS3 VM**”
- Ensuite dans “**virtualization engine**” sélectionner VirtualBox puis dans “**VM Name**” choisir la VM créée auparavant  et enfin appuyer sur “**OK**”

- Télécharger image du routeur (cisco c 3640) sur https://drive.google.com/drive/folders/102jxZ9ECpe6ZFtXYdK_81iEVuuFoGOGR

- Cliquer sur “New Template” et  “Manually create a template”

- Aller sur Dynamips => IOS router

- Cliquer sur New et Run this IOS router on my local computer puis finir l’installation de l’image en sélectionnant l’image déja existante et en suivant les consignes d’installation

### Step 2: Windows Server

- Télécharger windows server 

- Dans “**Tableau de bord**” cliquer sur “**Rôles des serveurs**” puis cocher les cases “**Services AD DS**” et “**Serveur DNS**”

- Dans “**DNS**” choisir un type de zone principal dans l’assistant nouvelle zone
- Ensuite choisir de répliquer vos données DNS dans votre domaine créer 
- Cocher la zone de recherche inversé IPV4 
  puis choisir l’ID du réseau
 
- Enfin n’autoriser que les mises à jour dynamiques sécurisées 

- Ensuite aller dans “**AD DS**” puis dans “**configuration de déploiement**” pour y ajouter “**une nouvelle forêt**” et choisir le nom du domaine racine

- Maintenant dans “**option du contrôleur de domaine**” cocher les cases “**Serveur DNS**” et “**Catalogue global**” et pour le niveau fonctionnel de la nouvelle forêt et domaine racine choisir “**Windows server 2016**” puis Le mot de passe du DSRM

- Passer les étapes 

- Créer un utilisateur sur windows server dans “**Utilisateurs et ordinateurs Active Directory**” puis dans votre domaine local aller dans “**Users**” et faire un nouvel objet en lui donnant le nom désiré ainsi que son nom d’ouverture de session 
- Ensuite choisir votre mot de passe et cocher les cases "**l'utilisateur ne peut pas changer de mot de passe**" et "**le mot de passe n'expire jamais**"



### Step 3: 
