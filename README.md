Lancer un projet web de Vial avec IntelliJ
=====================

Ingrédients:
* Jdk instalé (retenez le dossier d'installation si vous le faite pour l'occasion)
* Tomcatre installé et configuré (c'est-à-dire avoir été lancé avec succès avec le standalone après avoir SET JAVA_HOME)
* IntelliJ Ultimate (logique vu le nom de ce tutoriel) ((Pour ceux qui n'ont pas l'ultimate, elle est gratuite en étant étudiant si vous entrez votre mail etu sur http://jetbrains.com/student))

1. Ouvrir le projet

Sélectionnez «Import Project»
![Acceuil de IntelliJ](url "texte pour le titre, facultatif")

Sélectionnez le dossier décompresser du projet eclipse

![Ecran de choix](url "texte pour le titre, facultatif")

«From external model» > Eclipse

«Next» jusqu'à arriver sur cette erreur:
![Imported project refers to unknown jdks Java SE 8](url "texte pour le titre, facultatif")

Selectionnez «Ok» puis le projet s'ouvre

2. Configurer le projet

![Projet](url "texte pour le titre, facultatif")

Après un rapide indexage du projet, une popup «Framework detected» apparait. Cliquez sur «Configure»

![Setup Frameworks](url "texte pour le titre, facultatif")

Laissez tout coché et faites «Ok»

Clicker ensuite sur l'icone de «Make» représentée par une flêche verte

![Icone Make](url "texte pour le titre, facultatif")

Une erreur sauvage apparait (en réalité la même qu'au début)

![Erreur sauvage](url "texte pour le titre, facultatif")

Il va falloir changer le jdk du projet par le votre, pour cela selectionnez le votre dans le menu déroulant
Si il s'agit de votre premier projet (shame on you !), vous devez rajouter votre jdk en faisant «New…» et sélectionnez le dossier de votre jdk (en général C:\Program Files(x86)\Java…)

![Choix jdk](url "texte pour le titre, facultatif")

3. Lancer le projet

À present il faut lancer le projet mais pour cela il va falloir créer une configuration Tomcat

![Edit configuration](url "texte pour le titre, facultatif")

Cliquez sur le menu déroulant à côté de Make et sélectionnez «Edit configuration»

![Run/Debug Configurations](url "texte pour le titre, facultatif")

Cliquez sur le + en vert > Tomcat Server (dans «Show x irrelevant item») > Local

![Tomcatre server local](url "texte pour le titre, facultatif")

Choissisez 
