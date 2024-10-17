# VC_P3

## Tarea 1

En esta tarea se ha utilizado el diametro de las monedas para identificarlas, como referencia se emplea la moneda de 1 euro, para la obtención e identificación de los bordes se ha aplicado un filtro gaussiano a la imagen convertida a escala de grises, posteriormente se ha restado a la imagen las misma imagen con un filtro de Canny aplicado para resaltar los bordes y a está finalmente se la aplicado un umbralizado. Finalmente, se ha detectado los bordes externos y se han eliminados los bordes detectados que estan contenidos dentros de otros bordes. Cabe destacar que a las imágenes se le ha aplicado un reescalado para mayor comodidad. Tras haber obtenido los contornos y extraido la información, en esta caso el diametro, se ha comparado el ratio (diametro en pixeles / diametro real) de la moneada de 1 euro que se selecciona con los demás obtenidos para averiguar cuales son las monedas en cuestión, el ratio más cercano obtenido significa que es la moneda.

Monedas_1

Resize (0.3,0.3)

![image](https://github.com/user-attachments/assets/2ed6b804-4ad8-41db-907b-0bb492133274)

Monedas_2

Resize (0.4,0.4)

![image](https://github.com/user-attachments/assets/5ddc3b03-c927-4a74-90bf-a92a505ee602)

Monedas_3

Resize(0.5,0.5)

![image](https://github.com/user-attachments/assets/39068cb7-bb3f-4518-8ba6-d204892e68fb)


## Tarea 2

En esta tarea se han utilizado como características geométricas la presencia del negro en las muestras a través del color promedio en la muestra y su circularidad. Para la detección de los bordes de las muestras se ha convertido la imagen a escala de grises, aplicado un filtro gaussiano, un umbralizado, se han detectados los contornos externos y se han descartados los que estan contenidos dentros de otros bordes. Tras haber obtenido la información, clasificamos las muestras dependiendo de la presencia del negro u oscuridad, significa que es TAR, su circularidad nos indica si es PELLET y en el caso de que no corresponder con ninguno de los anteriores se clasifica como FRA (Fragmentos). En estos caso hemos establecido ciertos valores como un mínimo de circularidad (17) y de presencia de negro (120) para la clasificación.

Fragmentos

![image](https://github.com/user-attachments/assets/9d506309-a281-469c-ae03-12c38441a8fc)

Tar

![image](https://github.com/user-attachments/assets/6d513f16-18dd-4fb2-bc9d-127ff64358ed)

Pellets

![image](https://github.com/user-attachments/assets/3b1021e3-6f95-46d6-ab52-e08d1561bc85)

Matriz de confusión 0 TAR 1 FRA 2 PEL

![image](https://github.com/user-attachments/assets/c185f658-f014-4e13-bc4d-5cc1399c2389)


