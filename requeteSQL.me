# Requêtes MySQL pour le Projet Coffee Shop Sales

Ce projet consiste à analyser les ventes d'un coffee shop à l'aide de requêtes MySQL. L'objectif est de convertir, transformer et analyser les données afin d'extraire des informations clés sur les performances des ventes.

## Pré-traitement des données

### Conversion des Colonnes de Date et Heure

1. **Conversion de la colonne ****`transaction_date`**** au format date**

```sql
UPDATE coffee_shop_sales
SET transaction_date = STR_TO_DATE(transaction_date, '%d-%m-%Y');
```

2. **Modification du type de données de la colonne ****`transaction_date`**

```sql
ALTER TABLE coffee_shop_sales
MODIFY COLUMN transaction_date DATE;
```

3. **Conversion de la colonne ****`transaction_time`**** au format heure**

```sql
UPDATE coffee_shop_sales
SET transaction_time = STR_TO_DATE(transaction_time, '%H:%i:%s');
```

4. **Modification du type de données de la colonne ****`transaction_time`**

```sql
ALTER TABLE coffee_shop_sales
MODIFY COLUMN transaction_time TIME;
```

### Renommage des Colonnes

- Correction du nom de la colonne `ï»¿transaction_id` en `transaction_id`

```sql
ALTER TABLE coffee_shop_sales
CHANGE COLUMN `ï»¿transaction_id` transaction_id INT;
```

## Analyse des KPI

### Ventes Totales

- Calcul des ventes totales pour le mois de mai (CM-May)

```sql
SELECT ROUND(SUM(unit_price * transaction_qty)) as Total_Sales
FROM coffee_shop_sales
WHERE MONTH(transaction_date) = 5;
```

### Croissance Mensuelle des Ventes (MOM)

```sql
SeFROM
    coffee_shop_sales
WHERE
    MONTH(transaction_date) IN (4, 5)
GROUP BY
    MONTH(transaction_date)
ORDER BY
    MONTH(transaction_date);
```

### Commandes Totales

- Calcul du nombre total de commandes pour mai

```sql
SELECT COUNT(transaction_id) as Total_Orders
FROM coffee_shop_sales
WHERE MONTH(transaction_date) = 5;
```

### Croissance Mensuelle des Commandes

```sql
SELECT
    MONTH(transaction_date) AS month,
    ROUND(COUNT(transaction_id)) AS total_orders,
    (COUNT(transaction_id) - LAG(COUNT(transaction_id), 1)
    OVER (ORDER BY MONTH(transaction_date))) / LAG(COUNT(transaction_id), 1)
    OVER (ORDER BY MONTH(transaction_date)) * 100 AS mom_increase_percentage
FROM
    coffee_shop_sales
WHERE
    MONTH(transaction_date) IN (4, 5)
GROUP BY
    MONTH(transaction_date)
ORDER BY
    MONTH(transaction_date);
```

### Quantité Totale Vendue

```sql
SELECT SUM(transaction_qty) as Total_Quantity_Sold
FROM coffee_shop_sales
WHERE MONTH(transaction_date) = 5;
```

### Croissance Mensuelle de la Quantité Vendue

```sql
SELECT
    MONTH(transaction_date) AS month,
    ROUND(SUM(transaction_qty)) AS total_quantity_sold,
    (SUM(transaction_qty) - LAG(SUM(transaction_qty), 1)
    OVER (ORDER BY MONTH(transaction_date))) / LAG(SUM(transaction_qty), 1)
    OVER (ORDER BY MONTH(transaction_date)) * 100 AS mom_increase_percentage
FROM
    coffee_shop_sales
WHERE
    MONTH(transaction_date) IN (4, 5)
GROUP BY
    MONTH(transaction_date)
ORDER BY
    MONTH(transaction_date);
```

## Tableau de Bord Journalier

- Calcul des ventes, quantité et commandes pour une journée spécifique

```sql
SELECT
    SUM(unit_price * transaction_qty) AS total_sales,
    SUM(transaction_qty) AS total_quantity_sold,
    COUNT(transaction_id) AS total_orders
FROM
    coffee_shop_sales
WHERE
    transaction_date = '2023-05-18';
```


