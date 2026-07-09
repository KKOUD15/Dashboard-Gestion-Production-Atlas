SOLUTION SIMPLE POUR POWER BI
1. Dans Power BI Desktop : Accueil > Obtenir les données > Excel.
2. Sélectionner le fichier : Atlas_Irrigation_Tech_SOURCE_POWERBI_PROPRE.xlsx.
3. Cocher uniquement les tables PBI_*.
4. Cliquer sur Charger. Normalement, il ne doit plus y avoir de lignes nulles décoratives.
5. Utiliser PBI_ARTICLES comme table centrale.
6. Créer les relations :
   - PBI_ARTICLES[Code_Article] -> PBI_ABC[Code_Article]
   - PBI_ARTICLES[Code_Article] -> PBI_STOCK_SECURITE[Code_Article]
   - PBI_ARTICLES[Code_Article] -> PBI_ALERTES[Code_Article]
   - PBI_ARTICLES[Code_Article] -> PBI_WILSON[Code_Article]
   - PBI_ARTICLES[Fournisseur_Principal] -> PBI_FOURNISSEURS[Fournisseur]
   - PBI_ARTICLES[Code_Article] -> PBI_HISTORIQUE[Code_Article]
   - PBI_ARTICLES[Code_Article] -> PBI_PREVISIONS[Code_Article]
7. Pour le PDP et le CBN/MRP, les tables sont déjà au format long exploitable directement dans les graphiques.
