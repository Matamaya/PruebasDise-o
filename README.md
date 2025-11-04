# Pruebas de Diseño (Flex, Grid, Animación)

## Descripción
Realizar pruebas de diseño en HTML con los códigos proporcionados

## FlexBox
Las pruebas a continuacion funcionan gracias a que tenemos puesto display: flex 

### Ejercicio 1: Alinear elementos en una fila

Objetivo: Crear un contenedor Flexbox que alinee tres elementos en una fila.

- Resultado con flex-direction: row
<img width="521" height="187" alt="image" src="https://github.com/user-attachments/assets/2457c0d5-7c72-4a39-b625-f7bdc371a4a5" />

Podemos cambiar la flex-direction:
- Column
<img width="1152" height="309" alt="image" src="https://github.com/user-attachments/assets/ab4a5688-d3d7-4554-b34c-ae3d973795f4" />

O invertirlo con row-reverse:
<img width="961" height="227" alt="image" src="https://github.com/user-attachments/assets/3d50557c-789b-4919-a75e-bdf61c986124" />


### Ejercicio 2: Alinear elementos en el centro vertical y horizontalmente
Objetivo: Centrar tres elementos en el medio de la pantalla, tanto vertical como horizontalmente.

Resultado:
<img width="599" height="352" alt="image" src="https://github.com/user-attachments/assets/41f39700-58f9-4b52-9782-f00925378716" />

Al igual que antes, podemos cambiar la dirección a modo columna
<img width="470" height="435" alt="image" src="https://github.com/user-attachments/assets/aacf8083-5117-477a-8694-74a311f5bf77" />

Con justify-content elegimos la alineacion horizontal:

- flex-start (a la derecha)
<img width="700" height="378" alt="image" src="https://github.com/user-attachments/assets/4d079503-68bd-4f38-9596-6ec39f52ff82" />

Y tambien el espaciado:
<img width="885" height="338" alt="image" src="https://github.com/user-attachments/assets/891e0f46-5ee0-4788-91f3-e6e9e3b5a9ad" />

Con align-items podemos modificar la alineacion vertical:
- flex-start (arriba)
<img width="598" height="538" alt="image" src="https://github.com/user-attachments/assets/236056a8-31c3-4cb7-8d64-d446857a4de0" />

También se puede externder el interior de los contenedores con:
- stretch
  <img width="442" height="480" alt="image" src="https://github.com/user-attachments/assets/f29cc013-efea-48e2-878b-9fda73904c94" />

### Ejercicio 3: Crear una barra de navegación horizontal con enlaces distribuidos equitativamente

<img width="1902" height="106" alt="image" src="https://github.com/user-attachments/assets/94bf5c60-4050-49a6-bd26-b56efd9b248e" />

Usando la propiedad justify-content: "space-around" --> Distribuimos el espacio entre los enlaces

### Ejercicio 4: Flexbox con varias filas (flex-wrap)
Organizar seis tarjetas en un contenedor Flexbox que permita dividir los elementos en varias filas cuando no quepan en una sola línea

Tamaño Completo:
<img width="1913" height="236" alt="image" src="https://github.com/user-attachments/assets/1dd00dc8-2b13-41ad-b435-826a3e13763b" />

Reduciendo el tamaño en pantalla:

<img width="1358" height="286" alt="image" src="https://github.com/user-attachments/assets/fd9cae68-f312-49ef-a77a-ef799a8bac36" />
<img width="1336" height="191" alt="image" src="https://github.com/user-attachments/assets/7104a0b2-f693-4e6f-bee5-beebb45f911f" />
<img width="1036" height="208" alt="image" src="https://github.com/user-attachments/assets/eb9382b0-e4ce-4437-b96a-bd1b5a0570f0" />
<img width="778" height="281" alt="image" src="https://github.com/user-attachments/assets/597f3dc1-0ba6-4c74-bdfb-4e34990bb42c" />
<img width="531" height="596" alt="image" src="https://github.com/user-attachments/assets/2e196b9a-e677-48b3-af27-84b58b82f2bc" />

Este efecto se consigue haciendo uso de la propiedad flex-wrap: "wrap" --> especifica si los elementos "hijos" son obligados a permanecer en una misma línea (non-wrap) o como en este caso pueden fluir en varias líneas (wrap)
gap (para el espacio entre elementos)
Además cada tarjeta tiene la proiedad flex: 1 1 220px --> /* En este caso son tres valores: flex-grow (el factor de crecimiento de un elemento) | flex-shrink (el factor de contracción) | flex-basis (el tamaño inicial de un elemento flexible) */

### Ejercicio 5: Flex-grow para ajustar tamaños
Crear tres columnas de diferente tamaño que crezcan proporcionalmente al espacio disponible
<img width="1912" height="187" alt="image" src="https://github.com/user-attachments/assets/0b999302-786a-4f5b-8b62-5f1aa0425a38" />

La columna Azul es la mayor, porque como se especifica con el estilo de .columna:nth-child(2) --> Es decir, se modifica al 2do elemento de un grupo de elementos hermanos (las columnas)
Y se le aplica flex-grow: 2 --> para que crezca el doble que las demas


### Ejercicio 6: Usar justify-content y align-items juntos
Alinear y distribuir los elementos usando justify-content y align-items para crear una disposición más compleja
<img width="1914" height="372" alt="image" src="https://github.com/user-attachments/assets/12a63ef9-662b-466f-b26b-149b9fad1066" />

Se usa justify-content: space-between y align-items: center, además de determinar una altura determinada con height

### Ejercicio 7: Flexbox Grid simple (flex-direction y flex-wrap)
Crear un diseño estilo "Grid" básico usando Flexbox, donde los elementos se dividan en filas y columnas, pero sin usar CSS Grid

<img width="746" height="301" alt="image" src="https://github.com/user-attachments/assets/ce2be196-c1cb-497c-bdcb-3f2c3dc93cfd" />

Al igual que antes usamos flex-wrap para permitir el escalado de elementos por filas
