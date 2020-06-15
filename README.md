# Jaws

# DataCleaning.csv

## Data Cleaning - Limpiando los datos: 
**1. Columnas validas**
Analisis del el numero de datos NaN por columna:  
Unnamed 22 & Unnamed 23 ---> no tenian datos ---> eliminando...  

**2. Filas validas**
Eliminando aquellas filas que contengan NaN en las columnas de la lista interested_columns=['Date', 'Year', 'Type', 'Country', 'Area', 'Location', 'Activity', 'Name', 'Sex ', 'Age', 'Injury', 'Fatal (Y/N)', 'Time', 'Species ']
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

