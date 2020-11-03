# Modele-de-scoring
l'objectif est de fournir un modèle fiable de détection de défaut de crédit. le modèle doit rester interprétable afin de pouvoir comprendre les mécanismes d’octroi de crédit

Les données sont fournies par Home Credit, un service dédié à l'octroi de lignes de crédit (prêts) à la population non bancarisée. Prévoir si un client va ou non rembourser un prêt ou s'il a des difficultés est un besoin essentiel des entreprises. Home Credit organise ce concours sur Kaggle pour voir quels types de modèles la communauté d'apprentissage machine peut développer pour l'aider dans cette tâche.

Il existe 7 sources de données différentes :

   * application_train/application_test : les principales données de formation et de test avec des informations sur chaque demande de prêt auprès de Home Credit. Chaque prêt a sa propre ligne et est identifié par la caractéristique SK_ID_CURR. Les données relatives aux demandes de formation sont accompagnées de la mention TARGET indiquant 0 : le prêt a été remboursé ou 1 : le prêt n'a pas été remboursé.
   * bureau : données concernant les crédits antérieurs du client auprès d'autres institutions financières. Chaque crédit précédent a sa propre ligne dans bureau, mais un prêt dans les données de demande peut avoir plusieurs crédits précédents.
   * bureau_balance : données mensuelles concernant les crédits précédents en bureau. Chaque ligne correspond à un mois d'un crédit antérieur, et un seul crédit antérieur peut avoir plusieurs lignes, une pour chaque mois de la durée du crédit.
   * previous_application : demandes précédentes de prêts au crédit immobilier des clients dont les données de demande contiennent des prêts. Chaque prêt actuel dans les données de demande peut avoir plusieurs prêts précédents. Chaque demande précédente comporte une ligne et est identifiée par la caractéristique SK_ID_PREV.
   * POS_CASH_BALANCE : données mensuelles sur les prêts antérieurs au point de vente ou en espèces que les clients ont contractés auprès de Home Credit. Chaque ligne correspond à un mois d'un précédent prêt sur le lieu de vente ou en espèces, et un seul prêt précédent peut comporter plusieurs lignes.
   * credit_card_balance : données mensuelles sur les cartes de crédit que les clients ont utilisées précédemment dans le cadre du crédit immobilier. Chaque ligne correspond à un mois de solde de carte de crédit, et une seule carte de crédit peut comporter plusieurs lignes.
   * installments_payment : historique des paiements pour les prêts précédents au Crédit immobilier. Il y a une ligne pour chaque paiement effectué et une ligne pour chaque paiement manqué.
