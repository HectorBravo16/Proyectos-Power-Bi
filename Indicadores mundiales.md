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

La idea de estas tablas era obtener insights en español y la "dificultad" estaba en que en la tabla de población los paises estaban en inglés. Simplemente había que sacar las relaciones con las otras dos tablas.

### Tabla Esperanza de vida

| Country             | Life Expectancy |
|---------------------|-----------------|
| Afghanistan         | 51.3            |
| Albania             | 78.3            |
| Algeria             | 76.8            |
| American Samoa      | 75.4            |
| Andorra             | 82.8            |
| Angola              | 56.0            |
| Antigua and Barbuda | 76.5            |
| Argentina           | 77.1            |
| Armenia             | 74.6            |
| Aruba               | 76.8            |

### Tabla Mortalidad infantil

| Country             | Infant Mortality |
|---------------------|------------------|
| Afghanistan         | 163.07           |
| Albania             | 21.52            |
| Algeria             | 31.00            |
| American Samoa      | 9.27             |
| Andorra             | 4.05             |
| Angola              | 191.19           |
| Antigua and Barbuda | 19.46            |
| Argentina           | 15.18            |
| Armenia             | 23.28            |
| Aruba               | 5.89             |

## Nuevas columnas, métricas, Bookmarks y estética
Una vez los datos estaban listos, para cumplir con los objetivos era necesario crear algunas métricas sencillas (promedios, máximos y mínimos) y columnas de grupos (grupos de población, mortalidad, esperanza de vida) mediante DAX.

## Proyecto terminado
Lo mejor para entender todas las visualizaciones es navegar por ellas, filtrar por las diferentes opciones que hay y sacar conclusiones. Algunas preguntas que nos hemos propuesto son:
1. ¿Hay relación entre una alta mortalidad infantil y una baja esperanza de vida?
2. ¿Influye la cantidad de población en alguno de estos 2 indicadores?

El reporte completo está subido a powerbi.com. El enlace para verlo es este: https://app.powerbi.com/view?r=eyJrIjoiNzQyNjUyYzctZGZiOC00YjY2LThjOTMtZmJlMGYyNTMwZmNiIiwidCI6Ijg3YmNjZDBkLTdiMjUtNGUzZC04OWZiLWMyYWI5M2E2OGVjOCIsImMiOjh9
