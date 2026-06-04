## Contraintes MVP — MicroFinanceVerte

### Persona
Moussa Diallo · 43 · Petit exploitant agricole · Kaolack · Feature phone (Wave)

### Chapeau Blanc — Faits & Données
- La majorité des personas (ex. Moussa Diallo, 43 ans) ont un feature phone et utilisent Wave/Orange Money pour recevoir de l'argent plutôt que de gérer des comptes bancaires formels.
- Les tontines locales existent comme mécanisme d'épargne et de garantie sociale, mais sont tenues manuellement (cahiers) et manquent de traçabilité numérique vérifiable.
- Les montants recherchés sont modestes (≈50 000–200 000 FCFA) et les agriculteurs remboursent généralement après la récolte; prêts informels à taux très élevés (60–100% saisonnier) sont courants.

### Chapeau Noir — Risques & Critique
- Risque de base‑risk pour une assurance paramétrique : l'indice météo choisi peut mal refléter les pertes réelles, entraînant perceptions d'injustice.
- Digitalisation des tontines peut exclure les membres les moins alphabétisés ou sans réseau mobile fiable, fragilisant la confiance collective.
- Transformer l'épargne tontine en "garantie" reconnue pourrait encourager collusion ou pressions sociales, augmentant le risque de défaut groupé.

### Contraintes Non Négociables

#### Contrainte 1
**Critère :** Le MVP DOIT fonctionner sur feature phones via USSD/SMS et permettre l'enregistrement des cotisations sans application smartphone.
**Origine :** Chapeau Blanc
**Élimine :** interfaces smartphone natives et dépendance à une application mobile riche

#### Contrainte 2
**Critère :** Le MVP NE DOIT PAS reposer uniquement sur un indice météo non vérifié pour déclencher des indemnisations ; il DOIT inclure un mécanisme d'arbitrage local pour contester les paiements.
**Origine :** Chapeau Noir
**Élimine :** assurance paramétrique sans procédure de contestation ni validation terrain

#### Contrainte 3
**Critère :** Le MVP DOIT garantir l'inclusion des membres analphabètes (reçus vocaux ou confirmation par agent local).
**Origine :** Chapeau Blanc
**Élimine :** interfaces textuelles seules sans alternative vocale ou humaine

#### Contrainte 4
**Critère :** Le MVP DOIT enregistrer et rendre consultable l'historique des cotisations (traçabilité minimale), accessible au groupe et à l'agent validateur.
**Origine :** Chapeau Blanc
**Élimine :** système non traçable (cahier uniquement) comme unique source de vérité

#### Contrainte 5
**Critère :** Le MVP NE DOIT PAS transformer l'épargne communautaire en garantie sans protocole de gouvernance et protection sociale (prévenir pressions et collusion).
**Origine :** Chapeau Noir
**Élimine :** mécanisme automatique de saisie d'épargne tontine comme garantie sans accords et filet de protection

### Fonctionnalités Éliminées
- Application smartphone riche → éliminée parce que la majorité des utilisateurs ont des feature phones.
- Automatisation complète de l'indemnisation paramétrique sans recours → éliminée à cause du risque de base‑risk et de défiance.
- Utilisation de l'historique tontine comme garantie sans protocole → éliminée pour prévenir pressions sociales et défauts groupés.
- Intégration bancaire immédiate (exiger compte bancaire) → éliminée car contradictoire avec l'objectif d'accès sans compte formel.

### Critère de Validation Final
Le MVP est valide si et seulement si il permet, via USSD/SMS ou voix et avec gouvernance locale minimale, d'enregistrer la cotisation de la tontine, de produire un historique traçable consultable par le groupe, et d'ouvrir l'accès à un micro‑crédit de campagne pilote tout en prévoyant un mécanisme d'arbitrage pour les indemnisations paramétriques.

### Instructions pour usage
1. Ouvrez `docs/chapeaux-bono.md` et vérifiez que les sections Chapeau Blanc et Chapeau Noir correspondent aux éléments ci‑dessus.
2. Ajustez les contraintes si nécessaire pour qu'elles reflètent fidèlement vos données terrain.
3. Committez ce fichier sur GitHub avec le message : `docs: ajout contraintes-mvp.md - Contraintes MVP MicroFinanceVerte`.

