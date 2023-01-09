# WasmRP-Documentation

1. Accès à l'Application

Pour accéder à l'application, cliquez sur le lien suivant : <span style="font-weight:bolder;">https://blazorwasmrp.pages.dev</span>

2. Sauvegarde / Chargement des Données

L'application fonctionne avec comme volume de donnée, un fichier JSON généré par l'application. Ce fichier a pour nom une succession d'informations comme ceci : Sauvegarde_Blai_24_06_2022 15_49_45.

Etant donné que fichier de sauvegarde a été téléchargé, il est possible de le modifier afin de faire correspondre des modificiations entre deux séances.

❌ <span style="color: red; font-weight: bolder;">**Attention**</span> ❌

Vous pouvez certes modifier les données de votre personnnage mais il est recommandé d'effectuer les modifcations via l'application afin d'éviter les possibles perturbations du fichier et ainsi ne plus pouvoir charger votre personnage.


3. Modules

Dans l'application, il y a plusieurs sous-parties que j'appellerai les modules qui sont au nombre de 7.

- L'Affichage Général (Sidebar de Gauche) : 

![image](https://user-images.githubusercontent.com/58788952/176604492-442bbb79-4828-42bf-8888-03be592491d3.png)

Ce module permet d'avoir les statistiques générales du personnage affichées en permancance, de permettre la naviagation vers les différents modules restants, d'appliquer sur l'application le theme sombre ou encore de charger et sauvegarder toutes les données de votre personnage dans un fichier.

- L'Acceuil (Hub) : 

![image](hubGeneral.png)

Ce module permet la modification des caractéristiques principales de votre personnage.

- L'Inventaire : 

![image](https://user-images.githubusercontent.com/58788952/176604898-a8223124-e7e9-4ec6-b11d-f70d91ef3693.png)

Ce module permet la modification de l'inventaire de votre personnage ainsi que toutes les caractéristiques des items contenus dans cet inventaire.

- Les Compétences : 

![image](https://user-images.githubusercontent.com/58788952/176605000-b7ab100f-0bf6-44b8-9ee0-d7ce67cf2a7f.png)

Ce module permet de manager les compétences de votre personnage ainsi que de les utiliser (consommation de ressource définie à savoir aucune ressource, pv uniquement, pm uniquement, pv et pm)

- Les Familiers : 

![image](https://user-images.githubusercontent.com/58788952/176605099-121c9a51-d282-41a6-b495-93de9ffe2bbb.png)

Module à implémenter quand nous aurons une idée claire du systeme

- Les Affinités : 

![image](https://user-images.githubusercontent.com/58788952/176605157-494f58fc-abc3-4ff7-b9d1-6c8226fbc7f5.png)

Ce module est un affichage plus sympa de l'avancée de vos affinités

- Le Calcul de dégats : 

Ce module est fonctionnel mais il manque encore de quelques travaux pour qu'il puisse etre modulable et propre à chacun

4. Fonctionnalités des Modules

Cette partie est réservée à l'utilisation de chacun des modules. Nous allons donc réutiliser l'ordre de présentation pour ne pas vous perdre.

- L'Affichage Général (Sidebar de Gauche) : 
    *   Charger / Sauvegarder ses données :
            Cette action nécéssite deux clics, le premier sur le bouton "Charger / Sauvegarder" qui débloquera les deux options suivantes :
            
           ![image](https://user-images.githubusercontent.com/58788952/176605374-61a582d5-3491-499c-b806-d95441d74074.png)
            
           ![image](https://user-images.githubusercontent.com/58788952/176605487-c3cc10be-71c5-4063-8801-2b4a50dd1174.png)

           🛑 **De plus, vous pouvez sauvegarder votre personnage depuis la vision de n'importe quel module, par contre, le chargement de votre personnage n'est permis que lorsque vous avez la vision sur le Hub.** 🛑
    *   Se déplacer dans les différents modules :
        
        ![image](genDisplayLiens.png)

        Il suffit de cliquer sur l'un de ces boutons. Passer votre souris dessus vous indiquera vers quel module il vous emmenera.
    
    *   Appliquer le Dark Mode :

        ![image](genDisplayDM.png)

        Cliquer sur le bouton activera ou désactivera le Dark Mode.
    * Reset le Compteur de Tour :

        ![image](genDisplayCompteurTours.png)

        Il faut double-cliquer sur le texte pour reset le compteur.

- L'Acceuil (Hub) : 

    *   Il n'est plus possible de modifier l'armure physique et l'armure magique car ces dernières sont maintenant calculées automatiquement en fonction de l'armure portée par votre personnage.

    *   Il n'est plus possible de modifier la quantité de piece d'or, de piece d'argent et de piece de cuivre de façon générale puisque cette fonctionnalité a été déplacée aux containers (espace d'inventaire permettant le stockage d'item)

    *   Lorsque des items de type Accessoire ou Armure sont équipés, ils apparaissent dans l'emplacement **Equipement** de la manière suivante : 

    ![image](hubGear.png)

    *   Lorsque des items de type Arme, Arme de Jet, Chargeur, Consommable sont équipés, ils apparaissent dans l'emplacement **Inventaire Rapide** de la manière suivante : 

    ![image](hubFastInv.png)

    * Ces emplacements servent généralement d'affichage de certaines caractériques et permettent parfois, selon le type d'item, d'effectuer une action particuliere telle que modifier l'emplacement d'un item, consommer une potion ou bien tirer un projectile. 
    
    Sinon toutes les autres caractéristiques sont modifiables et répercutées dans l'Affichage Général.


- L'Inventaire : 
    *   Il est possible de créer des containers avec un nom et une capacité modifiés.
    *   Il est possible de supprimer les containers en les sélectionnant au préalable.
    *   Il est possible de créer jusque 5 containers maximum.
    *   Le container nommé Inventaire Personnage est permanent. Il ne peut etre supprimé.
    *   Pour sélectionner un container, il suffit de cliquer sur son emplacement. Une fois sélectionné, le fond de l'emplacement passe en couleur orange.
    *   Pour ouvrir un container et voir ce qu'il contient, double-cliquez sur l'emplacement du container.
    *   
- Les Compétences : Ce module permet de manager les compétences de votre personnage ainsi que de les utiliser (consommation de ressource définie à savoir aucune ressource, pv uniquement, pm uniquement, pv et pm)
- Les Familiers : Module à implémenter quand nous aurons une idée claire du systeme
- Les Affinités : Ce module est un affichage plus sympa de l'avancée de vos affinités
- Le Calcul de dégats : Ce module est fonctionnel mais il manque encore de quelques travaux pour qu'il puisse etre modulable et propre à chacun



<span style="color: blue">TEST COULEUR</span>

