# From Zero to PlantDB: A Complete Plant Database

## English Version

Our Python programming professor, Daniel Báscones García (UCM) with Carlos González Calvo (UCM), propose the following problem:

A botany laboratory aims to organize its plant collection in a database in order to provide accurate and reliable information to its researchers. They do not wish to use any existing database system and have tasked us with developing one entirely from scratch.
The database will be implemented as a dictionary of dictionaries. In the outer dictionary, the key will be the plant’s name. The inner dictionary will contain three fields: the plant’s height in centimeters, its habitat (aquatic or terrestrial), and a list of provinces where it can be cultivated.

The program will provide a menu-driven interface allowing users to perform the following operations:

- Enter data for a new plant (the number of provinces where it can be cultivated may vary). If the plant already exists in the database, its previous data will be overwritten.
- List all plants, displaying only their names (formatted appropriately).
- Display the data of a specific plant (formatted appropriately).
- Search for plants whose height falls within a user-specified range (e.g., between 120 and 180 cm).
- Search for plants according to their habitat (aquatic or terrestrial).
- Search for plants that can be cultivated in a given province.
- Exit the program.

The program must be structured using functions corresponding to each menu option. Each function should accept the database as an argument, request any necessary input from the user, process the data, and return the appropriate results. The program’s main function (or "main") will host the interactive menu, allowing the user to perform multiple operations until they choose to exit.

To preserve the data entered by the user, the database will be stored in a file named BBDD_plantas.txt. Upon launching the program, any previously stored data should be loaded. Upon exiting, the program must write the updated database back to the file. If the database file does not exist when the program starts, it should be created, and the user should be informed that the database is initially empty.

### Database Structure
The database (BBDD) is a dictionary of dictionaries:
- **Key:** plant name
- **Value:** dictionary with the following fields:
  - `size`: height in centimeters
  - `habitat`: "aquatic" or "terrestrial"
  - `provinces`: list of Spanish provinces where the plant can be cultivated

### Features
The program provides an interactive menu that allows:
1. Adding or updating a plant (any number of provinces)
2. Listing all plants (names only)
3. Displaying data of a specific plant
4. Searching plants within a size range
5. Searching plants by habitat
6. Searching plants by (spanish) provinces
0. Exiting the program

### File Storage
The database is stored in `BBDD_plantas.txt`:
- The program loads existing data on start.
- If the file does not exist, a new empty database is created.
- Data is saved back to the file on exit.

### How to Use
1. Open the Jupyter Notebook (`PINTADO_RODRIGO_ALBA-Práctica_final_BIO.ipynb`).
2. Run all cells sequentially.
3. Use the menu to interact with the database.
4. Your data will be saved automatically when exiting.

---

## Versión en Español

Nuestros profesores de programación en Python, Daniel Báscones García (UCM) junto a Carlos González Calvo (UCM) nos proponen el siguiente problema:

Un laboratorio de botánica quiere organizar su colección de plantas en una base de datos (BBDD) a fin de proporcionar información adecuada a sus investigadores. No quiere utilizar ninguna BBDD existente y nos propone desarrollarla desde cero:

La BBDD será un diccionario de diccionarios. Para el primer diccionario la clave será el nombre de la planta. El segundo diccionario (el que estaría dentro del primer diccionario) consta de 3 campos: tamaño en centímetros de la planta, hábitat (acuático o terrestre) y una lista con las provincias donde puede cultivarse.

El programa nos permitirá hacer una serie de cosas, elegidas por un menú:

    1. Introducir los datos de una nueva planta (el número de provincias donde se puede cultivar puede variar de una a otra) (Si ya existía en la BBDD se sobreescribirán los datos con los nuevos).
    2. Listar todas las plantas mostrando únicamente sus nombres (con cierto formato).
    3. Mostrar los datos de una planta determinada (con cierto formato).
    4. Buscar aquellas plantas cuyo tamaño se encuentre en un determinado rango que se pedirá al usuario (p.ej entre 120 y 180cm).
    5. Buscar aquellas plantas de un hábitat determinado (Acuático/terrestre).
    6. Buscar aquellas plantas que se puedan cultivar en una provincia.
    0. Salir del programa. 

El programa debe estructurarse con funciones para cada una de las diferentes opciones. Las funciones deberán recibir como argumento la BBDD. Pedirán al usuario la información necesaria, y la procesarán para devolver el resultado pertinente. La función principal del programa (o "main") que contenga el menú, será interactiva para el usuario, permitiendo ejecutar varias funcionalidades hasta que el usuario quiera salir.

Para no perder los datos que el usuario va introduciendo vamos a almacenar la BBDD en un fichero llamado 'BBDD_plantas.txt'. De esta forma, cada vez que se ejecute el programa deberán recuperarse los datos almacenados previamente y al salir del programa debe escribirse la información de la BBDD en fichero. Si al iniciar el programa, no existe el fichero de BBDD, deberá crearse y advertir al usuario de que comienza con una BBDD vacía.

### Estructura de la BBDD
La BBDD es un diccionario de diccionarios:
- **Clave:** nombre de la planta
- **Valor:** diccionario con los siguientes campos:
  - `tamaño`: altura en centímetros
  - `hábitat`: "acuático" o "terrestre"
  - `provincias`: lista de provincias españolas donde puede cultivarse la planta

### Funcionalidades
El programa ofrece un menú interactivo que permite:
1. Añadir o actualizar una planta (cualquier número de provincias)
2. Listar todas las plantas (solo nombres)
3. Mostrar los datos de una planta determinada
4. Buscar plantas por rango de tamaño
5. Buscar plantas por hábitat
6. Buscar plantas por provincia
0. Salir del programa

### Almacenamiento en archivo
La base de datos se almacena en `BBDD_plantas.txt`:
- Se cargan los datos existentes al iniciar el programa.
- Si el archivo no existe, se crea una BBDD vacía.
- Los datos se guardan al salir del programa.

### Cómo usar
1. Abrir el notebook de Jupyter (`PINTADO_RODRIGO_ALBA-Práctica_final_BIO.ipynb`).
2. Ejecutar todas las celdas en orden.
3. Usar el menú para interactuar con la base de datos.
4. Los datos se guardan automáticamente al salir.

