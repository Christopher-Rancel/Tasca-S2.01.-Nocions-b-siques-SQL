## Descripció

En aquest exercici he utilitzat JOIN per combinar les dues taules (`company` i `transaction`) i obtenir informació sobre les vendes.

L’objectiu és analitzar des de quins països es generen les vendes, saber quants països diferents hi participen i identificar quina empresa té la mitjana més alta de vendes.

---

## Llistat dels països que estan generant vendes

En aquesta consulta he unit les dues taules per obtenir el país associat a cada transacció.

He utilitzat `DISTINCT` per evitar que els països es repeteixin.

```sql
-- Llistat dels països que estan generant vendes
SELECT DISTINCT country
FROM transaction AS t
JOIN company AS c
    ON t.company_id = c.id;
```

---

## Des de quants països es generen les vendes

En aquest cas he volgut saber el nombre total de països diferents que generen vendes.

Per fer-ho he utilitzat `COUNT(DISTINCT country)` per comptar només els països únics.

```sql
-- Des de quants països es generen les vendes
SELECT COUNT(DISTINCT country) AS total_paisos
FROM transaction AS t
JOIN company AS c
    ON t.company_id = c.id;
```

---

## Identifica la companyia amb la mitjana més gran de vendes

En aquesta consulta he calculat la mitjana de l’import de les transaccions per empresa utilitzant `AVG(amount)`.

Després he agrupat per `company_name` amb `GROUP BY`, he ordenat els resultats de major a menor amb `ORDER BY` i finalment he utilitzat `LIMIT 1` per mostrar només l’empresa amb la mitjana més alta.

```sql
-- Identifica la companyia amb la mitjana més gran de vendes
SELECT company_name, ROUND(AVG(t.amount), 2) AS mitjana_vendes
FROM transaction AS t
JOIN company AS c
    ON t.company_id = c.id
GROUP BY company_name
ORDER BY mitjana_vendes DESC
LIMIT 1;
```
