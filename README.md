# Yam – Feuille de score

Feuille de score numérique pour le jeu de Yam, utilisable sur mobile et ordinateur.

**Site disponible sur : https://flake9025.github.io/yam-scores/**

---

## Fonctionnalités

- 2 joueurs avec noms personnalisables
- Jeu en tour par tour : la colonne du joueur inactif est verrouillée
- Confirmation du score via une pop-up avant de valider son tour
- Calcul automatique des scores en temps réel, indicateur visuel du joueur en tête
- Lanceur de dés intégré (3 lancers par tour, choix des dés à garder)
- Icônes de dés SVG pour chaque combinaison
- Écran de fin de partie avec résultat et bouton "Nouvelle partie"
- Installable en raccourci sur iOS et Android (PWA)

---

## Comment jouer

### Déroulement d'un tour

1. C'est à toi de jouer — ton nom est affiché en haut avec la couleur de ta colonne.
2. **Lance les dés** en appuyant sur 🎲 (en haut à gauche). Tu as droit à **3 lancers** :
   - Le premier lancer est automatique à l'ouverture.
   - Après chaque lancer, **touche les dés que tu veux garder** (ils se surligent en vert).
   - Appuie sur **Relancer** pour relancer les dés non gardés.
   - Au 3e lancer, les dés sont définitifs.
3. **Choisis une case** dans ta colonne correspondant à ta combinaison.
4. Une **pop-up de confirmation** s'affiche — appuie sur **Valider** pour enregistrer le score et passer la main, ou **Changer** pour essayer une autre case.
5. L'autre joueur joue à son tour.

La partie se termine quand toutes les cases des deux joueurs sont remplies (12 cases chacun, 24 au total).

---

## Règles du Yam

### Matériel

- 5 dés classiques à 6 faces
- La feuille de score (cette application !)

### Partie supérieure — les nombres

À chaque tour, le joueur peut inscrire le total des dés d'une même valeur dans la case correspondante.

| Catégorie    | Score                    | Exemple (5 dés)      |
|--------------|--------------------------|----------------------|
| Nombre de 1  | 1 pt par dé montrant 1   | 1-1-1-3-5 → 3 pts    |
| Nombre de 2  | 2 pts par dé montrant 2  | 2-2-4-5-6 → 4 pts    |
| Nombre de 3  | 3 pts par dé montrant 3  | 3-3-3-3-1 → 12 pts   |
| Nombre de 4  | 4 pts par dé montrant 4  | 4-4-2-3-6 → 8 pts    |
| Nombre de 5  | 5 pts par dé montrant 5  | 5-5-5-5-5 → 25 pts   |
| Nombre de 6  | 6 pts par dé montrant 6  | 6-6-1-2-3 → 12 pts   |

Si le **total de la partie supérieure atteint 63 pts ou plus**, une **prime de +37 pts** est automatiquement ajoutée au total partiel.

### Combinaisons

| Combinaison  | Score   | Condition                        | Exemple              |
|--------------|---------|----------------------------------|----------------------|
| Brelan       | 5–30 pts | Somme des 5 dés si 3 identiques  | 4-4-4-1-2 → 15 pts   |
| Petite suite | 25 pts  | Les 5 dés forment 1-2-3-4-5      | 1-2-3-4-5            |
| Grande suite | 25 pts  | Les 5 dés forment 2-3-4-5-6      | 2-3-4-5-6            |
| Full         | 30 pts  | Un brelan + une paire            | 3-3-3-6-6            |
| Carré        | 40 pts  | Au moins 4 dés identiques        | 2-2-2-2-5            |
| Yam !        | 50 pts  | Les 5 dés sont identiques        | 6-6-6-6-6            |

### Fin de partie et décompte

Une fois toutes les cases remplies :
- Le **total partiel** est la somme des 6 cases de la partie supérieure.
- Le **total combinaisons** est la somme des 6 combinaisons.
- Le **total général** = total partiel + total combinaisons.

Le joueur avec le **total général le plus élevé** remporte la partie.

---

## Installation (PWA)

**Android (Chrome)** : menu ⋮ → *Ajouter à l'écran d'accueil*

**iOS (Safari)** : bouton partage ↑ → *Sur l'écran d'accueil*

L'application fonctionne entièrement hors-ligne une fois installée.
