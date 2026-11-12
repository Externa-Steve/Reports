  titre: "Audit de sécurité réseau — cabinet médical"
  type: cas-client
  secteur: santé (cabinet médical)
  annee: 2026
  role: auditeur sécurité (mission réelle, client anonymisé)
  statut: livré



                    # Cas client 01


  Audit de sécurité d'un cabinet médical
Mission réelle réalisée pour un cabinet médical en 2026.
Client anonymisé (données de santé — secret médical + RGPD art. 9).
Preuves et rapport complet disponibles sur demande, en entretien.

  Le contexte :
Petit cabinet médical (~5 postes de travail, 1 serveur de stockage réseau,1 imprimante réseau, box opérateur grand public). 
Le poste principal manipule des données de santé de patients via un logiciel métier et une base de données locale. 

  Enjeu fort : 
secret médical, RGPD (article 9), continuité de l'activité de soins.
Le cabinet n'avait jamais fait auditer son informatique. 

  Ma mission : 
Évaluer le niveau de sécurité réel du poste de travail sensible 
et du réseau local, puis livrer des actions correctives priorisées, compréhensibles par un non-informaticien.

  Ma démarche (ce que j'ai fait, étape par étape)
1. Reconnaissance OSINT, recherche de l'exposition publique du cabinet et de son personnel (données qui traînent en ligne, surface d'attaque externe).
2. Cartographie réseau découverte des hôtes puis scan de ports (outils en mode prudent pour ne pas perturber l'activité), identification des services exposés sur le réseau local.
3. Audit du poste sensible sur site, inspection de la configuration Windows (pare-feu, antivirus, comptes, mises à jour, accès distants) en ligne de commande.
4. Rédaction du rapport classement des constats par criticité (critique / important / moyen) avec, pour chacun, le risque métier expliqué simplement.
5. Plan de remédiation actions à faire sous 24-48h, cette semaine, ce mois. 

  Résultats clés (anonymisés) 
  Constats remontés, hiérarchisés par risque réel pour le cabinet 
Critique: pare-feu du poste désactivé, mot de passe Wi-Fi récupérable en clair, base de données de santé hébergée sur un moteur ancien non maintenu (plus de correctifs.
Critique: sauvegardes présentes mais jamais testées en restauration : fausse sécurité, aucune garantie de récupérer les données en cas d'incident.
Critique: conformité données de santé hébergées via une solution non  conforme aux exigences d'hébergement de données de santé (HDS) non-conformité réglementaire directe.
Important: accès distant (RDP) exposé sur le réseau sans durcissement vérifié, partages de fichiers (SMB) exposés sur plusieurs machines => risque de propagation d'une attaque de poste à poste, imprimante et serveur de stockage accessibles sans protection suffisante.
Moyen: journalisation du pare-feu désactivée (aucune trace en cas d'incident), comptes à droits trop larges à vérifier, bloatware à nettoyer, hygiène physique (informations sensibles visibles sur les écrans, en post-it, pas de verification pour les clés usb client).
Moyen: poste en salle d'attente vulnerable et accessible physiquement.

J'ai aussi noté les bons points existants (compte administrateur intégré désactivé, antivirus professionnel présent, clé Wi-Fi robuste) 
un audit honnête ne fait pas que faire peur, il reconnaît ce qui va.

  Livrables produits
Rapport d'audit complet
Plan de remédiation priorisé et chiffré
Devis de remédiation séparé


