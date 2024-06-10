# TAS9- FUNCIONES AGREGACION 

### 1. Obtener la edad promedio de los miembros:
- Sentencia:
```
SELECT AVG (age) AS edad_promedio
FROM member;
```

- Captura

<img src="./TAS9-capturas/Pasted image 20240610130105.png" alt="drawing0" width="500"/>

 ### 2. Obtener la edad mínima de los miembros:
---
- Sentencia:
```
SELECT MIN (age) AS edad_min
FROM member;
```

- Captura
<img src="./TAS9-capturas/Pasted image 20240610130234.png" alt="drawing0" width="500"/>


### 3. Obtener el número total de registros asistidos:
---
- Sentencia:
```
SELECT COUNT (*) AS total_registros
FROM register;
```

- Captura
<img src="./TAS9-capturas/Pasted image 20240610130633.png" alt="drawing0" width="500"/>

### 4. Obtener el número total de asistentes a todas las conferencias
---
- Sentencia:
```
SELECT SUM (total_attendees) AS total_asistentes
FROM conference;
```

- Captura
<img src="./TAS9-capturas/Pasted image 20240610130950.png" alt="drawing0" width="500"/>

### 5. Obtener el número total de eventos por cada ciudad:
---
- Sentencia:
```
SELECT city, COUNT (*) AS total_evento
FROM event
GROUP BY city;
```

- Captura
<img src="./TAS9-capturas/Pasted image 20240610131240.png" alt="drawing0" width="500"/>

### 6. Obtener el número de registros por cada miembro:
---
- Sentencia:
```
SELECT member_id, COUNT(*) AS total_registros
FROM register
GROUP BY member_id;
```

- Captura
<img src="./TAS9-capturas/Pasted image 20240610131506.png" alt="drawing0" width="500"/>

### 7. Obtener el número de registros por cada conferencia: 
---
- Sentencia:
```
SELECT conference_id, COUNT(*) AS total_registros
FROM register
GROUP BY conference_id;
```

- Captura
<img src="./TAS9-capturas/Pasted image 20240610131721.png" alt="drawing0" width="500"/>
