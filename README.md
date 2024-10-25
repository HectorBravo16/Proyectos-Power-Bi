# Proyectos-Power-Bi
En este archivo readme describiré los distintos proyectos realizados en Power BI a modo de portfolio.
# Reporte de recursos humanos
El objetivo era visualizar indicadores de Colaboradores, Sueldos y Desempeño en un mismo reporte de recursos humanos para una compañía inventada (SKU-DON). La idea es poder compartir este reporte por enlace web.

## Objetivos particulares
1. Análisis de todos los parámetros de cada empleado mediante una tabla.
2. Conteos varios (empleados por cada estado, por cada departamento, etc).
3. Promedios de edad, sueldo y desempeño calculados mediante métricas.
4. Deducir relación sueldo-edad por medio de un gráfico de dispersión.
5. Máximo y mínimo de desempeño agrupado por jefes.

## Tablas iniciales
Se parten de 3 tablas que se muestran a continuación. Cada una de ellas tiene 195 filas.

### Tabla Empleados
| ID Empleado   | Nombre Empleado      | Estado                          | Nacimiento   | Género  | Departamento  | Posición         | Nombre Jefe  |
| ------------- | -------------------- | -------------------------------- | ------------ | ------- | ------------- | ---------------- | ------------ |
| 1102024149    | Spirea, Kelley        | California, Estados Unidos       | 28/09/1980   | Female  | Admin Offices | Administrative II| Elijah Gray  |
| 1001109612    | Darson, Jene'ya       | California, Estados Unidos       | 10/05/1983   | Female  | Admin Offices | Administrative II| Elijah Gray  |
| 1000974650    | Stanley, David        | Texas, Estados Unidos            | 16/12/1975   | Male    | Admin Offices | Manager          | Debra Houlihan|
| 1206043417    | Quinn, Sean           | Massachusetts, Estados Unidos    | 10/06/1969   | Male    | Admin Offices | Manager          | Janet King   |
| 1307060188    | Boutwell, Bonalyn     | California, Estados Unidos       | 02/04/1972   | Female  | Admin Offices | Manager          | Elijah Gray  |
| 1011022932    | Hendrickson, Trina    | California, Estados Unidos       | 26/08/1977   | Female  | Admin Offices | Administrative II| Elijah Gray  |
| 1101023619    | Wallace, Theresa      | California, Estados Unidos       | 06/02/1985   | Female  | Admin Offices | Administrative II| Elijah Gray  |
| 1107027575    | LeBel, Jonathan R.    | California, Estados Unidos       | 17/10/1986   | Male    | Admin Offices | Administrative II| Elijah Gray  |
| 1102024115    | LeBlanc, Brandon      | Massachusetts, Estados Unidos    | 05/10/1969   | Male    | Admin Offices | Manager          | Janet King   |
| 1105026041    | Gaul, Barbara         | California, Estados Unidos       | 11/02/1968   | Female  | Admin Offices | Administrative II| Elijah Gray  |

### Tabla Evaluación
| ID Empleado   | Evaluación |
| ------------- | -----------|
| 1307060199    | 5,91       |
| 1011022883    | 9,46       |
| 1501072311    | 5,70       |
| 1304055947    | 7,21       |
| 1107027358    | 5,99       |
| 1212051409    | 6,25       |
| 1212052023    | 9,35       |
| 1307060083    | 5,06       |
| 1303054329    | 7,24       |
| 1403066194    | 7,80       |

### Tabla Sueldo
| ID Empleado   | Sueldo |
| ------------- | ------ |
| 1205033102    | 26536  |
| 1211051232    | 27684  |
| 1204032927    | 28153  |
| 1308060366    | 28865  |
| 1408069882    | 29135  |
| 1202031618    | 30150  |
| 1001735072    | 30600  |
| 1011022887    | 31152  |
| 1304055987    | 32015  |
| 1107027392    | 32400  |

## Transformación de datos
La ETL de este proyecto es muy básica, pues no es el objetivo principal, pero en muchos casos siempre queda alguna transformación que hacer mediante Power Query.

## Tablas de Sueldo y Evaluación
Las transformaciónes aquí eran muy básicas. Simplemente había que quitar el encabezado y cambiar el formato de la columna "ID empleado" a números enteros.

## Tabla de Empleados
A parte del encabezado, aquí se han hecho más transformaciónes. En primer lugar se han traducido los géneros del inglés al español. A continuación, la columna "nombre empleado" pasó a tener formato "nombre apellido". Por último, la columna de "estado" se editó eliminando "Estados Unidos", pues aparecía en todas las filas y no aportaba información relevante.

## Nuevas columnas, métricas, Bookmarks y estética
Una vez los datos estaban listos, para cumplir con los objetivos era necesario crear algunas métricas sencillas (promedios, máximos y mínimos) y columnas de grupos (grupos de edad, de salario, evaluación) mediante DAX. Se han creado tambien botones para navegar entre páginas y se han importado tanto temas nuevos como un fondo propio de la empresa fictícea.

## Proyecto terminado
Lo mejor para entender todas las visualizaciones es navegar por ellas, filtrar por las diferentes opciones que hay y sacar conclusiones. Algunas preguntas que nos hemos propuesto son:
1. ¿En qué grupo de edad trabaja más gente? ¿Es este mismo grupo al que más salario se le dedica?
2. ¿Qué departamento tiene un mejor salario promedio?
3. ¿Hay relación entre la evaluación de un empleado y su salario? ¿Y entre la edad y el salario?
4. ¿Hay brecha salarial en esta empresa?

El reporte completo está subido a powerbi.com. El enlace para verlo es este: https://app.powerbi.com/view?r=eyJrIjoiYjJlNTQwZTMtYWY0NC00NTJhLTlkNjMtZjhmODhmM2I1YmZhIiwidCI6Ijg3YmNjZDBkLTdiMjUtNGUzZC04OWZiLWMyYWI5M2E2OGVjOCIsImMiOjh9 
