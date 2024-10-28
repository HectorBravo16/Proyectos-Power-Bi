# Reportes de población e indicadores mundiales
El objetivo era visualizar datos de población por pais y continente, a la vez que visualizar indicadores de esperanza de vida y mortalidad infantil. Es un proyecto relativamente simple y de bajo nivel, cuya única finalidad es iniciarse en Power BI y familiarizarse con indicadores, tarjetas y alguna medida simple.

## Objetivos particulares
1. Analizar los datos por distintas categorías (continente, grupos de población por cantidad, grupos de esperanza de vida y grupos de mortalidad infantil).
2. Deducir una relación entre la esperanza de vida y la mortalidad infantil.

## Tablas iniciales
Para el reporte de población, partíamos de 3 tablas

### Tabla Countries
| Country Code | Country                  | Continent |
|--------------|--------------------------|-----------|
| DZA          | Algeria                  | Africa    |
| AGO          | Angola                   | Africa    |
| BEN          | Benin                    | Africa    |
| BWA          | Botswana                 | Africa    |
| BFA          | Burkina Faso             | Africa    |
| BDI          | Burundi                  | Africa    |
| CPV          | Cabo Verde               | Africa    |
| CMR          | Cameroon                 | Africa    |
| CAF          | Central African Republic | Africa    |
| TCD          | Chad                     | Africa    |

### Tabla Paises
| Codigo Pais | País                      | Continente |
|-------------|---------------------------|------------|
| DZA         | Argelia                   | África     |
| AGO         | Angola                    | África     |
| BEN         | Benín                     | África     |
| BWA         | Botsuana                  | África     |
| BFA         | Burkina Faso              | África     |
| BDI         | Burundi                   | África     |
| CPV         | Cabo Verde                | África     |
| CMR         | Camerún                   | África     |
| CAF         | República Centroafricana   | África     |
| TCD         | Chad                      | África     |

### Tabla Population
| Country             | Population |
|---------------------|------------|
| Afghanistan         | 34,656,032 |
| Albania             | 2,876,101  |
| Algeria             | 40,606,052 |
| American Samoa      | 55,599     |
| Andorra             | 77,281     |
| Angola              | 28,813,463 |
| Antigua and Barbuda | 100,963    |
| Argentina           | 43,847,430 |
| Armenia             | 2,924,816  |
| Aruba               | 104,822    |

La idea de estas tablas era obtener insights en español y la "dificultad estaba en que en la tabla de población los paises estaban en inglés. Simplemente había que sacar las relaciones con las otras dos tablas.




## Nuevas columnas, métricas, Bookmarks y estética
Una vez los datos estaban listos, para cumplir con los objetivos era necesario crear algunas métricas sencillas (promedios, máximos y mínimos) y columnas de grupos (grupos de edad, de salario, evaluación) mediante DAX. Se han creado tambien botones para navegar entre páginas y se han importado tanto temas nuevos como un fondo propio de la empresa fictícea.

## Proyecto terminado
Lo mejor para entender todas las visualizaciones es navegar por ellas, filtrar por las diferentes opciones que hay y sacar conclusiones. Algunas preguntas que nos hemos propuesto son:
1. ¿En qué grupo de edad trabaja más gente? ¿Es este mismo grupo al que más salario se le dedica?
2. ¿Qué departamento tiene un mejor salario promedio?
3. ¿Hay relación entre la evaluación de un empleado y su salario? ¿Y entre la edad y el salario?
4. ¿Hay brecha salarial en esta empresa?

El reporte completo está subido a powerbi.com. El enlace para verlo es este: https://app.powerbi.com/view?r=eyJrIjoiYjJlNTQwZTMtYWY0NC00NTJhLTlkNjMtZjhmODhmM2I1YmZhIiwidCI6Ijg3YmNjZDBkLTdiMjUtNGUzZC04OWZiLWMyYWI5M2E2OGVjOCIsImMiOjh9 
