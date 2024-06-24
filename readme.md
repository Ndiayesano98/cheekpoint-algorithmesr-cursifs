Fonction estAnneeBissextile(annee)
    Si (annee % 4 = 0) Alors
        Si (annee % 100 != 0) Ou (annee % 400 = 0) Alors
            Retourner Vrai
        Sinon
            Retourner Faux
    Sinon
        Retourner Faux
Fin Fonction
Fonction prixBillet(age)
    Si (age <= 12) Alors
        Retourner 10
    Sinon Si (13 <= age <= 17) Alors
        Retourner 15
    Sinon
        Retourner 20
Fin Fonction
Fonction fibonacci(n)
    Si (n <= 0) Alors
        Retourner 0
    Sinon Si (n = 1) Alors
        Retourner 1
    Sinon
        Retourner fibonacci(n - 1) + fibonacci(n - 2)
Fin Fonction
Fonction estPalindrome(chaine)
    chaine = retirerEspacesEtPonctuation(chaine)
    chaine = convertirEnMinuscules(chaine)
    
    Si (longueur(chaine) <= 1) Alors
        Retourner Vrai
    Sinon Si (chaine[0] = chaine[-1]) Alors
        Retourner estPalindrome(sousChaine(chaine, 1, longueur(chaine) - 1))
    Sinon
        Retourner Faux
Fin Fonction

Fonction retirerEspacesEtPonctuation(chaine)
    # Implémente la logique pour retirer les espaces et la ponctuation
    # Retourne la chaîne nettoyée
Fin Fonction

Fonction convertirEnMinuscules(chaine)
    # Implémente la logique pour convertir la chaîne en minuscules
    # Retourne la chaîne convertie
Fin Fonction
