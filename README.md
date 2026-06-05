## Équipe projet

<<<<<<< HEAD
| Prénom Nom     | Rôle | GitHub Username | E-mail GitHub                                                                                       |
| --------------- | ----- | ---------------| --------------------------------------------------------------------------------------------------- |
| Bienvenu Mendy  |       | @BemvindoTech  | [bienvenu.mendy@univ-thies.sn  ](bienvenu.mendy@univ-thies.sn)                                         |
| Abdoulaye Ndour |       | @petitlaye03   | [ndourabdoulaye1803@gmail.com](mailto:ndourabdoulaye1803@gmail.com "mailto:ndourabdoulaye1803@gmail.com") |
| Marie Soukèye  |       | @marie-sou      | [mariesr2377@gmail.com](mailto:mariesr2377@gmail.com)             |
| Adja            |       |@AdjaDimeBomou  | [adjabomou99@gmail.com ](mailto:adjabomou99@gmail.com)            |
| Khémesse Diouf  |       | @Khemesse333   |[dioufkhemesse333@gmail.com  ](mailto:dioufkhemesse333@gmail.com)  |
=======
| Prénom Nom                | Rôle                        | GitHub Username | E-mail GitHub                                                                                       |
| -------------------------- | ---------------------------- | --------------- | --------------------------------------------------------------------------------------------------- |
| Bienvenu Mendy             | Chef de Projet               | @BemvindoTech   | [bienvenu.mendy@univ-thies.sn  ](bienvenu.mendy@univ-thies.sn)                                         |
| Abdoulaye Ndour            | Master Prompt Engineer       | @petitlaye03    | [ndourabdoulaye1803@gmail.com](mailto:ndourabdoulaye1803@gmail.com "mailto:ndourabdoulaye1803@gmail.com") |
| Marie Soukèye Rwiyamirira | Développeur UI              | @marie-sou      | [mariesr2377@gmail.com](mailto:mariesr2377@gmail.com)                                                  |
| Adja Dime Bomou            | Responsable Impact & Ethique |                 |                                                                                                     |
| Khemesse Diouf             | Développeur No-Code         | @Khemesse333    | dioufkhemesse333@gmail.com                                                                          |
>>>>>>> 6e78949 (feat(S2): Update directory docs)

---

## Défi

* **Secteur :** Micro-finance verte pour l'agriculture durable — Crédit agricole, assurance récolte et épargne communautaire dans les zones rurales du Sénégal
* **Contexte :** Les petits producteurs agricoles font face à des difficultés d'accès au financement en raison de l'absence de garanties formelles, de leur forte exposition aux risques climatiques et du manque de reconnaissance des mécanismes d'épargne communautaire existants.
* **HMW :** Comment pourrions-nous concevoir une solution de micro-finance verte qui permette aux agriculteurs ruraux d'accéder à des services de crédit agricole, d'assurance récolte et d'épargne communautaire adaptés à leur réalité économique, sociale et climatique ?

---

## Livrables S1

- [X] Fiche équipe → [Voir le fichier](docs/fiche-equipe.md)
- [X] Dépôt GitHub public créé
- [X] Carte d'empathie → [Voir le fichier](docs/carte-empathie.md)
- [X] Énoncé HMW validé

---

## Architecture du dépôt

```
Micro-fin-app/ 
├── README.md
└── docs/
    ├── fiche-equipe.md
    └── carte-empathie.md
  
```

## Notre défi — HMW Définitif S2

"Comment pourrions-nous aider les petits exploitants agricoles du Sénégal à construire une identité financière alternative — à partir de leurs flux mobile money et de leur épargne communautaire existante — pour accéder à un crédit de campagne, une assurance récolte et une épargne sécurisée, sans titre foncier ni compte bancaire formel, via un service accessible sur feature phone ?"

## Livrables S2

