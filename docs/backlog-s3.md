## Backlog S3 — MicroFinanceVerte

### HMW Définitif
"Comment pourrions-nous aider les petits exploitants agricoles du Sénégal à construire une identité financière alternative — à partir de leurs flux mobile money et de leur épargne communautaire existante — pour accéder à un crédit de campagne, une assurance récolte et une épargne sécurisée, sans titre foncier ni compte bancaire formel, via un service accessible sur feature phone ?"

### User Stories MUST
*(À construire obligatoirement en S3)*

#### US-01
**Story :** En tant que Moussa, je veux enregistrer la cotisation de ma tontine en composant un code USSD et recevoir un reçu qui confirme l'enregistrement, afin de garder une trace transparente de mes épargnes.  
**Priorité :** MUST  
**Outil :** Dify (backend) + Africastalking/Twilio USSD + SMS API  
**Effort :** moyen  
**Adresse :** Gain Creator (activation USSD) + Contrainte 4 (traçabilité)  
**Critère d'acceptation :** 
- L'exploitant compose #TONTINE#<montant> et reçoit un SMS de confirmation avec date/montant dans les 30 secondes.
- L'enregistrement est stocké et consultable en backend.
- Testé avec 5 exploitants et 100% de réussite.

#### US-02
**Story :** En tant qu'agent local du GIE, je veux consulter l'historique complet des cotisations de ma tontine (noms, montants, dates) via une interface simple, afin de vérifier la transparence et valider les membres pour le crédit.  
**Priorité :** MUST  
**Outil :** Dify (backend) + Google Sheets / Firebase + SMS de consultation  
**Effort :** moyen  
**Adresse :** Pain Reliever (scoring hybride) + Contrainte 4 (consultabilité)  
**Critère d'acceptation :**
- Agent envoie SMS: *HISTORIQUE* et reçoit lien/fichier avec tableau cotisations.
- Historique inclut: nom, montant, date, cumul par personne.
- Démo: consulter historique pour 2 tontines pilotes.

#### US-03
**Story :** En tant qu'agent de terrain, je veux recevoir un signal SMS simple pour les cotisations anormales (> 2× moyenne) ou défaillantes (pas de cotisation 3 semaines), afin de vérifier rapidement les anomalies.  
**Priorité :** MUST  
**Outil :** Dify (logique) + SMS  
**Effort :** faible  
**Adresse :** Gain Creator (gouvernance locale) + Contrainte 3 (inclusion)  
**Critère d'acceptation :**
- Agent reçoit SMS: "Alerte: Moussa a cotisé 150k (vs 50k normal)" ou "Alerte: Malick absent depuis 3 semaines".
- Alerts envoyées chaque lundi matin.
- Testé sur 2 semaines de pilote.

### User Stories SHOULD
*(À construire si le temps le permet)*

#### US-04
**Story :** En tant que Moussa, je veux connaître mon "score d'épargne" (% de régularité + cumul) afin de savoir si je peux accéder à un crédit de campagne.  
**Priorité :** SHOULD  
**Outil :** Dify (calcul) + SMS réponse  
**Effort :** moyen  
**Adresse :** Gain Creator (accès crédit) + Pain Reliever (scoring hybride)  
**Critère d'acceptation :**
- Moussa envoie SMS: *SCORE* et reçoit: "Score: 78% — Crédit possible: 100k FCFA".
- Score = (cotisations régulières / 12 semaines) × (cumul / seuil référence).
- Non automatique — validé manuellement par agent avant déclenchement crédit.

#### US-05
**Story :** En tant que Moussa, si mon score d'épargne atteint 75%, je veux recevoir une offre pré-approuvée de crédit de campagne (montant, taux, durée), afin de planifier mon financement de saison.  
**Priorité :** SHOULD  
**Outil :** Dify (logique) + SMS + formulaire consent Dify  
**Effort :** moyen  
**Adresse :** Gain Creator (accès crédit) + Contrainte 5 (protocole gouvernance)  
**Critère d'acceptation :**
- SMS: "Crédit de 100k FCFA disponible. Taper ACCEPTER pour formulaire" → Dify form link.
- Formulaire inclut consentement pour vérification tontine + préavis arbitrage.
- Offre reste valide 7 jours.

### User Stories COULD
*(Roadmap post-MVP)*

#### US-06
**Story :** En tant que Moussa, je veux m'inscrire à une assurance récolte paramétrique simple qui indemnise si la pluviométrie chute <60mm/mois, et recevoir l'indemnité directement via Wave.  
**Priorité :** COULD  
**Outil :** Dify + SMS + API météo (OpenWeatherMap) + Wave API  
**Effort :** élevé  
**Adresse :** Produit & Service (assurance) + Pain Reliever (co-validation + arbitrage)  
**Critère d'acceptation :**
- Moussa envoie SMS: *ASSURANCE* → reçoit termes simples et prime (ex: 5k FCFA/mois).
- Système récupère données météo via API + signal SMS du groupement (3/5 signalements perte).
- Indemnisation automatique seulement après arbitrage local validation en 48h.
- Démo: simuler 1 cycle d'indemnisation sur données historiques.

#### US-07
**Story :** En tant que Moussa, je veux que mes transactions Wave (versements reçus) soient automatiquement importées comme "preuve de flux" dans mon passeport agricole, afin de renforcer mon score.  
**Priorité :** COULD  
**Outil :** Bolt.new (webhook) + Wave API + Dify backend  
**Effort :** élevé  
**Adresse :** Produit & Service (passeport agricole) + Pain Reliever (scoring hybride)  
**Critère d'acceptation :**
- Chaque réception Wave via Wave Callback déclenche enregistrement dans passeport.
- Passeport consultable via SMS: *PASSEPORT* → résumé flux/score/statut crédit.
- Testé avec 5 comptes Wave réels (données anonymisées).

### Sprint S3

**Semaine 1 :** 
- US-01: Enregistrement USSD cotisation + SMS reçu (setup Dify + USSD gateway).
- US-02: Backend historique + consultation simple.
- **Délivrable:** Système enregistrement/consultation fonctionnel sur 2 tontines pilotes.

**Semaine 2 :** 
- US-03: Alertes anomalies (logique Dify simples).
- US-04: Score d'épargne calculation.
- **Délivrable:** Alertes opérationnelles + premiers scores calculés.

**Semaine 3 (if time):**
- US-05: Déclenchement offre crédit seuil + formulaire consentement.
- **Délivrable:** Pilote d'accès crédit testé avec 3 exploitants.

**Démo S6 :** 
- ✅ US-01 en live: Moussa compose *COTISATION#50000* → SMS reçu confirmant enregistrement.
- ✅ US-02 en live: Agent consulte historique via SMS et visualise 4 semaines de cotisations sur affichage.
- ✅ US-03 en live: Alerte anomalie reçue et validée par agent.
- *Bonus si temps:* US-04 score affiché pour 1 exploitant.
