# CoopHabitat — Gestion numérique d'une coopérative d'habitat

Projet réalisé dans le cadre du module **Gestion de Projet Informatique Avancée** (Projet 5 / 14) par le **Groupe 11**.

## Présentation

Les coopératives d'habitat sont un mécanisme répandu au Sénégal pour permettre aux fonctionnaires et aux travailleurs du secteur formel d'accéder au logement. Leur gestion repose encore souvent sur des assemblées physiques, des carnets d'épargne papier et des trésoriers surchargés. Les membres n'ont donc aucune visibilité sur leurs cotisations ni sur l'avancement du projet, ce qui alimente les litiges sur les attributions de lots et la gestion des fonds.

**CoopHabitat** est une plateforme transparente qui permet de :

- digitaliser les cotisations et automatiser les rappels ;
- gérer les attributions de lots avec un workflow auditable ;
- publier les comptes de la coopérative à tous les membres.

## Fonctionnalités

- **Gestion des membres** : inscription, numéro d'adhérent, type de membre (fondateur, ordinaire, bénéficiaire), statut actif ou suspendu
- **Plan de cotisation** : montant mensuel, date d'échéance, pénalités de retard configurables
- **Suivi des paiements** : saisie manuelle ou Mobile Money (Wave / SendFlash en sandbox), reçu PDF automatique, solde cumulé par membre
- **Gestion des lots** : terrains et logements (superficie, localisation GPS, statut disponible / attribué / litigieux)
- **Workflow d'attribution** : tirage au sort ou commission, PV d'attribution en PDF, notification des membres
- **Espace comptable** : budget prévisionnel, dépenses réelles, trésorerie disponible, rapport financier exportable en PDF et Excel
- **Assemblée générale numérique** : convocations, ordre du jour, délibérations, comptes rendus publiés
- **Rôles** : Président, Trésorier, Secrétaire, Membre
- **Rappels automatiques** par SMS ou e-mail 3 jours avant l'échéance

## Stack technique

| Couche | Technologie |
|---|---|
| Back-end | Spring Boot |
| Front-end | Angular (mobile-first, mode offline partiel via Service Worker) |
| Base de données | PostgreSQL |
| Rapports | Jasper Reports |
| Sécurité | Authentification JWT avec gestion des rôles |
| Documentation API | Swagger / OpenAPI 3.0 |

## Équipe : Groupe 11

- Abdourahmane Diaw
- Coumbel Ka
- Ousmane Niang
- Hawa Diallo
- Abib Traoré

## Documentation de gestion de projet

Le dépôt contient le portfolio d'équipe et les présentations de chaque thème du module, tous appliqués au projet CoopHabitat.

| Thème | Sujet | Livrables |
|---|---|---|
| 2 | Cadrage et initialisation | Charte de projet, matrice des parties prenantes, contraintes et hypothèses |
| 3 | Waterfall et cycle en V | Plan de projet séquentiel comparé à l'approche Agile |
| 4 | Méthodes Agiles (Scrum et Kanban) | Product Backlog, sprint planning, tableau Kanban, User Stories |
| 5 | Planification et ordonnancement | WBS, diagramme de Gantt, chemin critique (PERT) |
| 6 | Gestion des risques | Registre des risques, matrice probabilité × impact, plans de contingence |
| 7 | Coûts et budget | CBS, indicateurs EVM (CPI, SPI, EAC), courbe en S, rapport financier |
| 8 | Ressources humaines et leadership | Matrice RACI, leadership situationnel, plan de développement d'équipe |
| 9 | Communication et reporting | Plan de communication, tableau de bord, rapport d'avancement |
| 10 | Qualité et tests | Plan de tests, Definition of Ready / Done, cas de tests, non-conformités |
| 11 | Gouvernance et cadres de référence | Comparatif PMBOK / PRINCE2 / ITIL, recommandation, cartographie PMBOK |
| 12 | Clôture et retour d'expérience | Rapport de clôture, rétrospective, leçons apprises, base de connaissance |

## Contenu du dépôt (à adapter à votre arborescence)

- `Portfolio_CoopHabitat_Themes2a12.docx` : portfolio d'équipe complet (livrables pratiques et pages de réflexion)
- `Theme4-…`, `Theme5-…`, `Theme8-…`, `Theme9-…`, `Theme10-…`, `Theme11-…`, `Theme12-….pptx` : diaporamas des thèmes
- `Fiche_Synthese_Theme…docx` : fiches de synthèse individuelles

## Critères de réussite du projet

- Le tableau de bord du trésorier affiche en temps réel les membres à jour, en retard et la trésorerie disponible.
- Un rappel automatique est envoyé 3 jours avant l'échéance de cotisation.
- Le workflow d'attribution génère un PV PDF signé numériquement et notifie le bénéficiaire.
- L'espace membre affiche l'historique complet des paiements et le solde restant dû.
- Les rapports financiers sont exportables en PDF et en Excel.
- Le code respecte les principes SOLID et est couvert à au moins 60 % par des tests.

## Licence

Projet pédagogique. Tous droits réservés au Groupe 11.
