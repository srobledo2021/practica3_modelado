# Práctica 3

En este blog se van a explicar las gráficas que estudian el comportamiento del robot además de una serie de vídeos con su funcionamiento.

## 📊 Graficas requeridas y explicación

### 🚀 Comparativa de las velocidades de las ruedas

**Velocidad en cada rueda en el mapa de 'floor'**

![vel_floor](https://github.com/srobledo2021/practica3_modelado/assets/113594786/c0bbadf5-c70d-4aa3-b120-a2500d01696f)

**Velocidad en cada rueda en el mapa de 'sand'**

![vel_sand](https://github.com/srobledo2021/practica3_modelado/assets/113594786/3866a27e-fd89-4b08-b3e7-a676b5323998)

> Vemos como en ambas gráficas se cumple la especificación de la velocidad, ya que se asemejan a la gráfica que encontramos en el enunciado de la práctica. Durante los primeros 5 segundos el robot aumenta de forma constante su velocidad hasta ser esta de 5 y mantenerse otros 5 segundos. Más tarde en los últimos 5 desciende proporcionalmente hasta detenerse.

> Como vemos encontramos en ambas ciertas oscilaciones, estas coinciden que son mucho mas amplias cuando el robot choca con la caja y la arrastra. El hecho de que estas oscilaciones se presenten podría deberse a que en estos momentos se arrastra el cubo o incluso a que se ejecuten demasiados launchers ademas del rosbag en un ordenador que tiene ciertas limitaciones. 

> Ciertas diferencias que notamos son en estas oscilaciones ya que son muy distintas cuando el terreno también es distinto.


### 🔄 Comparativa de la velocidad de las ruedas y los desplazamientos que el controlador cree hacer

**Comparativa de velocidad y desplazamiento en el mapa de 'floor'**

![desp_floor](https://github.com/srobledo2021/practica3_modelado/assets/113594786/b652fd36-9e2f-4d04-9c40-9e467c01466a)

**Comparativa de velocidad y desplazamiento en el mapa de 'sand'**

![desp_sand](https://github.com/srobledo2021/practica3_modelado/assets/113594786/a3588bcf-bfe4-470f-884a-51951f182e9e)

> En este caso analizamos el desplazamiento y vemos como en el caso del mapa de floor, no ha sido tan contínuo como en el de sand. A pesar de que el robot demuestra que una vez choca con la rueda al cubo, la arrastra sin ningún problema, vemos como en el mapa de floor, cerca del segundo 9 durante un breve periodo de tiempo, el robot no se desplaza de la misma manera que el resto de la gráfica, ya que la pendiente es mayor en este intervalo. Además podemos fijarnos que en el mapa de sand al arrastrar el cubo, no se desplaza tantos metros como antes a la misma velocidad, es por esto que cerca del momento de choque, la pendiente de la gráfica se reduce y pasa a tener menos inclinación.


### ⚡ Comparativa de las aceleraciones ejercidas por el robot en cada mundo

**Comparativa de aceleraciones en el mapa de 'floor'**

![ac_floor](https://github.com/srobledo2021/practica3_modelado/assets/113594786/0316755c-dde8-43a4-b304-61eaec1d0bd1)

**Comparativa de aceleraciones en el mapa de 'sand'**

![ac_sand](https://github.com/srobledo2021/practica3_modelado/assets/113594786/c976ee80-9ff4-4b96-a70d-42b6acbb5c51)

> Para las aceleraciones, es muy claro como cumplen estos tres intervalos de 5 segundos de aumento de velocidad, velocidad constante y disminución. Ya que si nos fijamos en los 5 primeros segundos desde que se comienzan a comandar velocidades vemos como la aceleración cada vez es mayor hasta llegar aproximadamente a los 15 m/s^2, momento en el que disminuye por mantenerse otros 5 segundos a velocidad constante. Sin embargo este aumento de aceleración en estos primeros 5 segundos no es proporcional y esto es debido a que mientras el robot aumenta su velocidad, también se topa con el cubo, lo que hace que pierda aceleración de forma abrupta, como vemos en la gráfica.

## 🎥 Vídeos de la trayectoria que el robot sigue en cada mundo

[sand_world](media/sand.mp4)

[floor_world](media/floor.mp4)

### Rosbag Links

- [🌍 Floor World Rosbag](rosbag_files/kitt_rosbag_floor)
- [🏜️Sand World Rosbag](rosbag_files/kitt_rosbag_sand)

### 📹 Video explicativo de la parte A

[Ver Vídeo](https://www.youtube.com/watch?v=agDZcI3ZCNc)
