### Cual es la mascara por default de una direccion de clase A, B Y C?
* A: 255.0.0.0
* B: 255.255.0.0
* C: 255.255.255.0

### Indicar el rango de redes privadas correspondientes al rango de direcciones de clase A, B y C
* A: 10.0.0.0 ... 10.255.255.255
* B: 172.16.0.0 ... 172.31.255.255
* C: 192.168.0.0 ... 192.168.255.255

### A que clase corresponde la direccion IP 10.34.106.78 con mascara 255.255.255.0
Clase A

### En que Subred se encuentra inserto el host cuya dirección IP es 168.26.201.245 y máscara 255.255.252.0
Subred: 168.26.200.0
```
Clase B -> 255.255.0.0 adicionalemente se tomaron 6 bit mas*
128 64 32 16 8 4 2 1 
1   1  1  1  1 1 0 0
1   1  0  0  1 0 0 1
```

### Cuales son los host validos para la red a la que pertence el host 199.37.2.33/29. Idem para la red 199.37.2.9/27. Teoricamente es una red valida la anterior? Si se tomara la primera combinacion distinta de cero en el campo de subred que se observara con respecto a la subred 199.37.2.33/29
1. 199.37.2.33/29 -> Host Por subred: 6. 199.37.2.33 - 199.37.2.38
2. 199.37.2.9/27  -> Host Por subred: 30. 199.37.2.1 - 199.37.2.30
```
Clase C: /24  29-24=5
Publica
Masc Subnet = 255.255.255.248
Bit para host 8-5=3
Host Por subred: 2^3-2 (ID RED + BR) = 6
SubRed: 199.37.2.32
Broadcast: 199.37.2.39
```

### Cual es la direccion de red, broadcast y host validos a la cual pertence el host 120.77.2.50 con 12 bits de subnetting.
Direccion de red: 120.64.0.0
Broadcast: 120.79.255.255
Cant Host validos: 2 ^ ( 32 - 12 ) - 2
Rango Host validos: 120.64.0.1 - 120.79.255.254

### La subred obtenida en el punto anterior vuelve a subdividirse, tomandose ahora 6 bit mas de subnetting (120.77.2.50/18). Indicar:
a. Rengo de subredes disponibles: 120.0.0.0 .. 120.255.192.0
b. Cantidad de host en cada subred:  2 ^ ( 32 - 18 ) - 2
c. Para la ultima subred permitida obtener:
 1.  Direccion del gw: 120.255.192.1
 1.  Direccion del 1 host: 120.255.192.2
 1.  Direccion del ultimo host: 120.255.255.254
 1.  Direccion de broadcast: 120.255.255.255
 
### Planificar
* Se debe realizar una conexion punto a punto entre un router de la casa central de un banco y otro router en una de sus sucursales. Determinar:
a) La mascara de subred mas conveniente desde el punto de vista de la optimizacion de direcciones IP.
b) La direccion de red, broadcast y las direcciones de hosts si se parte de la direccion clase C 192.68.1.0/24
