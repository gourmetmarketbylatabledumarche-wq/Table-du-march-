# Brigade · La Table du Marché

Application de gestion du personnel du restaurant La Table du Marché (Marrakech).
Un seul fichier, `app/index.html`. Pas d'installation ni de serveur : il suffit de l'ouvrir sur un téléphone, une tablette ou un ordinateur.

## Modules

| Module | Ce qu'il fait |
|---|---|
| **Tableau de bord** | Présents maintenant, manquants, retards, avancement des checklists, masse salariale. Alertes regroupées par employé : retards répétés, absences injustifiées, avances trop élevées, jours sans pointage. |
| **Pointage** | Arrivée et départ en un clic. Retard calculé automatiquement à partir du planning, avec une tolérance réglable. Statuts : absence injustifiée, absence justifiée, maladie. |
| **Planning** | Grille de la semaine par service (Matin / Soir / Coupure / Repos / Congé), basée sur le planning type de chaque employé. Reprise de la semaine précédente, alerte au-delà de 48 h par semaine, envoi du planning sur WhatsApp. |
| **Équipe** | Fiches employés : poste, service, téléphone, CIN, CNSS, embauche, salaire mensuel ou journalier, horaire, jour de repos. Historique des 14 derniers jours. |
| **Checklists** | Ouverture, mise en place, service, fermeture, hygiène HACCP. Tâches attribuées à un responsable, cochées chaque jour avec l'heure. Rappel WhatsApp des tâches restantes. |
| **Paie & avances** | Calcul du net à payer pour chaque employé : absences retenues au prorata, pénalités de retard facultatives, primes, retenues, avances. Fiche individuelle à copier et export CSV pour Excel. |
| **Journal RH** | Avertissements, félicitations et notes datés par employé. |
| **Réglages** | Horaires des services, tolérance, règles de retenue, sauvegarde et restauration (JSON). |

## Données

Les données sont enregistrées dans le navigateur de l'appareil utilisé (localStorage).
Faites une sauvegarde chaque semaine depuis **Réglages → Télécharger la sauvegarde**.
Au premier lancement, l'application affiche une équipe d'exemple. Le bouton « Effacer et commencer avec mon équipe » la supprime.

Les montants de paie sont bruts et indicatifs. Ils n'incluent pas les cotisations CNSS/AMO ni l'IR.
