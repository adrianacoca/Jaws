# Jaws
 ![Jaws.jpg](/Images/Jaws.jpg)  
# DataCleaning.csv
 
## Data Cleaning - Limpiando los datos: 
**1. Columnas validas**
Analisis del el numero de datos NaN por columna:  
Unnamed 22 & Unnamed 23 ---> no tenian datos ---> eliminando...  

**2. Filas validas**
Eliminando aquellas filas que contengan NaN en las columnas de la lista:   interested_columns=['Date', 'Year', 'Type', 'Country', 'Area', 'Location', 'Activity', 'Name', 'Sex ', 'Age', 'Injury', 'Fatal (Y/N)', 'Time', 'Species ']
Eliminando 19000 filas...   

**3. Renombrando columnas**
Modificando las columnas 'Sex ', 'Species ', 'Fatal (Y/N)' para eliminar caracteres como espacios, parentesis...  

## Data Reading - Leyendo los datos: 
**1. Año**  
Datos validos?  ✅  
**2. País**  
Datos validos?  ✅  
**3. Area**  
Datos validos?  ✅  
**4. Hora**  
Datos validos?  ✅  
**5. Fatalidad**  
Datos validos?  ✅  
**6. Tipos de Ataques**  
Datos validos?  ✅  
**7. Tipo de lesión**  
Datos validos?  ❌  
**8. Actividad**  
Datos validos?  ❌  
**9. Especie**  
Datos validos?  ❌  

Exportando datos...  

Horizontal Rule

---
# DataAnalysing.csv  

### Hipótesis 1
### Relación entre gravedad del ataque y país  
Los países con más casos de ataques son: 
![top_country_attacks](/Images/top_country_attacks.png)  
**RESULTADO: Los países con ataques más mortales no son aquellos en los que se produce más ataques** 
 ![death_ratio_country](/Images/death_ratio_country.png)  
Reflexión: Puede que esto se deba a que los países con probabilidad de muertes más alta registre menos datos, por lo tanto es más probable que registre un caso sólo si la victima ha muerto.   

### Hipótesis 2
### El ratio de muertes y ataques provocados/no provocados  
El ratio de muertes en ataques provocados es: 0.0335  
El ratio de muertes en ataques no provocados es: 0.2605 !!!   
**RESULTADO: Los ataques no provocados son más mortales**   
Reflexión: Sólo se han registrado 574 ataques provocados y 4595 ataques no provocados. Por lo tanto es posible que la muestra de ataques provocados no sea tán fiable como aquella de ataques no provocados.   
  
### Hipótesis 3  
### Relación entre la hora del ataque y si es provocado  
 ![hambre](/Images/hambre.png)  
**RESULTADO: Es más probable que un ataque sea provocado por la noche**     
* Ratio de ataques provodados por la mañana : 0.066   
* Ratio de ataques provodados por la medio día : 0.062   
* Ratio de ataques provodados por la tarde : 0.068   
* Ratio de ataques provodados por la noche : 0.081 