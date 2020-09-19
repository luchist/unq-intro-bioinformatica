# Trabajo Practico #3

## Integrantes

 - Esteban Cicovich
 - Luis Coronel
 - Nicolas Alvarez
 - Juan Hualumpa


## Reto 1:
### Enumerá las diferencias que existen entre una célula procariota y eucariota.
 


Eucariota

	* Tiene núcleo con su ADN centralizado
	* Tiene membrana celular
	* Es de mayor tamaño
	* Tiene mitocondria
	* Tiene sus componentes sectorizados
	* No tiene flagelo
	* los genes “informacionales” tienen su origen en el reino archaea, mientras que los genes “operacionales” tienen su origen en el reino bacteria


Procariota

	* Tiene su ADN repartido en toda su estructura
	* Pared celular
	* Mucho mas pequeña que la eucariota
	* No posee mitocondria
	* No tiene division de componentes
	* Posee un flagelo


## Reto 2:
### Crea un programa sencillo en algún lenguaje de programación que conozcas que imprima una cadena de ARN codificante para el siguiente péptido (cadena corta de aminoácidos).

```
Sec1: ‘ATVEKGGKHKTGPNEKGKKIFVQKCSQCHTVLHGLFGRKTGQA'
```

```python
    
dict1 = {"A": "Phe", "T": "Leu", "V": "Ser"}
dict2 = {"Phe": "UUU", "Leu": "UGH", "Ser": "UUP"}


myString = 'ATV' #EKGGKHKTGPNEKGKKIFVQKCSQCHTVLHGLFGRKTGQA'
for c in myString:
    print(dict2[dict1[c]])

#diccionarios generados con regexp:

aminoacidsDict = {
    "A": "Ala",
    "R": "Arg",
    "N": "Asn",
    "D": "Asp",
    "C": "Cys",
    "Q": "Gln",
    "E": "Glu",
    "G": "Gly",
    "H": "His",
    "I": "Ile",
    "L": "Leu",
    "K": "Lys",
    "M": "Met",
    "F": "Phe",
    "P": "Pro",
    "S": "Ser",
    "T": "Thr",
    "W": "Try",
    "Y": "Tyr",
    "V": "Val"
}


geneticCodeDict = [
    "Phe": ["UUU", "UUC"],
    "Ser": ["UCU", "UCC", "UCA", "UCG", "AGU", "AGC"],
    "Tyr": ["UAU", "UAC"],
    "Cys": ["UGU", "UGC"],
    "Leu": ["UUA", "UUG", "CUU", "CUC", "CUA", "CUG"],
    "Try": ["UGG"],
    "Pro": ["CCU", "CCC", "CCA", "CCG"],
    "His": ["CAU", "CAC"],
    "Arg": ["CGU", "CGC", "CGA", "CGG", "AGA", "AGG"],
    "Gln": ["CAA", "CAG"],
    "Ile": ["AUU", "AUC", "AUA"],
    "Thr": ["ACU", "ACC", "ACA", "ACG"],
    "Asn": ["AAU", "AAC"],
    "Met": ["AUG"],
    "Lys": ["AAA", "AAG"],
    "Val": ["GUU", "GUC", "GUA", "GUG"],
    "Ala": ["GCU", "GCC", "GCA", "GCG"],
    "Asp": ["GAU", "GAC"],
    "Gly": ["GGU", "GGC", "GGA", "GGG"],
    "Glu": ["GAA", "GAG"]
}

```


## Reto 3: 
### Crea un programa sencillo de algun lenguaje de programacion que conozca que permita identificar las regiones promotoras de un gen en una secuencia dada de ADN, considerando que tal region comienza y termina con la caja TATA

 ```python
  p = "TATAAA TGCGAA TATAAA TTCAAG TATAAA TGCGCG TATAAATATAAA"

def devolverIntermedios(proteina,res):
    ls = []
    for i in list(range(0,len(res)-1)):
        ls.append(proteina[res[i]:res[i+1]-6])
    return ls

def identificarTATA(proteina) :
        res = []
        for n in list(range(0,len(proteina)-1)) : 
            if(proteina[n : (n + 6)] == "TATAAA"):
                res.append(n + 6)
        return devolverIntermedios(proteina,res)

#prueba
print(identificarTATA(p))
 ```

## Reto 4:
###

    Utilizamos Pilas Engine para realizar una demo. El arhivo se encuantra [aqui](/proyecto.pilas)