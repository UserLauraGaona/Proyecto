# Proyecto

![Captura de pantalla 2024-07-09 170334](https://github.com/UserLauraGaona/Proyecto/assets/175163285/533b13f7-cc8b-4560-9fab-84336958da30)


Este código define la interfaz gráfica de una aplicación para consultar resultados de constructores de Fórmula 1 por año, similar a la aplicación anterior para pilotos.

# Partes del código:
# Objetos:
* Se crea una instancia de ConstructorsRepository para interactuar con la base de datos y obtener resultados de constructores.
* Se define una TableView para mostrar los resultados en una tabla.
* Se crea un ComboBox para que el usuario seleccione el año.
# Método start:
* Define el título de la ventana principal ("Formula 1 Constructors Results").
* ComboBox para año:
* Similar al código anterior, se obtienen los años disponibles, se llena el ComboBox y se define un evento para actualizar la tabla.
# Etiqueta para ComboBox:
* Se crea una etiqueta ("SELECCIONAR EL AÑO QUE DESEA CONSULTAR:") para indicar al usuario la función del ComboBox.
* Se agrega la etiqueta y el ComboBox a un contenedor HBox para organizarlos horizontalmente.
# TableView para resultados:
* Se crean columnas para la tabla con los nombres de las propiedades del objeto Constructors (nombre del constructor, victorias, puntos totales y ranking).
* Se utiliza setCellValueFactory para asignar cada columna a la propiedad correspondiente del objeto Constructors.
* Se añaden todas las columnas a la tabla (tableView.getColumns().addAll).
# Layout:
* Se crea un contenedor VBox para organizar los elementos de forma vertical con un espacio de 10 pixeles entre ellos.
* Se agrega el contenedor HBox con la etiqueta y el ComboBox y luego la TableView al contenedor VBox.
* Se establece un margen de 10 pixeles para el contenedor principal.
* Se crea la escena con el contenedor VBox y se define su tamaño (600x400 pixeles).
* Se muestra la ventana principal (primaryStage).
# Método updateTable:
* Similar al código anterior, recibe el año seleccionado, obtiene los resultados, los convierte a ObservableList y actualiza la tabla.
# Método main:
* Inicia la aplicación JavaFX (launch).
