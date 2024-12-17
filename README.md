Exercice pour comprendre Héritage, Polymorphisme à l'exécution et Polymorphisme à la compilation
Contexte : Gestion d'une bibliothèque de médias

Tu vas créer un programme qui gère différents types de médias (livres, films, et magazines) dans une bibliothèque. Cet exercice te permettra de pratiquer l'héritage, le polymorphisme à l'exécution (dynamique) et le polymorphisme à la compilation (statique).
Étape 1 : Création de la classe Parent (Héritage)

    Crée une classe Media avec les éléments suivants :
        Un attribut String titre pour le titre du média.
        Une méthode afficherInfos() qui affiche un message générique : "Ceci est un média intitulé : <titre>.".
        Un constructeur pour initialiser le titre du média.

Étape 2 : Création des classes Enfants (Héritage)

Crée trois classes qui héritent de la classe Media :

    Livre :
        Un attribut String auteur.
        Redéfinis la méthode afficherInfos() pour afficher les informations du livre :
        "Livre : <titre> écrit par <auteur>.".
        Ajoute un constructeur pour initialiser titre et auteur.

    Film :
        Deux attributs : String réalisateur et int duree (durée en minutes).
        Redéfinis la méthode afficherInfos() pour afficher les informations du film :
        "Film : <titre>, réalisé par <réalisateur>, durée : <duree> minutes.".
        Ajoute un constructeur pour initialiser titre, réalisateur et duree.

    Magazine :
        Un attribut int numeroEdition.
        Redéfinis la méthode afficherInfos() pour afficher les informations du magazine :
        "Magazine : <titre>, numéro d'édition : <numeroEdition>.".
        Ajoute un constructeur pour initialiser titre et numeroEdition.

Étape 3 : Polymorphisme à l'exécution (Dynamique)

    Dans une classe Bibliotheque, crée une méthode afficherMedia(Media media) qui prend un objet Media en paramètre et appelle sa méthode afficherInfos().

    Dans la méthode main :
        Crée un tableau ou une liste de médias contenant des objets Livre, Film, et Magazine.
        Parcours le tableau et utilise la méthode afficherMedia() pour afficher les informations de chaque média. Grâce au polymorphisme à l'exécution, la méthode spécifique de chaque sous-classe sera appelée.

Étape 4 : Polymorphisme à la compilation (Statique)

    Crée une classe Operations avec deux méthodes calculer surchargées pour démontrer le polymorphisme statique :
        calculer(int a, int b) : Affiche la somme des deux entiers.
        calculer(int a, int b, int c) : Affiche la somme de trois entiers.

    Dans la méthode main :
        Crée un objet de type Operations.
        Appelle les deux versions de la méthode calculer.
