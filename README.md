# SimulateurAAC-PdFv2
Outil web de calcul de la subvention départementale et de contrôle de la participation minimale du maître d'ouvrage, conforme à l'article L.1111-10, III du Code général des collectivités territoriales (version en vigueur depuis le 31 mars 2024).

# Simulateur du plan de financement - Aide aux communes

Outil web de calcul de la subvention départementale et de contrôle de la participation minimale du maître d'ouvrage, conforme à l'article L.1111-10, III du Code général des collectivités territoriales (version en vigueur depuis le 31 mars 2024).

## Fonctionnalités

- Saisie du coût total HT, de la dépense subventionnable, de la subvention départementale proposée et de la participation du maître d'ouvrage.
- Financeurs publics (jusqu'à 10) et privés (jusqu'à 5) avec libellés libres. Les financements privés sont exclus de l'assiette.
- Contrôle de l'équilibre du plan de financement, avec bouton « Reporter le solde ».
- Calcul de la participation minimale (20 % du FAPP en droit commun) et écrêtement automatique de la subvention départementale, arrondi à l'euro inférieur.
- Si l'écrêtement ne suffit pas, la subvention est ramenée à 0 € et l'écart restant est signalé.
- Régimes paramétrables : droit commun (taux limite 80 %), FEDER (85 %), rénovation scolaire fixée par le préfet (90 %), dérogation préfectorale à taux libre.
- Taux du Département affiché par rapport à la dépense subventionnable et au coût HT.
- Récapitulatif imprimable ou enregistrable en PDF.

## Caractéristiques techniques

- Fichier HTML unique et autonome (CSS, JavaScript, logos et bandeau intégrés).
- Aucune dépendance externe, aucun appel réseau.
- Politique de sécurité de contenu (CSP) avec empreintes SHA-256 : toute modification du code impose de recalculer ces empreintes.
- Calcul entièrement local en JavaScript, en centimes entiers pour éviter les erreurs d'arrondi.

## Protection des données (RGPD)

- Aucune donnée personnelle n'est demandée ni transmise.
- Aucune persistance : pas de cookie, de stockage local ni de base de données.
- Les journaux de connexion de l'hébergeur du site restent soumis à la politique de protection des données du Département.

## Statut

Version 1.0 - paramétrage au 31/03/2024. Mentions RGPD à valider par le délégué à la protection des données avant mise en ligne.

## Tests

Six scénarios validés sur navigateur (écrêtement, plan conforme, insuffisance, dérogation, déséquilibre, arrondi), sans erreur console, affichage mobile sans défilement horizontal.

## Licence et usage

Usage interne au Département de l'Oise. Les logos et la charte graphique appartiennent au Département.
