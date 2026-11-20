# L'évolution des ordinateurs : rapport et présentation en LaTeX

Un rapport de 7 pages et une présentation de 10 diapositives sur l'histoire des ordinateurs, des premières machines à calculer jusqu'aux PC d'aujourd'hui.

C'est un travail de groupe (quatre étudiants) réalisé de septembre à novembre 2023 pendant le cours PPEI de L3 informatique. Le but du cours n'était pas le sujet en lui-même, mais d'apprendre à écrire des documents avec des langages de balisage : on pouvait choisir entre Markdown et LaTeX, et nous avons choisi LaTeX.

## À lire

Pas besoin d'installer quoi que ce soit pour voir le résultat :

- [`rapport.pdf`](rapport.pdf) : le rapport
- [`diapos.pdf`](diapos.pdf) : la présentation

## Contenu du rapport

1. Introduction
2. Définition (l'origine du mot « ordinateur »)
3. Les premières machines à calculer : le boulier et la Pascaline
4. Les machines à circuits électriques : le Z3 et l'ENIAC
5. Les premiers ordinateurs personnels : Apple, IBM, puis le PC actuel
6. Conclusion

La présentation suit le même plan, avec un format plus court pour un exposé oral de quelques minutes.

## Ce que nous avons utilisé

- **LaTeX** (classe `article`) pour le rapport, avec table des matières, figures et légendes
- **Beamer** (thème Madrid) pour les diapositives
- **BibTeX** pour la bibliographie (`rapport.bib`)
- **Git** pour le rendu : le travail a été remis par fork et pull request sur Codeberg

## Recompiler les documents

Il faut une installation LaTeX (TeX Live ou MiKTeX). Depuis le dossier du projet :

```
pdflatex rapport
bibtex rapport
pdflatex rapport
pdflatex rapport

pdflatex diapos
pdflatex diapos
```

Les images doivent rester dans le dossier `Images/`, à côté des fichiers `.tex`.

## Fichiers

```
├── rapport.tex  rapport.bib  rapport.pdf
├── diapos.tex   diapos.pdf
└── Images/
```

## À propos des images

Les illustrations viennent d'internet et ne sont pas de nous. Elles restent la propriété de leurs auteurs et ne sont là que pour illustrer ce travail d'étudiants.
