
## Connexions 6 Chapeaux → VPC — MicroFinanceVerte

### Profil Client — Origines

#### Jobs To Be Done	

| Job                                                                                        | Chapeau d'origine | Citation exacte                                                                                                                   |
| ------------------------------------------------------------------------------------------ | ----------------- | --------------------------------------------------------------------------------------------------------------------------------- |
| Obtenir un petit crédit de campagne sans titre foncier                                    | Chapeau Blanc     | "la majorité des exploitants comme Moussa ne possèdent aucun titre foncier individuel opposable aux institutions financières." |
| Recevoir/envoyer paiements et services financiers via son feature phone                    | Chapeau Blanc     | "Moussa utilise Wave pour recevoir des transferts, mais jamais pour un service financier lié à son activité agricole."         |
| Capitaliser et valoriser l'historique de la tontine comme preuve de fiabilité financière | Chapeau Blanc     | "ces flux réguliers représentent un historique de comportement financier réel"                                                 |

#### Pains

| Pain                                                                           | Chapeau d'origine | Citation exacte                                                                                                                                    |
| ------------------------------------------------------------------------------ | ----------------- | -------------------------------------------------------------------------------------------------------------------------------------------------- |
| Honte et découragement après des refus institutionnels                       | Chapeau Rouge     | "Moussa ressent une honte silencieuse ... 'le système n'est pas fait pour lui'."                                                                  |
| Exclusion numérique si le scoring repose uniquement sur activity mobile money | Chapeau Noir      | "Un scoring alternatif basé sur l'historique Wave peut exclure les exploitants les plus vulnérables"                                             |
| Perte réelle non indemnisée par assurance paramétrique (base‑risk)         | Chapeau Noir      | "une sécheresse localisée sur 2 km² peut ne pas être détectée par une station météo distante de 30 km, laissant Moussa sans indemnisation" |

#### Gains

| Gain                                                                    | Chapeau d'origine | Citation exacte                                                                                                                                            |
| ----------------------------------------------------------------------- | ----------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Activation technique facile (USSD/SMS utilisable)                       | Chapeau Jaune     | "Moussa utilise Wave aujourd'hui, ce qui signifie que la barrière d'activation ... est technique, pas comportementale — il sait déjà composer un code" |
| Valorisation d'une épargne réelle (tontine) comme levier de crédit   | Chapeau Jaune     | "Les tontines prouvent que les exploitants ruraux ont une discipline d'épargne réelle et régulière"                                                    |
| Accès à un micro‑crédit bien calibré augmente rendement et revenus | Chapeau Jaune     | "Un crédit de 100 000–150 000 FCFA bien calibré en début de saison peut doubler le rendement de Moussa"                                                |

### Proposition de Valeur — Origines

#### Pain Relievers

| Pain Reliever                                                                                        |                            Pain adressé | Chapeau d'origine                                      |
| ---------------------------------------------------------------------------------------------------- | ---------------------------------------: | ------------------------------------------------------ |
| Combiner score mobile money avec validation par agent local / preuve photo et historiques de tontine |                    Exclusion par scoring | Chapeau Noir (risque identifié; mitigation dérivée) |
| Ajouter signal communautaire + vérif. terrain avant décision d'indemnisation                       |                Base‑risk de l'assurance | Chapeau Noir (risque identifié; mitigation dérivée) |
| Déployer co‑conception, formation et règles de gouvernance locales avant digitalisation complète | Fracture sociale liée à digitalisation | Chapeau Noir (risque identifié; mitigation dérivée) |

#### Gain Creators

| Gain Creator                                                                           |                 Gain adressé | Chapeau d'origine |
| -------------------------------------------------------------------------------------- | ----------------------------: | ----------------- |
| Onboarding USSD/SMS quasi‑instantané (faible friction)                               |   Activation technique facile | Chapeau Jaune     |
| Piloter localement avec partenaire institutionnel (GIE/IMF) pour légitimer le service | Accès au crédit & confiance | Chapeau Bleu      |

### Éléments Non Tracés

- Aucun — tous les éléments du VPC sont tracés vers les chapeaux (Blanc / Rouge / Noir / Jaune / Vert / Bleu) selon `docs/chapeaux-bono.md`.

### Synthèse de Cohérence

**Alignement :** partiel
**Tension principale :** la proposition est synergiquement alignée mais dépend fortement de la fiabilité du scoring hybride et du déclenchement paramétrique — si ces mécanismes échouent, le service perdra légitimité auprès des exploitants.
**Recommandation avant S3 :** lancer un pilote terrain court (20 exploitants, 2 tontines) pour (1) auditer l'activité Wave et mesurer l'exclusion potentielle, et (2) backtester déclenchements satellite vs rapports locaux sur incidents passés — décider ensuite du protocole de scoring hybride et des règles de co‑validation communautaire.
