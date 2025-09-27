# Projet d’Application de Conversion de Devises
### Membres du groupe :
 1. Joseph Jean Renel
 2. François Steeve
 3. Marcellin Yves Kendy
 4. Destin Edelin
    
Convertisseur de devises permet de convertir rapidement des montants d’une devise à une autre en utilisant des taux de change mis à jour en temps réel. Que l’utilisateur soit un voyageur, un commerçant ou un étudiant, il peut connaître instantanément la valeur de sa monnaie dans plus de 7 devises. L’application est conçue pour être simple, rapide et fiable, même en déplacement.


# Convertisseur-de-devises
## Description
Une interface intuitive où l’utilisateur saisit un montant, sélectionne une devise source et une devise cible, puis obtient la conversion instantanée. L’application se met à jour automatiquement à partir d’une API de taux de change, tout en permettant de sauvegarder les devises favorites.

## User Stories (Fonctionnalités attendues)
### Indispensable (Must have)
1. L’utilisateur doit pouvoir saisir un montant à convertir.
2. L’utilisateur doit pouvoir choisir une devise de départ et une devise d’arrivée.
3. L’application doit afficher le résultat instantanément en utilisant le taux de change le plus récent.
4. L’application doit mettre à jour les taux de change en temps réel (via internet).
5. L’utilisateur doit pouvoir voir la date/heure du dernier taux mis à jour.
6. L’application doit fonctionner en mode portrait sur smartphone.
### Optionnel (Maybe)
1. L’utilisateur peut marquer des devises comme favoris pour un accès rapide.
2. L’application peut stocker les taux récents pour une utilisation hors-ligne limitée.
3. L’utilisateur peut inverser rapidement les devises (ex. EUR ↔ USD).
4. L’application peut proposer un historique de conversions effectuées.
5. L’utilisateur peut visualiser un graphique d’évolution des taux sur 7 ou 30 jours.
   
### Souhaitable (Would be nice to have)
1. L’utilisateur peut activer un mode voyage qui détecte automatiquement la devise locale.
2. Intégration d’un widget pour convertir directement depuis l’écran d’accueil.
3. Possibilité de choisir une API alternative (en cas d’indisponibilité de la principale).
4. Notifications lorsque le taux d’une paire de devises dépasse un seuil défini.

## Écrans & Flux utilisateur

1. Écran principal — champ de saisie du montant, menu déroulant pour devise source et devise cible, bouton « Convertir » (ou conversion automatique).
2. Écran favoris/historique — liste des conversions récentes et devises enregistrées.
3. Réglages — choix du thème (clair/sombre), sélection de l’API, options de mise à jour automatique.
 
## Contraintes techniques & choix recommandés

1. Plateforme : Android (Kotlin) ou multiplateforme (Flutter/React Native).
2. Source des taux : API fiable (ex. ExchangeRate API, Open Exchange Rates).
3. Stockage : Room/SharedPreferences pour les favoris et l’historique.
4. Mise en cache : Conservation des derniers taux pour usage hors-ligne temporaire.
5. Interface : Material Design, boutons lisibles, sélection de devise par liste ou recherche.
   
## Critères d’acceptation (exemples)

1. Si l’utilisateur saisit 100 USD et choisit EUR, le résultat doit afficher le montant exact selon le taux du jour.
2. L’inversion des devises doit s’effectuer en un seul clic.
3. L’application doit signaler clairement si le taux affiché est hors-ligne (non actualisé).
5. Les devises favorites doivent apparaître en haut de la liste déroulante.
   
![Convertisseur de devises](https://github.com/user-attachments/assets/42982dd8-5498-4ddb-b85a-76feadd6615c)


