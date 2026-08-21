# Emiasd - Monte Carlo Search

Ce dépôt regroupe mon travail pour le cours **Monte Carlo Search** du **Master Exécutif EMIASD (Intelligence Artificielle et Sciences des Données) de l'Université Paris-Dauphine**.

Le cours couvre les méthodes de recherche par Monte Carlo appliquées à la prise de décision séquentielle et aux jeux : recherche à plat (Flat Monte Carlo), UCB/bandits, MCTS, RAVE/AMAF, Nested Monte Carlo Search (NRPA) et les approches "Zero Learning" (type AlphaZero).

## Contenu

- **`1.Cours/`** — Notes de cours au format Markdown, organisées par notion :
  - `1.move_class_reference.md`, `2.board_class_reference.md` : structures de base (coup, plateau) utilisées dans les TP, illustrées sur le jeu **Breakthrough**.
  - `3.flat_monte_carlo_reference.md`, `4.ucb_algorithm_reference.md` : recherche à plat et algorithme UCB (bandits multi-bras).
  - `5.board_hash_comparison.md` : comparaison de méthodes de hachage de plateau.
  - `6.rave_algorithm_reference.md`, `7.amaf_complete_explanation.md`, `8.rave_mathematical_analysis.md` : RAVE et AMAF (accélération de l'apprentissage par partage de statistiques).
  - `MonteCarlo.pdf` : support de cours principal.

- **`2.TP & Notebooks/`** — Notebooks Jupyter des travaux pratiques :
  - `Breakthrough.ipynb` : implémentation Monte Carlo Search sur le jeu Breakthrough.
  - `Nested-LeftMove.ipynb`, `NRPA-LeftMove.ipynb` : Nested Monte Carlo Search et Nested Rollout Policy Adaptation sur le problème "LeftMove".
  - `ExpressionDiscovery.ipynb` : découverte d'expressions par recherche Monte Carlo.
  - `Humanoid.ipynb`, `LunarLander.ipynb`, `LunarLanderv2.ipynb` : application à des environnements de contrôle continu (type Gym/OpenAI).
  - `generate/`, `generate.zip` : jeux de données générés utilisés par les notebooks.

- **`3.Articles/`** — Articles de recherche de référence, classés par thème :
  - `Monte Carlo Tree Search/` : survey MCTS, GRAVE, MCTS-Gelly-Silver, SHUSS...
  - `Nested Monte Carlo Search/` : articles fondateurs du Nested Monte Carlo Search.
  - `Playout Policy Adaptation/` : NRPA et PPA.
  - `Zero Learning/` : approches type AlphaZero/Polygames (apprentissage sans connaissance experte).

## Utilisation

Les notebooks (`2.TP & Notebooks/*.ipynb`) s'ouvrent avec Jupyter :

```bash
jupyter notebook "2.TP & Notebooks"
```

Les notes de cours (`1.Cours/*.md`) sont consultables directement en Markdown et servent de référence théorique aux implémentations des notebooks.
