DESCRIPCION 
Python scripts are invoked kind of like programs in the Terminal... Can you run [this Python script](https://mercury.picoctf.net/static/325a52d249be0bd3811421eacd2c877a/ende.py) using [this password](https://mercury.picoctf.net/static/325a52d249be0bd3811421eacd2c877a/pw.txt) to get [the flag](https://mercury.picoctf.net/static/325a52d249be0bd3811421eacd2c877a/flag.txt.en)?

SOLUCION
Utilicé este comando desde git bash "printf "%s\n" "$(tr -d '\r' < pw.txt)" | python3 -u ende.py -d flag.txt.en"
picoCTF{4p0110_1n_7h3_h0us3_ac9bd0ff}

NOTAS ADICIONALES
Entretenido

REFERENCIAS
