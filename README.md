# Jaws

# Limpiar Limpiar Limpiar

Al abrir la base de datos de 'attacks.csv', resultó ser una base de datos en la que había muchos datos vacíos. 

Creando la definición:  
`def valid_columns(x):
    y=x.isnull().sum().sort_values(ascending=False)
    return y`
para poder ver qué columnas eran las que estaban más vacías

**RESULTADOS !!**

Número de filas           25723              Ratio de datos 

Unnamed: 22               25722         -->  0.0000388757143412     Datos prácticamente inexistentes 🚨
Unnamed: 23               25721         -->  0.0000777514286825      Datos prácticamente inexistentes 🚨
Time                      22775         -->  0.11460560587800801   
Species                   22259         -->  0.13466547447809354 
Age                       22252         -->  0.1349376044784823
Sex                       19986         -->  0.2230299731757571
Activity                  19965         -->  0.22384636317692339
Location                  19961         -->  0.22400186603428837
Fatal (Y/N)               19960         -->  0.22404074174862962
Area                      19876         -->  0.22730630175329472
Name                      19631         -->  0.23683085176690122
Country                   19471         -->  0.24305096606150137
Injury                    19449         -->  0.2439062317770089
Investigator or Source    19438         -->  0.24433386463476267
Type                      19425         -->  0.24483924892119893
Year                      19423         -->  0.24491700034988143
href formula              19422         -->  0.24495587606422267
pdf                       19421         -->  0.24499475177856392
href                      19421         -->  0.24499475177856392
Case Number.1             19421         -->  0.24499475177856392
Case Number.2             19421         -->  0.24499475177856392
Date                      19421         -->  0.24499475177856392
original order            19414         -->  0.2452668817789527
Case Number               17021         -->  0.33829646619756637

Despues de borrar las columnas vacías 'Unnamed 22' y 'Unnamed 23', escojí las columnas con los datos que más me interesaban 
*'Date' 
*'Year' 
*'Type'
*'Country' 
*'Area' 
*'Location'
*'Activity' 
*'Name' 
*'Sex '
*'Age'
*'Injury' 
*'Fatal (Y/N)'
*'Time'
*'Species '

**Despues de limpiar aquellas filas que apenas tenían datos, estos eran los resultados de NaN en cada columna:**

*Time                      3354
*Species                   2838
*Age                       2831
*Sex                        565
*Activity                   544
*Location                   540
*Fatal (Y/N)                539
*Area                       455
*Name                       210
*Country                     50
*Injury                      28
*Investigator or Source      17
*Type                         4
*Year                         2
*Case Number                  1
*href formula                 1
*Case Number.2                0
*pdf                          0
*href                         0
*Case Number.1                0
*Date                         0
*original order               0


Posibles hipotesis: 
concentración de accidentes en cada pais (por area)
fatalidad por area --> especie de tiburón 