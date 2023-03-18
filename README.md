# Script para actualización de programa LCA
## Documentación de diseño
### Script: Análisis LCA

El script que vamos a utilizar para la carga de archivos (LCA y Base de AM's) y análisis de datos permite unir tres DataFrames para su posterior análisis, buscando posibles duplicidades y filtrando aquellos registros que no tienen un vendedor asignado. A continuación se detallará cómo utilizar este script para cargar los archivos necesarios y ejecutar la rutina de análisis.

### Instalación de librerías
Este script utiliza algunas librerías que no están instaladas por defecto en Python. Para instalarlas, debemos descomentar las líneas que contienen las funciones pip install y ejecutarlas. Una vez hecho esto, ya estaremos preparados para ejecutar el script.

### Establecer las rutas de los archivos
Antes de comenzar la carga de archivos, debemos establecer las rutas donde se encuentran los archivos necesarios. Para ello, debemos modificar las siguientes variables:

* dir_path_src: ruta del directorio principal del proyecto.
* dir_path_data: ruta donde se encuentran los archivos de entrada.
* dir_path_output: ruta donde se guardarán los archivos de salida.
* nom_archivo_lca: nombre del archivo de datos que vamos a utilizar.
* nom_archivo_vendedores: nombre del archivo de vendedores que vamos a utilizar.
* nom_archivo_configuracion: nombre del archivo de configuración que vamos a utilizar.
* nom_archivo_actualizacion_am: nombre del archivo temporal donde se guardarán los registros sin vendedor.

### Cargar los archivos de entrada
Para cargar los archivos de entrada, debemos ejecutar el script en Python. Cuando se ejecute, se mostrarán en pantalla los archivos que se van cargando y si se han cargado correctamente o no.

### Unión de DataFrames
Una vez cargados los archivos, el script unirá los DataFrames necesarios para comenzar con el análisis. Si alguno de los archivos no se ha cargado correctamente, el script mostrará un mensaje de error y no se podrá continuar con la rutina de análisis.

### Completar los registros sin vendedor
El script verifica si existen registros sin vendedor asignado. Si es así, los filtra y los guarda en un archivo temporal. Para este proceso, el script utiliza la etiqueta * TBD * para identificar los registros sin vendedor. Si no existe ningún registro sin vendedor asignado, el script mostrará un mensaje indicando que no se han encontrado registros sin vendedor.

### Guardar los archivos de salida
El script guardará los archivos de salida en la ruta dir_path_output. Si se ha guardado algún archivo temporal durante la ejecución del script, este también se guardará en esta ruta.

Con estos pasos, ya estaríamos preparados para ejecutar el script y comenzar con el análisis de datos.
