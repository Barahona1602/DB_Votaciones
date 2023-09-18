# DB_Votaciones
| Nombre   |Carnet   |
|----------|---------|
| Pablo Josué Barahona Luncey  | 202109715   |

Esta es una base de datos sobre las elecciones de Guatemala del año 2023 a la cual tiene como finalidad poder acceder a los datos de una manera precisa y filtrada para poder obtener precisión. 
Al momento de hacer consultas la estructura del proyecto está establecida con una Api Rest creada en Fast Api con Python y una base de datos creada con sql server.
Para la Api se crearon diferentes tipos de consultas de tipo get las cuales acceden a la base de datos, ya sea crear el o eliminar bases de datos como también filtrar información. 
## Consultas
- Crear Base de datos
- Eliminar Base de datos
- Cargar tablas temporales
- Presidentes y Vicepresidentes por partido
- Numero de diputados
- Candidatos a alcalde
- Cantidad de candidatos por partido
- Votos por departamento
- Votos nulos
- Top 10 edad de ciudadanos
- Top 10 candidatos más votados para presidencia
- Top 5 mesas mas frecuentadas
- Top 5 hora mas concurrida
- Cantidad de votos por género

La estructura de la base de datos Está hecha de la siguiente manera en la cual mostramos el modelo conceptual de la base de datos. También tenemos el modelo lógico que utilizamos para poder crear posteriormente nuestro modelo físico.

### Modelo Conceptual

![ModeloConceptual](https://github.com/Barahona1602/DB_Votaciones/assets/98893615/df10b9f5-97ba-4e92-a172-0ad088b182f6)

### Modelo Lógico

![ModeloLogicol](https://github.com/Barahona1602/DB_Votaciones/assets/98893615/b2b4fc9d-3fb2-4187-b287-78716141ebb7)

### Modelo Físico

![ModeloFisico](https://github.com/Barahona1602/DB_Votaciones/assets/98893615/ae045b1d-af92-4ea5-89c7-0468906f8fbb)

Al momento de crear las tablas se tuvo que normalizar para eliminar la redundancia de datos ya que venían valores repetidos la tabla que se normalizó es la tabla voto la cual despliega una nueva tabla llamada detalle voto y esta especifica los valores que se añadieron. Finalmente se crearon ocho tablas las cuales están conectadas entre sí ya que sql es un modelo de bases de datos relacional en el cual se accede con llaves primarias  llaves foráneas el objetivo de este tipo de bases de datos es eliminar la redundancia de datos Y así obtener mayor orden y precisión en su obtención de datos
