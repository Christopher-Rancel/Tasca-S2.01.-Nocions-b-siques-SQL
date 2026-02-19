# Sprint SQL – Bases de Dades Relacionals

En aquest sprint es repassen les nocions bàsiques per a l’ús de bases de dades relacionals.

L’objectiu és iniciar l’experiència pràctica treballant amb una base de dades que conté informació d’una empresa dedicada a la venda de productes en línia.

Durant l’activitat es treballarà amb dades relacionades amb:

- Les transaccions efectuades
- La informació corporativa de les empreses participants

---

# Nivell_1

## Exercici_1

A partir dels documents adjunts (`estructura_dades` i `dades_introduir`), s’importen les dues taules.

Cal:

- Mostrar les característiques principals de l’esquema creat  
- Explicar les diferents taules i variables que existeixen  
- Incloure un diagrama que il·lustri la relació entre les taules i variables  

---

## Exercici_2

Utilitzant **JOIN**, realitzar les següents consultes:

- Llistat dels països que estan generant vendes  
- Des de quants països es generen les vendes  
- Identificar la companyia amb la mitjana més gran de vendes  

---

## Exercici_3

Utilitzant només **subconsultes** (sense utilitzar JOIN):

- Mostrar totes les transaccions realitzades per empreses d’Alemanya  
- Llistar les empreses que han realitzat transaccions amb un `amount` superior a la mitjana de totes les transaccions  
- Eliminar del sistema les empreses que no tenen transaccions registrades i mostrar el llistat d’aquestes empreses  

---

# Nivell_2

## Exercici_1

Identificar els cinc dies en què es va generar la quantitat més gran d’ingressos per vendes.

Mostrar:

- La data de cada transacció  
- El total de vendes  

---

## Exercici_2

Calcular la mitjana de vendes per país.

Presentar els resultats ordenats de major a menor mitjana.

---

## Exercici_3

Es planteja un nou projecte per llançar campanyes publicitàries per competir amb la companyia **"Non Institute"**.

Es demana:

- Llistat de totes les transaccions realitzades per empreses situades en el mateix país que aquesta companyia  

Mostrar el llistat:

- Aplicant JOIN i subconsultes  
- Aplicant només subconsultes  

---

# Nivell_3

## Exercici_1

Presentar:

- Nom  
- Telèfon  
- País  
- Data  
- Amount  

D’aquelles empreses que van realitzar transaccions amb un valor comprès entre **350 i 400 euros** en alguna de les següents dates:

- 29 d’abril del 2015  
- 20 de juliol del 2018  
- 13 de març del 2024  

Ordenar els resultats de major a menor quantitat.

---

## Exercici_2

Es necessita optimitzar l’assignació de recursos segons la capacitat operativa requerida.

Cal mostrar la informació sobre la quantitat de transaccions que realitza cada empresa i indicar si:

- Té més de 400 transaccions  
- Té menys de 400 transaccions  
