# <center>UNIVERSIDAD TECNOLOGICA NACIONAL</center> 

<center>

![](img1.png)

</center>

# <center>FACULTAD REGIONAL RESISTENCIA</center>
  
## <center> SISTEMAS OPERATIVOS</center>

### <center>Proyecto: Simulador para la administración de memoria y Planificación de Procesos
__Integrantes del equipo:__
- Arias, Leandro Exequiel
- Florentin, Cristian Alexis
- Imfeld, Facundo Nicolas
- Nasir, Khalil Abdul
- Matto, Pablo  

__Equipo docente:__
- Ing. Cuenca Plestch, Liliana
- Ing. Ristoff, Alberto
- Ing. Roa, Jorge Alejandro
- Ing. Gramajo, Sergio 
***
***
## __Índice__
#### [Introducción](#id1)
#### [Datos de Entrada y Salida](#id2)
#### [Visualización del Planificador](#id3)
#### [Consideraciones](#id4)
### Documentación del Simulador de Planificación de Procesos y Administración de Memoria 
#### Introducción<a name="id1"></a>

<p align=justify> El objetivo del desarrollo del siguiente simulador es permitir visualizar los aspectos de la planificación de procesos a corto plazo, empleando los algoritmos de planificación FCFS, Prioridades, Round Robin, Colas Multinivel. A demás se representará la gestión de la memoria con particiones Fijas y Variables para un esquema de un solo procesador, mostrando el ciclo de vida completo de un proceso desde su ingreso al sistema hasta su finalización.</p>  
<p align=justify> El objetivo de este documento es brindar información acerca del funcionamiento del simulador, en el mismo se detallaran las consideraciones que se tienen que tener en cuenta a la hora de cargar los datos requeridos para la simulación. Se detallara y adjuntara el funcionamiento de los diferentes algoritmos de planificacion y algoritmos de intercambio. </p>

### Datos de Entrada y Salida<a name="id2"></a>

__Partición de memoria__
1. Fija
  * Algoritmos de intercambio:
    * First Fit
    * Best Fit
  * Tamaño total
  * Tamaño ocupado para el SO
  * Cantidad de particiones
  * Tamaño de cada partición 
2. Variable
  * Algoritmos de intercambio:
    * Best Fit
    * Works Fit
  * Tamaño total
  * Tamaño ocupado para el SO

__Algoritmos de asignación__
* FCFS
* Por prioridades
* RR
  * Quantum
* Cola Multinivel

__Procesos__
* Cantidad de procesos
* Tamaño de cada proceso
* Tiempo de arribo
* Tiempo de irrupción

__Colas__
* Cola de Nuevos
* Cola de Listos
* Cola de CPU
* Cola de Entrada
* Cola de Salida

__Cálculos__
* TRP 
* TE
* TEP

__PCB__
* Id Proceso
* Estado
* Registro CPU
* Memoria asignada
* RLI
* RLS
* Base
* Desplazamiento  

### Visualización del Simulador<a name="id3"></a>

<p align=justify>Dispondremos de un menu en el cual podremos optar por Configuración de Arquitectura o Carga de Procesos</p>
<center> 

![](img2.jpeg)
</center>

__Opción Configuración de Arquitectura__  
<p align=justify>En esta opción podremos seleccionar el tipo de algoritmo de planificación con el que queremos trabajar(FCFS,Por Prioridades,Round Robin, Colas multinivel); también cargaremos aquí los datos correspondientes a la Memoria, en el cual seleccionaremos el tipo de partición a utilizar, el tamaño de la memoria y su unidad (b, kb, mb, gb), y el algoritmo de ajuste deseado. 

El campo Particiones estará disponible sólo en el caso que se seleccione particiones fijas. 
</p> 
<center>

![](img3.jpeg)
</center>

__Opción Carga de Procesos__
<p align=justify>Esta opción nos permitirá realizar la carga de todos los datos de los procesos requeridos para la simulación, como su nombre, tiempo de arribo tiempo de irrupción y ráfaga</p>
<center>

![](img4.jpeg)
</center>

__Pantalla de Resultados__  

Luego de cargar todos los datos necesarios, al ejecutar la simulación obtendremos en pantalla una tabla con toda la información de los procesos, y el Diagrama de Gantt . 
<center>

![](img5.jpeg)
</center>

### Consideraciones<a name="id4"></a> 
* Las imagenes presentadas anteriormente se presentan en modo de diseño preliminar, sujetas a modificaciones durante el desarrollo del proyecto hasta su entrega final.
* Colas multinivel: Se toma como referencia tres niveles de colas. Definir el quantum para cada cola.
