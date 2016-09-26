Importer un projet web JEE avec IntelliJ
=====================

Ingrédients :
* JDK installé (retenez le dossier d'installation si vous le faites pour l'occasion)
* Tomcatre installé et configuré (c'est-à-dire avoir été lancé avec succès avec le standalone après avoir SET JAVA_HOME)
* IntelliJ Ultimate (logique vu le nom de ce tutoriel) ((Pour ceux qui n'ont pas l'ultimate, elle est gratuite en étant étudiant si vous entrez votre mail etu sur http://jetbrains.com/student))

Préparations :
* Moins de 5 minutes (sauf avec eduram)

Ouvrir le projet
----------------

1. Sélectionnez «Import Project»
![Accueil de IntelliJ](https://github.com/J0hn-/Polytech-Tuto-IntelliJ/raw/master/Screenshots/1.png)

2. Sélectionnez le dossier décompressé du projet eclipse
![Ecran de choix](https://github.com/J0hn-/Polytech-Tuto-IntelliJ/raw/master/Screenshots/2.png)

3. «From external model» > Eclipse
«Next» jusqu'à arriver sur cette erreur:
![Imported project refers to unknown jdks Java SE 8](https://github.com/J0hn-/Polytech-Tuto-IntelliJ/raw/master/Screenshots/3.png)

4. Sélectionnez «Ok» puis le projet s'ouvre

Configurer le projet
--------------------

![Projet](https://github.com/J0hn-/Polytech-Tuto-IntelliJ/raw/master/Screenshots/4.png)

Après un rapide indexage du projet, une pop-up «Framework detected» apparait.

1. Cliquez sur «Configure»
![Setup Frameworks](https://github.com/J0hn-/Polytech-Tuto-IntelliJ/raw/master/Screenshots/5.png)

2. Laissez tout coché et faites «Ok»

3. Cliquez ensuite sur l'icône de «Make» représentée par une flèche verte
![Icone Make](https://github.com/J0hn-/Polytech-Tuto-IntelliJ/raw/master/Screenshots/6.png)

4. Une erreur sauvage apparait (en réalité la même qu'au début)
![Erreur sauvage](https://github.com/J0hn-/Polytech-Tuto-IntelliJ/raw/master/Screenshots/7.png)

Il va falloir changer le JDK du projet par le vôtre, pour cela sélectionnez le vôtre dans le menu déroulant
Si il s'agit de votre premier projet (shame on you !), vous devez rajouter votre JDK en faisant «New…» et sélectionnez le dossier de votre jdk (en général C:\Program Files(x86)\Java…)

![Choix jdk](https://github.com/J0hn-/Polytech-Tuto-IntelliJ/raw/master/Screenshots/8.png)

Lancer le projet
----------------

À présent il faut lancer le projet mais pour cela il va falloir créer une configuration Tomcat

1. Cliquez sur le menu déroulant à côté de Make et sélectionnez «Edit configuration»
![Edit configuration](https://github.com/J0hn-/Polytech-Tuto-IntelliJ/raw/master/Screenshots/9.png)

2. Cliquez sur le + en vert > Tomcat Server (dans «Show x irrelevant item») > Local
![Run/Debug Configurations](https://github.com/J0hn-/Polytech-Tuto-IntelliJ/raw/master/Screenshots/10.png)

3. Choisissez votre Tomcat dans le menu déroulant ou si il s'agit de la première fois, Cliquez sur «Configure…» pour choisir l'emplacement du dossier Tomcat
![Tomcatre server local](https://github.com/J0hn-/Polytech-Tuto-IntelliJ/raw/master/Screenshots/11.png)

4. Une fois choisi, sélectionnez «Fix» afin de créer un artifact

5. Cliquez sur le + vert > Web Application Exploded > From modules
![Project Structure](https://github.com/J0hn-/Polytech-Tuto-IntelliJ/raw/master/Screenshots/12.png)

6. Choisissez votre module
![Select Modules](https://github.com/J0hn-/Polytech-Tuto-IntelliJ/raw/master/Screenshots/13.png)

7. Faites des «Ok» jusqu'à arriver sur la page du projet

Servir le projet
----------------

![Tomcatre server local](https://github.com/J0hn-/Polytech-Tuto-IntelliJ/raw/master/Screenshots/over 9000.png)

Il n'y a plus qu'à lancer avec l'autre flèche verte apparût par magie, après quelques secondes votre navigateur s'ouvre sur http://localhost:8080/ et la magie vous submerge… C'est prêt !
