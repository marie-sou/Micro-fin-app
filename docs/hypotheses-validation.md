## Hypothèses de Validation — MicroFinanceVerte

### HMW Définitif

"Comment pourrions-nous aider les petits exploitants agricoles du Sénégal à construire une identité financière alternative — à partir de leurs flux mobile money et de leur épargne communautaire existante — pour accéder à un crédit de campagne, une assurance récolte et une épargne sécurisée, sans titre foncier ni compte bancaire formel, via un service accessible sur feature phone ?"

### Hypothèses CRITIQUES

*(Si fausse → le MVP ne fonctionne pas)*

#### Hypothèse C1

**Affirmation :** Nous croyons que l'utilisation d'un score basé uniquement sur l'historique Wave exclura une portion significative des exploitants les plus vulnérables.
**Indicateur :** Nous le saurons si ≥30% des exploitants ciblés n'ont pas d'activité Wave suffisante pour générer un score utilisable et/ou refusent d'adopter le service après explication.
**Méthode :** entretiens terrain + collecte consentie des relevés Wave (audit simple) + tests d'acceptation sur 20 exploitants.
**Qui valide :** PM + agent terrain / leader de GIE local.
**Délai S3 :** semaine 1–2

#### Hypothèse C2

**Affirmation :** Nous croyons que les indices pluviométriques satellite disponibles ne détecteront pas de façon fiable les pertes localisées, entraînant des indemnisations manquantes.
**Indicateur :** Nous le saurons si le backtest historique montre que ≥50% des épisodes de perte locale signalés par exploitants ne sont pas corrélés à un déclenchement d'indice satellite.
**Méthode :** backtest historique (données satellite vs rapports locaux/expériences passées) + vérification terrain ponctuelle avec 3 incidents simulés/rapportés.
**Qui valide :** Data analyste (ou stagiaire data) + partenaire météo local + responsable impact.
**Délai S3 :** semaine 1–3

### Hypothèses IMPORTANTES

*(Si fausse → expérience dégradée mais MVP utilisable)*

#### Hypothèse I1

**Affirmation :** Nous croyons que digitaliser les registres de tontine sans accompagnement participatif augmentera la méfiance et réduira la cohésion du groupement.
**Indicateur :** Nous le saurons si, après un pilote de 4 semaines, >25% des membres déclarent moins confiance ou cessent de cotiser dans la tontine numérisée.
**Méthode :** atelier co‑conception + pilote USSD sur 2 tontines et interviews post‑pilot.
**Qui valide :** Responsable Impact / facilitateur terrain + trésorier du GIE.
**Délai S3 :** semaine 2–4

### Hypothèses SECONDAIRES

*(À valider après le MVP)*

#### Hypothèse S1

**Affirmation :** Nous croyons qu'un mécanisme de co‑validation communautaire (ex. seuil de signalement 3/5) réduira le coût d'expertise et la fraude sans sacrifier la rapidité d'indemnisation.
**Indicateur :** Nous le saurons si le pilote montre une réduction ≥30% du coût moyen de vérification par sinistre tout en gardant un taux de contestation <15%.
**Méthode :** pilote S4 combinant signalements SMS + vérif. terrain aléatoire.
**Qui valide :** Opérationnel pilote + analyste coûts.
**Délai S3 :** planification S3, test en S4

### Priorité de Validation S3

La première chose à tester en S3 : réaliser en semaine 1–2 un audit terrain auprès de 20 exploitants (divers niveaux d'usage mobile money) pour mesurer l'exclusion potentielle du scoring basé sur Wave (Hypothèse C1).
