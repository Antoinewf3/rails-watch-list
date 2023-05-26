Début
    Tant que l'utilisateur n'a pas choisi de quitter
        Afficher "1. Voir toutes les listes de films"
        Afficher "2. Créer une liste de films"
        Afficher "3. Voir les détails d'une liste de films"
        Afficher "4. Marquer un film dans une liste de films"
        Afficher "0. Quitter"
        Lire choixUtilisateur

        Si choixUtilisateur est égal à 1
            Afficher "Voici toutes les listes de films :"
            AfficherListesFilms()

        Sinon, si choixUtilisateur est égal à 2
            Afficher "Entrez le nom de la nouvelle liste de films :"
            Lire nomListe
            CreerListeFilms(nomListe)
            Afficher "La liste de films a été créée avec succès."

        Sinon, si choixUtilisateur est égal à 3
            Afficher "Entrez le nom de la liste de films :"
            Lire nomListe
            AfficherDetailsListeFilms(nomListe)

        Sinon, si choixUtilisateur est égal à 4
            Afficher "Entrez le nom de la liste de films :"
            Lire nomListe
            Afficher "Entrez le titre du film :"
            Lire titreFilm
            MarquerFilm(nomListe, titreFilm)
            Afficher "Le film a été marqué avec succès."

        Sinon, si choixUtilisateur est égal à 5
            Afficher "Entrez le nom de la liste de films :"
            Lire nomListe
            Afficher "Entrez le titre du film :"
            Lire titreFilm
            DetruireBookmark(nomListe, titreFilm)
            Afficher "Le bookmark a été détruit avec succès."

        Sinon, si choixUtilisateur est égal à 0
            Afficher "Au revoir !"
            QuitterApplication()

        Sinon
            Afficher "Choix invalide. Veuillez réessayer."
