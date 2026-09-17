# Estimate Drift Watch for Jira — Documentation

[English](#english) | [Français](#français)

---

## English

### Overview

**Estimate Drift Watch for Jira** helps Jira teams detect estimation drift by comparing an issue’s **first known Original Estimate** with its **current forecast**.

The app is designed to help project managers and delivery teams identify issues that are still on track, beginning to drift, or significantly overrunning their initial estimate.

### How the forecast is calculated

The current forecast is calculated as:

**Forecast = Time Spent + Remaining Estimate**

The drift is then calculated as:

**Drift = Forecast - Initial Estimate**

And the drift percentage as:

**Drift % = Drift / Initial Estimate × 100**

### Initial estimate baseline

Estimate Drift Watch uses the **first known Original Estimate** found in Jira history as the baseline.

This means that if an issue was initially estimated at 5h, later changed to 8h, and then changed again to 6h, the app still keeps **5h** as the historical baseline.

This helps teams preserve the original estimation context even after Jira estimates are updated.

### Project overview

The project-level page provides a summary of estimation drift across measurable issues.

It includes:

- number of issues analysed;
- number of measurable issues;
- number of drifting issues;
- number of critical drifts;
- total initial estimate;
- current forecast;
- total drift;
- overall drift percentage.

The issue table also displays:

- issue key;
- summary;
- status;
- assignee;
- initial estimate;
- time spent;
- remaining estimate;
- current forecast;
- drift;
- drift percentage;
- severity.

### Issue-level panel

Each Jira issue includes an Estimate Drift panel with the main indicators:

- Initial Estimate;
- Time Spent;
- Remaining Estimate;
- Current Forecast;
- Drift;
- Drift %.

The panel also provides a short interpretation of the current estimation status.

If the Jira Original Estimate has changed since its first known value, the app indicates that the historical baseline has been preserved.

### Severity levels

Estimate Drift Watch classifies measurable issues into simple severity levels to make risks easier to identify.

Depending on the calculated drift, an issue may appear as:

- **OK**
- **Warning**
- **Critical**
- **Not measurable**

An issue is not measurable when no usable initial estimate can be reconstructed.

### Supported languages

The app supports:

- English
- French

Visible labels are adapted to the Jira user locale where supported.

### Time tracking

Durations are formatted using Jira time-tracking settings, including the configured number of working hours per day when available.

Examples:

- English: `1d 2h`
- French: `1j 2h`

### Data handling and privacy

Estimate Drift Watch is built on **Atlassian Forge**.

The app:

- does not use an external application backend;
- does not use an external application database for Jira issue data;
- does not use external analytics or advertising trackers;
- does not intentionally transmit Jira End-User Data to external third-party services.

The app only requests the Jira permissions required for its functionality.

Privacy policy:

https://kessosan.github.io/estimate-drift-watch-docs/PRIVACY_POLICY.html

### Support

For support requests, bug reports, or feature requests, please use the support page:

https://kessosan.github.io/estimate-drift-watch-docs/SUPPORT.html

### Limitations

Estimate Drift Watch depends on the Jira estimation and worklog data available for each issue.

Results may be incomplete when:

- no Original Estimate has ever been set;
- issue history is unavailable;
- time tracking data is incomplete;
- permissions prevent access to the required Jira data.

The app is intended as a project monitoring aid and does not replace project governance or delivery decisions.

---

## Français

### Présentation

**Estimate Drift Watch for Jira** aide les équipes Jira à détecter les dérives d’estimation en comparant la **première estimation d’origine connue** d’un ticket avec sa **prévision actuelle**.

L’application est conçue pour aider les chefs de projet et les équipes de delivery à identifier rapidement les tickets qui restent conformes à l’estimation initiale, commencent à dériver ou présentent un dépassement significatif.

### Calcul de la prévision

La prévision actuelle est calculée ainsi :

**Prévision = Temps consommé + Reste à faire**

La dérive est ensuite calculée ainsi :

**Dérive = Prévision - Estimation initiale**

Et le pourcentage de dérive :

**Dérive % = Dérive / Estimation initiale × 100**

### Estimation initiale de référence

Estimate Drift Watch utilise comme référence la **première Original Estimate connue dans l’historique Jira**.

Par exemple, si un ticket a été estimé initialement à 5h, puis modifié à 8h, puis à 6h, l’application conserve **5h** comme estimation initiale historique.

Cela permet de préserver le contexte de l’estimation d’origine même lorsque l’estimation Jira est modifiée par la suite.

### Vue projet

La page au niveau projet fournit une synthèse des dérives d’estimation sur les tickets mesurables.

Elle affiche notamment :

- le nombre de tickets analysés ;
- le nombre de tickets mesurables ;
- le nombre de tickets en dérive ;
- le nombre de dérives critiques ;
- l’estimation initiale totale ;
- la prévision actuelle ;
- la dérive totale ;
- le pourcentage de dérive global.

Le tableau des tickets affiche également :

- la clé du ticket ;
- le résumé ;
- le statut ;
- le responsable ;
- l’estimation initiale ;
- le temps consommé ;
- le reste à faire ;
- la prévision actuelle ;
- la dérive ;
- le pourcentage de dérive ;
- la sévérité.

### Panneau au niveau du ticket

Chaque ticket Jira dispose d’un panneau Estimate Drift présentant les principaux indicateurs :

- Estimation initiale ;
- Temps consommé ;
- Reste à faire ;
- Prévision actuelle ;
- Dérive ;
- Dérive %.

Le panneau fournit également une interprétation synthétique de la situation actuelle du ticket.

Lorsque l’Original Estimate Jira a été modifiée depuis sa première valeur connue, l’application indique que la référence historique a été conservée.

### Niveaux de sévérité

Estimate Drift Watch classe les tickets mesurables selon des niveaux de sévérité simples afin de faciliter l’identification des risques.

Selon la dérive calculée, un ticket peut apparaître comme :

- **OK**
- **Attention**
- **Critique**
- **Non mesurable**

Un ticket est non mesurable lorsqu’aucune estimation initiale exploitable ne peut être reconstruite.

### Langues prises en charge

L’application prend en charge :

- le français ;
- l’anglais.

Les libellés visibles sont adaptés à la langue de l’utilisateur Jira lorsque cela est pris en charge.

### Suivi du temps

Les durées sont formatées à partir des paramètres de suivi du temps Jira, notamment le nombre d’heures de travail par jour lorsque cette information est disponible.

Exemples :

- Français : `1j 2h`
- Anglais : `1d 2h`

### Données et confidentialité

Estimate Drift Watch est développé sur **Atlassian Forge**.

L’application :

- n’utilise pas de backend applicatif externe ;
- n’utilise pas de base de données applicative externe pour les données des tickets Jira ;
- n’utilise pas de service d’analytics externe ni de tracker publicitaire ;
- ne transmet pas intentionnellement les données utilisateur Jira à des services tiers externes.

L’application demande uniquement les permissions Jira nécessaires à son fonctionnement.

Politique de confidentialité :

https://kessosan.github.io/estimate-drift-watch-docs/PRIVACY_POLICY.html

### Support

Pour toute demande de support, signalement de bug ou suggestion de fonctionnalité, utilisez la page de support :

https://kessosan.github.io/estimate-drift-watch-docs/SUPPORT.html

### Limites

Estimate Drift Watch dépend des données d’estimation et de suivi du temps disponibles dans Jira pour chaque ticket.

Les résultats peuvent être incomplets lorsque :

- aucune Original Estimate n’a jamais été renseignée ;
- l’historique du ticket n’est pas accessible ;
- les données de suivi du temps sont incomplètes ;
- les permissions ne permettent pas d’accéder aux données Jira requises.

L’application est un outil d’aide au pilotage projet et ne remplace pas les décisions de gouvernance ou de delivery.
