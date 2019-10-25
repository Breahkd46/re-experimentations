# Alfred - Majordome de Batman

L’idée est de créer un système qui viendra rendre les services suivants :

- Affichage d’un indicateur de santé de la maison. Cet indicateur doit être capable de combiner les informations provenant de la mesure de plusieurs grandeurs physiques:
  - Température
  - Humidité
  - CO2
  - COV
  - Déplacement d’air (détecter un courant d’air)
  - Consommation électrique de la maison
  - Production électrique
  - Quantité d’eau chaude restante 
  - Charge de la voiture électrique (optionnel en fonction de ce qu’affiche la voiture)
  - Ratio production / consommation
  - etc.
- Affichage des indicateurs détaillés sur différents domaines (en instantané et avec des graphiques) / en le ramenant à des indicateurs intelligibles pour l’humain 
  - Qualité de l’air 
  - Consommation électrique (par rapport à une journée type de la saison ou bien en €)
  - Production électrique (par rapport à une journée type de la saison ou bien en €)
  - Voiture (en capacité de déplacement)
  - Quantité d’eau chaude (en nombre de douche ou autres)
  - Ratio production/consommation électrique
- Affichage des prévisions pour la journée / pour la semaine
  - Qualité de l’air
  - Consommation électrique prévue
  - Production d’énergie prévue
  - La voiture sera chargée pour faire votre trajet quotidien à 16h30…
  - Vous pourrez prendre une douche chaude à 8h10 demain matin …
  - Prévision du ratio production / consommation
- Affichage de conseils / alertes pour bénéficier au mieux des capacités passives de la maison
  - Ouvrir la fenêtre pendant 10 minutes
  - Ne pas faire entrer de nouveaux visiteurs
  - Limiter à 5 pendant les 2 prochaines heures le nombre de personnes présentes dans la maison
  - N’oubliez pas de fermer la fenêtre
  - Faire des signaux sonores (~ alarme environnementale)
  - ….

# Exigences du cahier des charges

Voici un accès au [tableur Google Sheets](https://bit.ly/2NaqEEY) dans lequel les exigences sont mises en valeur. 

Liste des exigences : 
1. [Afficher un indicateur](https://docs.google.com/spreadsheets/d/1QO8YWqOLj1kR1SySYSeu70GplX7kD6NAzeptP_iFG5k/edit#gid=0&range=A2)
2. [Combiner des informations](https://docs.google.com/spreadsheets/d/1QO8YWqOLj1kR1SySYSeu70GplX7kD6NAzeptP_iFG5k/edit#gid=0&range=A3)
3. [Afficher des graphiques](https://docs.google.com/spreadsheets/d/1QO8YWqOLj1kR1SySYSeu70GplX7kD6NAzeptP_iFG5k/edit#gid=0&range=A4)
4. [Faire des ratios](https://docs.google.com/spreadsheets/d/1QO8YWqOLj1kR1SySYSeu70GplX7kD6NAzeptP_iFG5k/edit#gid=0&range=A5)
5. [Comparer des données](https://docs.google.com/spreadsheets/d/1QO8YWqOLj1kR1SySYSeu70GplX7kD6NAzeptP_iFG5k/edit#gid=0&range=A6)
6. [Insérer des données types](https://docs.google.com/spreadsheets/d/1QO8YWqOLj1kR1SySYSeu70GplX7kD6NAzeptP_iFG5k/edit#gid=0&range=A7)
7. [Mesure](https://docs.google.com/spreadsheets/d/1QO8YWqOLj1kR1SySYSeu70GplX7kD6NAzeptP_iFG5k/edit#gid=0&range=A8)
8. [Mesurer la température](https://docs.google.com/spreadsheets/d/1QO8YWqOLj1kR1SySYSeu70GplX7kD6NAzeptP_iFG5k/edit#gid=0&range=A9)
9.  [Mesurer le taux d'humidité](https://docs.google.com/spreadsheets/d/1QO8YWqOLj1kR1SySYSeu70GplX7kD6NAzeptP_iFG5k/edit#gid=0&range=A10)
10. [Mesurer le taux de CO2](https://docs.google.com/spreadsheets/d/1QO8YWqOLj1kR1SySYSeu70GplX7kD6NAzeptP_iFG5k/edit#gid=0&range=A11)
11. [Mesurer le taux de COV](https://docs.google.com/spreadsheets/d/1QO8YWqOLj1kR1SySYSeu70GplX7kD6NAzeptP_iFG5k/edit#gid=0&range=A12)
12. [Détecter un courant d'air](https://docs.google.com/spreadsheets/d/1QO8YWqOLj1kR1SySYSeu70GplX7kD6NAzeptP_iFG5k/edit#gid=0&range=A13)
13. [Mesurer la consommation électrique de la maison](https://docs.google.com/spreadsheets/d/1QO8YWqOLj1kR1SySYSeu70GplX7kD6NAzeptP_iFG5k/edit#gid=0&range=A14)
14. [Mesurer la production électrique](https://docs.google.com/spreadsheets/d/1QO8YWqOLj1kR1SySYSeu70GplX7kD6NAzeptP_iFG5k/edit#gid=0&range=A15)
15. [Mesurer la quantité d'eau chaude restante](https://docs.google.com/spreadsheets/d/1QO8YWqOLj1kR1SySYSeu70GplX7kD6NAzeptP_iFG5k/edit#gid=0&range=A16)
16. [Mesurer la charge de la voiture électrique](https://docs.google.com/spreadsheets/d/1QO8YWqOLj1kR1SySYSeu70GplX7kD6NAzeptP_iFG5k/edit#gid=0&range=A17)
17. [Créer des prévisions](https://docs.google.com/spreadsheets/d/1QO8YWqOLj1kR1SySYSeu70GplX7kD6NAzeptP_iFG5k/edit#gid=0&range=A18)
18. [Créer des prévisions journalières](https://docs.google.com/spreadsheets/d/1QO8YWqOLj1kR1SySYSeu70GplX7kD6NAzeptP_iFG5k/edit#gid=0&range=A19)
19. [Créer des prévisions hebdomadaires](https://docs.google.com/spreadsheets/d/1QO8YWqOLj1kR1SySYSeu70GplX7kD6NAzeptP_iFG5k/edit#gid=0&range=A20)
20. [Alertes](https://docs.google.com/spreadsheets/d/1QO8YWqOLj1kR1SySYSeu70GplX7kD6NAzeptP_iFG5k/edit#gid=0&range=A21)
21. [Alertes vocales](https://docs.google.com/spreadsheets/d/1QO8YWqOLj1kR1SySYSeu70GplX7kD6NAzeptP_iFG5k/edit#gid=0&range=A22)
22. [Alertes visuelles](https://docs.google.com/spreadsheets/d/1QO8YWqOLj1kR1SySYSeu70GplX7kD6NAzeptP_iFG5k/edit#gid=0&range=A23)
23. [Système de verrouillage automatique](https://docs.google.com/spreadsheets/d/1QO8YWqOLj1kR1SySYSeu70GplX7kD6NAzeptP_iFG5k/edit#gid=0&range=A24)
24. [Verrouillage en fonction de l'environnement](https://docs.google.com/spreadsheets/d/1QO8YWqOLj1kR1SySYSeu70GplX7kD6NAzeptP_iFG5k/edit#gid=0&range=A25)
25. [Verrouillage par configuration manuelle](https://docs.google.com/spreadsheets/d/1QO8YWqOLj1kR1SySYSeu70GplX7kD6NAzeptP_iFG5k/edit#gid=0&range=A26)