| Fichier                       | Contenu                       |
| ----------------------------- | ----------------------------- |
| docs/chapeaux-bono.md         | 6 Chapeaux de Bono            |
| docs/contraintes-mvp.md       | Contraintes non négociables  |
| docs/hypotheses-validation.md | Hypothèses à tester en S3   |
| docs/metriques-succes.md      | Métriques de succès S6      |
| docs/vpc.md                   | Value Proposition Canvas      |
| docs/vpc-connections.md       | Traçabilité Chapeaux → VPC |
| docs/backlog-s3.md            | User stories S3               |
| docs/hmw-definitif.md         | HMW définitif validé        |

---





# Note Annexe S1 

## Énoncé HMW validé

> Observations et Opportunités de Conception

## Observations

### Obs. 1 — Crédit impossible sans garanties formelles ni historique bancaire

Les petits exploitants agricoles ne peuvent souvent pas accéder au crédit faute de garanties reconnues par les institutions financières (titre foncier, relevés bancaires, historique de crédit).

### Obs. 2 — Peur de l'endettement face aux risques climatiques imprévisibles

Les agriculteurs hésitent à contracter un prêt en raison de l'incertitude liée aux conditions climatiques (sécheresse, inondations, pluies irrégulières) qui peuvent compromettre leurs récoltes.

### Obs. 3 — Tontines utilisées mais gestion manuelle, peu transparente

Les systèmes d'épargne communautaire sont largement adoptés, mais leur gestion repose souvent sur des méthodes manuelles qui limitent la transparence et la traçabilité.

---

## Frustration centrale

> Difficulté à accéder à des services financiers fiables et adaptés à la réalité agricole et climatique des ruraux sénégalais.

---

# Énoncés « Comment pourrions-nous... » (HMW)

## HMW 1 — Crédit agricole

### Question

**Comment pourrions-nous aider les petits exploitants à démontrer leur fiabilité financière autrement qu'avec un titre foncier ou un relevé bancaire ?**

### Mots-clés

- Crédit
- Confiance
- Inclusion

### Ancrage

Observation 1

---

## HMW 2 — Assurance récolte

### Question

**Comment pourrions-nous permettre à un agriculteur de s'engager financièrement en saison sèche, sans craindre que la pluie ou la sécheresse lui fasse tout perdre ?**

### Mots-clés

- Assurance
- Risque climatique
- Sécurité

### Ancrage

Observation 2

---

## HMW 3 — Épargne communautaire

### Question

**Comment pourrions-nous renforcer la confiance et la transparence au sein des groupements d'épargne existants, sans rompre leur logique communautaire ?**

### Mots-clés

- Épargne
- Tontine
- Transparence

### Ancrage

Observation 3

---

## HMW 4 — Épargne × Crédit

### Question

**Comment pourrions-nous faire en sorte que l'épargne accumulée dans une tontine puisse servir de porte d'entrée vers un crédit agricole formel ?**

### Mots-clés

- Épargne
- Crédit
- Passerelle

### Ancrage

Observation 3 + Observation 1

---

## HMW 5 — Vision systémique

### Question

**Comment pourrions-nous concevoir un service financier qui s'adapte au calendrier agricole et aux aléas climatiques du Sénégal, plutôt que d'imposer des conditions fixes à l'agriculteur ?**

### Mots-clés

- Système
- Saisonnalité
- Adaptation

### Ancrage

Observation 1 + Observation 2 + Observation 3

---

# Axes de réflexion

## Crédit agricole

- Garanties alternatives
- Historique communautaire
- Inclusion financière

## Assurance récolte

- Protection contre les aléas climatiques
- Réduction du risque d'endettement
- Sécurisation des revenus agricoles

## Épargne communautaire

- Digitalisation des tontines
- Transparence et traçabilité
- Renforcement de la confiance collective

## Croisement / Vision système

- Épargne communautaire → Crédit agricole
- Crédit agricole → Assurance récolte
- Produits financiers adaptés aux saisons agricoles
- Services financiers flexibles et résilients face au climat

---

# Carte d'empathie — Moussa Diallo

## Persona

