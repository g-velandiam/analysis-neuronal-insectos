# Bitácora de prompts — lab 1

## Prompt 1
> *Trabajo en **Python** dentro de Google Colab.* *Tengo un DataFrame de pandas llamado **`datos`** con las columnas **`neurona`** (texto), **`estimulo`** (texto: "viento" o "silencio"), **`ensayo`** (entero) y **`n_spikes`** (entero). Son registros extracelulares del sistema cercal de un grillo.* *Quiero un ****gráfico de barras**** del promedio de **`n_spikes`** por **`estimulo`**, con ****barras de error**** de desviación estándar.* *Incluye labels de los ejes con unidades, un título corto y colores pálidos.* *Explícame qué hace cada línea con un comentario.*

**Qué me devolvió:** *¡Claro! En Google Colab puedes hacerlo así. Este código calcula el promedio y la desviación estándar de n_spikes para cada estímulo y luego los grafica como barras con barras de error.*
*¿Qué está haciendo en conjunto? groupby("estimulo") separa los datos entre viento y silencio. mean calcula el promedio de spikes. std calcula la desviación estándar, que aparece como las barras de error. yerr=resumen["std"] hace que cada barra tenga ±1 desviación estándar. capsize=5 agrega las pequeñas líneas en los extremos de las barras de error. Los colores usados son tonos pálidos para diferenciar los dos estímulos.*

**Qué tuve que corregir:** Nada


## Prompt 2
> *Trabajo en Python dentro de Google Colab. Tengo un DataFrame de pandas llamado datos con una columna n_spikes que indica el número de spikes registrados por ensayo. Crea un histograma de n_spikes únicamente para los registros con estímulo "viento". Filtra los datos antes de graficar, configura una estética limpia con colores pálidos, añade labels de los ejes con unidades, un título corto y una cuadrícula suave. Explica mediante comentarios qué realiza cada línea del código. Termina indicando brevemente cómo interpretar el histograma.*

**Qué me devolvió:** *Sii, siguiendo la misma lógica que hemos estado usando para las condiciones, puedes hacerlo así:*
*¿Cómo se interpreta? Cada barra muestra cuántos ensayos tuvieron un número de spikes dentro de determinado intervalo. Así puedes observar cuáles valores de n_spikes son más frecuentes cuando el estímulo es viento y qué tan dispersos están los registros.*

**Qué tuve que corregir:** Nada
