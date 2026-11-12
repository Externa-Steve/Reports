---
titre: "Audit de sécurité réseau : cabinet médical"
type: cas-client
secteur: santé
role: auditeur sécurité
mission: réelle (client anonymisé)
statut: livré
---

# Cas client 01 : audit d'un cabinet médical

> [!NOTE]
> Mission réelle, client anonymisé.
> Données de santé : secret médical + RGPD (art. 9).

## Contexte

Petit cabinet médical : quelques postes, un stockage réseau, une imprimante réseau, une box opérateur grand public.
Le poste principal manipule des données de santé via un logiciel métier et une base de données locale.

**Enjeux :** secret médical, RGPD (art. 9), continuité des soins.
Le cabinet n'avait jamais fait auditer son informatique.

## Ma mission

Évaluer le niveau de sécurité **réel** du poste sensible et du réseau local, puis livrer des actions correctives priorisées, compréhensibles par un non-informaticien.

## Démarche

1. **Reconnaissance OSINT** : exposition publique du cabinet et de son personnel (surface d'attaque externe).
2. **Cartographie réseau** : découverte des hôtes, scan de ports en mode prudent (sans perturber l'activité), identification des services exposés.
3. **Audit du poste sensible, sur site** : configuration Windows en ligne de commande (pare-feu, antivirus, comptes, mises à jour, accès distants).
4. **Rapport** : constats classés par criticité, chacun avec son risque métier expliqué simplement.
5. **Plan de remédiation** : actions sous 24-48 h, cette semaine, ce mois.

## Constats

| Niveau | Constat | Risque métier |
|---|---|---|
| Critique | Pare-feu du poste désactivé | Aucune barrière réseau sur le poste qui porte les données de santé |
| Critique | Mot de passe Wi-Fi récupérable en clair | Accès au réseau local pour quiconque met la main sur le poste |
| Critique | Base de données de santé sur un moteur ancien, non maintenu | Plus de correctifs de sécurité |
| Critique | Sauvegardes présentes mais **jamais testées en restauration** | Fausse sécurité : aucune garantie de récupérer les données |
| Critique | Hébergement des données de santé via une solution non conforme HDS | Non-conformité réglementaire directe |
| Important | Accès distant (RDP) exposé sur le réseau, durcissement non vérifié | Porte d'entrée pour un attaquant |
| Important | Partages SMB exposés sur plusieurs machines | Propagation d'un poste à l'autre |
| Important | Imprimante et stockage réseau insuffisamment protégés | Accès non maîtrisé aux documents |
| Moyen | Journalisation du pare-feu désactivée | Aucune trace en cas d'incident |
| Moyen | Comptes à droits trop larges (à vérifier), bloatware | Surface d'attaque inutile |
| Moyen | Hygiène physique : infos sensibles visibles, post-it, clés USB non contrôlées | Fuite par simple observation |
| Moyen | Poste en salle d'attente, accessible physiquement | Accès direct pour un visiteur |

## Bons points

Un audit honnête ne fait pas que faire peur, il reconnaît ce qui va :

- Compte administrateur intégré désactivé
- Antivirus professionnel présent
- Clé Wi-Fi robuste

## Livrables

- Rapport d'audit complet
- Plan de remédiation priorisé et chiffré
- Devis de remédiation séparé

> [!IMPORTANT]
> Rapport complet et preuves : communicables en entretien, uniquement avec l'accord du client.