| Champ                         | Détail                                                                    |
| ----------------------------- | -------------------------------------------------------------------------- |
| **Prénom, âge**       | Moussa Diallo, 43 ans                                                      |
| **Profession**          | Petit exploitant agricole                                                  |
| **Localisation**        | Kaolack, Sénégal                                                         |
| **Cultures**            | Mil, arachide, niébé — 2,5 ha                                           |
| **Situation familiale** | Père de 5 enfants                                                         |
| **Équipement digital** | Feature phone (Nokia basique) — Wave pour recevoir de l'argent uniquement |

**Problème principal :** Impossible d'obtenir un crédit agricole avant la saison des pluies : sans titre foncier ni compte bancaire, les caisses et banques refusent sa demande, le forçant à emprunter à des taux usuraires auprès de commerçants locaux.

---

## 1. Pense et ressent

- Il pense que les banques et les caisses ne sont pas faites pour des gens comme lui — trop de papiers, trop de conditions, trop loin.
- Il ressent une honte silencieuse à l'idée de se retrouver endetté face à ses enfants si la récolte est mauvaise.
- Il porte seul l'inquiétude de la saison : chaque matin nuageux en juillet lui rappelle que tout peut basculer en quelques jours.

**Émotions dominantes :** Anxiété · Méfiance · Résignation

---

## 2. Voit

- Des voisins qui s'endettent auprès de Modou le commerçant à 80% d'intérêt sur la saison, et qui revendent leur récolte à perte pour rembourser.
- Des publicités pour Orange Money à la radio, mais aucun agent capable de lui expliquer comment ça peut l'aider pour son champ.
- Sa femme gérer la tontine du quartier avec un cahier abîmé — elle sait exactement qui doit quoi, mais tout repose sur sa mémoire.

---

## 3. Entend

- Son frère aîné au téléphone : *"Ne va pas à la banque, ils vont te demander des choses que tu n'as pas, tu vas perdre ta journée."*
- À la mosquée du vendredi : des discussions sur la sécheresse de l'an passé, les pertes, et l'impossibilité d'être remboursé par qui que ce soit.
- À la radio RFM : un reportage sur des agriculteurs du Sine-Saloum qui ont reçu un prêt d'une ONG — mais il ne sait pas comment les contacter.

---

## 4. Dit et fait

- Il se lève à 5h30 pour arriver au champ avant la chaleur. Il note ses dépenses dans sa tête — jamais sur papier.
- Il utilise Wave pour recevoir de l'argent de son fils à Dakar, mais ne fait jamais de transfert lui-même.
- En public, il dit que "ça va, la saison est bonne" — mais en privé, il compte les jours avant la récolte avec angoisse.

> *"Si je pouvais avoir de l'argent juste pour les semences et l'engrais, je pourrais doubler ce que je produis. Mais personne ne me fait confiance sans papier."*

---

## 5. Frustrations (Pains)

- **Exclusion financière :** Exclu du crédit formel faute de garanties — contraint aux usuriers à 60–80% de taux sur la saison.
- **Absence de filet de sécurité :** Aucune protection face aux aléas climatiques : une mauvaise saison efface plusieurs années d'efforts.
- **Invisibilité institutionnelle :** Sentiment que les services financiers sont conçus pour "d'autres personnes", pas pour lui.

---

## 6. Aspirations (Gains)

- **Crédit accessible :** Accéder à un petit crédit de 50 000–150 000 FCFA avant l'hivernage, remboursable après la récolte, sans démarche humiliante.
- **Sécurité automatique :** Savoir qu'en cas de sécheresse, il recevra une aide automatiquement — sans avoir à prouver, négocier ni attendre.
- **Projet de vie :** Pouvoir montrer à ses enfants qu'il a bâti quelque chose de solide — agrandir le champ, acheter un âne, financer l'école.

---

## Observations sources

| #      | Observation                                                        |
| ------ | ------------------------------------------------------------------ |
| Obs. 1 | Crédit impossible sans garanties formelles ni historique bancaire |
| Obs. 2 | Peur de l'endettement face aux risques climatiques imprévisibles  |
| Obs. 3 | Tontines utilisées mais gestion manuelle, peu transparente        |

---

*Persona fictif basé sur les interviews terrain — projet micro-finance verte, Sénégal.*
