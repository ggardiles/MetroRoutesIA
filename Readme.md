# Proyecto Inteligencia Artificial
Universidad Politecnica de Madrid
### Formato del proyecto
Hay 4 clases fundamentales:
- **AtributosEstación**: Clase POJO donde se definen todas las propiedades de una estación
- **EstacionesMonterrey** Clase Pojo donde se crean todas las estaciones pertenecientes al metro de monterrey
- **InterfazGrafica** (main) Clase de Swing que monta la interfaz gráfica.
- **Imagen**: donde se carga el fondo de metro monterrey.
- **AlgoritmoEstrella**: es una implementación del algoritmo estrella en la que se calcula el camino más simple. Tiene que tener en cuenta al ir haciendo un camino si el nodo actual es un isTransbordo. Es llamado desde la interfaz gráfica una vez que el usuario da a Calcular Trayecto.

### To do tasks:

1. Refactorización completa del Algoritmo A*

    - Reducir variables globales al mínimo
    - Eliminar variables locales booleanas de los while, if, switch...
    - Comparaciones de transbordo con la propiedad de AtributoEstacion
    
2. Introducir Estaciones del metro de monterrey

    - Mirar coordenadas en google maps para calcular distancias
    - Introducir el valor boolean isTransbordo para los 2/3 transbordos
    - Meter todas las estaciones en la Lista
    
3. Refactorizar la clase InterfazGrafica (ya tiene el png de metro_monterrey)

    - Hay que eliminar las estaciones comentadas y hacerlas coincidir con las estaciones de la clase EstacionesMonterrey
    - Modificar los colores
    - Modificar las coordenadas de las estaciones para que coincidan con la posicion x,y de las estaciones de Monterrey
