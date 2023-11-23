# angelo.magalhaes_ex3
objectif: afficher hello world


![image](https://github.com/Lo0kii/angelo.magalhaes_ex3/assets/109228312/bcda9037-9faf-455b-8756-ad86d8e3ac11)



pour commencer, comme dhab crée un dossier , avec un main.tf et terraform.exe a l'interrieure, sur vs code ouvrir le dossier et le fichier main.tf
tips, dans la console iam dans aws oublier pas de mettre les droits necessaire a l'utilisateur 


proceder: 
1. Configuration Terraform pour l'Instance EC2 :
 déploie une instance EC2 sur AWS dans la région "eu-west-3" en utilisant les clés d'accès (access_key et secret_key) spécifiées
provider "aws" : Définit le fournisseur AWS et spécifie la région ainsi que les clés d'accès pour l'authentification.

resource "aws_instance" "geto_est_mort" : Déclare une ressource AWS de type instance EC2 avec le nom "geto_est_mort". Cette instance utilise une image AMI spécifiée (Ubuntu), un type d'instance t2.micro, et est associée à un groupe de sécurité nommé "HK_web". Le script de données utilisateur (user_data) exécute des commandes de configuration pour installer et démarrer Apache, puis crée une page HTML avec un message spécifique.

resource "aws_security_group" "HK_web" : Déclare un groupe de sécurité qui autorise le trafic HTTP (port 80) et le trafic SSH (port 22). Il porte le nom "HK-web". De plus, il spécifie une règle de trafic sortant permettant toutes les sorties.

en bonus Le message dans la page HTML indique que "Geto SUGURU est mort avec la tête tranchée par Yuta, bonne soirée."




 ![image](https://github.com/Lo0kii/angelo.magalhaes_ex3/assets/109228312/eaee8f47-8f2a-4015-9791-e3e9605f6fa2)



pour celui la j'ai eu des galere pour la page html, et trouver des information dessus sur internet c'etait long, la partie pour donner les droit a l'utilisateur, jai pas trouver la solution tout seul on m'a aider.
