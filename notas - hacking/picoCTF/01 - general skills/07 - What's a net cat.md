
DESCRIPCION
Usar netcat (nc) será muy importante. ¿Puedes conectarte a jupiter.challenges.picoctf.org en el puerto 41120 para obtener la bandera?
 
SOLUCION
Descargué Nmap en windows para escanear hosts y puertos, junto a eso viene Ncat que me sirvió también, lo agregué al path y ahora mi git bash logró acceder a la bandera con este comando:
ncat jupiter.challenges.picoctf.org 41120

y el resultado fue:
picoCTF{nEtCat_Mast3ry_3214be47}

NOTAS ADICIONALES
Estás en camino a convertirte en un gran maestro del Net Cat

REFERENCIAS