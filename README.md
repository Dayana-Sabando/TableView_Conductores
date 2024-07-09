## TableView de conductores


### Introducción 
El código es una aplicación JavaFX que muestra los resultados de pilotos de Fórmula 1 en una tabla, permitiendo la selección del año mediante un ComboBox para actualizar los datos mostrados. La interfaz gráfica incluye un ComboBox y una TableView, y los datos se obtienen de un repositorio (`DriverResultRepository`). 

![Captura de pantalla 2024-07-09 120421](https://github.com/Dayana-Sabando/TableView_Conductores/assets/168872451/4e10d555-974e-4a26-98c6-32bc5fc3aef2)



### Desarrollo 
En el desarrollo de la aplicación se mencionan varias clases Java situadas en el paquete `demo_jdbc.models`:

1. **Clase `Circuit`**: Hace referencia a un circuito con atributos como `circuitid`, `circuitref`, `name`, `location` y `country`, y cuenta con un constructor, así como métodos getter y setter.
2. **Clase `Season`**: Tiene un atributo `year`, un constructor, y métodos getter y setter para mostrar los años a consultar.
3. **Clase `CircuitRepository`**: Se encarga de las operaciones de base de datos relacionadas con objetos `Circuit`, incluyendo métodos para recuperar circuitos por país o todos los circuitos, y para agregar un nuevo circuito (aunque este último método está incompleto).
4. **Clase `DriverResult`**: Contiene los resultados de un conductor con atributos como `driverName`, `wins`, `totalPoints` y `rank`, e incluye un constructor y métodos getter y setter.
5. **Clase `SeasonRepository`**: Esta interactúa con una base de datos PostgreSQL para obtener una lista de objetos `Season`, estableciendo una conexión a la base de datos, ejecutando una consulta SQL y procesando los resultados para devolver una lista de temporadas.


![Captura de pantalla 2024-07-09 120437](https://github.com/Dayana-Sabando/TableView_Conductores/assets/168872451/ef8055f7-895f-4e83-a65b-dd84b2494fce)





![Captura de pantalla 2024-07-09 120525](https://github.com/Dayana-Sabando/TableView_Conductores/assets/168872451/413931b0-6751-4a2f-9652-142a96dfb5b3)



### Conclusión 
Esta aplicación JavaFX propuesta integra varias clases para manejar circuitos, temporadas y resultados de conductores, utilizando repositorios para interactuar con la base de datos y actualizar la interfaz gráfica basada en la selección del usuario. para luego mostrar el contenido que residen de cada una de las selecciones.
