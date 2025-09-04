DESCRIPCION
¿Se pueden invocar indicadores de ayuda para una herramienta o un binario? Este programa contiene información muy útil...

SOLUCION
Descargué el archivo y definí el aerchivo "warm" como "f" para usar estee comando que me ayudó en el reto pasado:
$strings "$f" | grep -oE 'picoCTF\{[^}]+\}'
Y la solución fue esto:

picoCTF{b1scu1ts_4nd_gr4vy_d6969390}

NOTAS ADICIONALES
Bastante fácil gracias al enterior

REFERENCIAS