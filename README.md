# Microsoft Fabric - Datawarehouse Analyseproject

Dit project is een oefening waarin we een relationele datawarehouse in Microsoft Fabric opzetten, data laden, analyseren en visualiseren.

## 📌 Wat hebben we gedaan?

1. **Workspace aangemaakt**
   - Een nieuwe Fabric-werkruimte is aangemaakt met proeflicentie.
   - Deze werkruimte is de basis voor alle verdere stappen.

2. **Datawarehouse aangemaakt**
   - Een nieuwe datawarehouse is gemaakt in de werkruimte.
   - Hiermee kunnen we volledige SQL-query’s uitvoeren (inclusief INSERT, UPDATE, DELETE).

3. **Tabelstructuur opgezet**
   - Een `DimProduct`-tabel is aangemaakt met T-SQL.
   - Vervolgens zijn er meerdere records in deze tabel ingevoerd.
   - Daarna zijn extra tabellen toegevoegd via een SQL-script:
     - `DimCustomer`
     - `DimDate`
     - `FactSalesOrder`

4. **Relaties gedefinieerd**
   - Relaties tussen de feitentabel en dimensietabellen zijn ingesteld:
     - `FactSalesOrder.ProductKey → DimProduct.ProductKey`
     - `FactSalesOrder.CustomerKey → DimCustomer.CustomerKey`
     - `FactSalesOrder.SalesOrderDateKey → DimDate.DateKey`

5. **SQL-query’s uitgevoerd**
   - Aggregaties van omzet per jaar, maand en regio werden opgehaald met `GROUP BY` en `JOIN`.
   - Een `VIEW` genaamd `vSalesByRegion` werd aangemaakt om deze analyse te bewaren.

6. **Visuele query gebouwd**
   - Een grafische query werd gemaakt met behulp van de visuele editor.
   - Filter toegepast op één specifiek product (“Cable Lock”) om een gerichte analyse te doen.

7. **Visualisatie gemaakt in rapport**
   - Niet-relevante kolommen verborgen voor rapportage.
   - Een Power BI rapport is aangemaakt met een geclusterde staafdiagram van verkoop per productcategorie.
   - Rapport is opgeslagen als **Sales Report**.

## 📂 Inhoud van de werkruimte

- 📦 Datawarehouse
- 🧠 Semantisch model
- 📊 Power BI rapport: **Sales Report**

# Analyze-data-in-a-data-warehouse
