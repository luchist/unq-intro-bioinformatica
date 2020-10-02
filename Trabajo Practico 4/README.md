# Trabajo Practico #4
# ¿En que se parecen una gallina y una mosca?

## Integrantes

 - Esteban Cicovich
 - Nicolas Alvarez
 - Luis Coronel
 - Juan Hualumpa

### Archivo FASTA
Creamos nuestro [archivo fasta](secuencias-citocromo-c.fasta) usando la herramienta Clustal Omega


### Completar el cuadro con el nombre comun

|   Secuencia   | Nombre taxonómico | Nombre común |
| ------------- |:-------------:|:-------------:|
|  NP_061820.1  |  Homo sapiens |    Humano     |
|  NP_001072946.1  |  Gallus gallus  |    Gallo    |
|  NP_001065289.1  |  Pan troglodytes  |  Chimpancé común  |
|  NP_001157486.1  |  Equus caballus |   Caballo   |
|  NP_001183974.1  | Canis lupus familiaris |  Perro Domestico  |
|  AEP27192.1  |  Gorilla gorilla  |  Gorila Occidental  |
|  XP_024245566.1  |  Oncorhynchus tshawytscha  |  Salmon Real  |
|  NP_001086101.1  |  Xenopus laevis  |  Rana de uñas africana  |
|  NP_477164.1  |  Drosophila melanogaster  |  Mosca de la fruta  |


### ¿Cuán sencillo será alinear dos o más secuencias a mano?
#### ¿Cuánto influirán el número de secuencias a alinear, su longitud, y la similitud entre ellas?
#### ¿Son parecidos los citocromos c de humano y gallo?

>R: Comparacion de citocromos de Humano y Gallo, hecha a mano

```
MGDVEKGKKIFIMKCSQCHTVEKGGKHKTGPNLHGLFGRKTGQAPGYSYTAANKNKGIIWGEDTLMEYLENPKKYIPGTKMIFVGIKKKEERADLIAYLKKATNE
MGDIEKGKKIFVQKCSQCHTVEKGGKHKTGPNLHGLFGRKTGQAEGFSYTDANKNKGITWGEDTLMEYLENPKKYIPGTKMIFAGIKKKSERVDLIAYLKDATSK
```

>No es sencillo comparar a mano las secuencias ya se se dificulta el encontrar diferencias, mas si se tratara de mas de dos especies

>Se podria decir que entre mas larga sea la secuencia mas posibilidades de encontrar diferencias por ejemplo de longitud o de aminoacidos faltantes,
lo cual requiere alinear los aminoacidos, complejizando mas la tarea.

>Los citocromos de Humano y Gallo son muy parecidos, teniendo la secuencia 12 diferencias de entre 105 aminoacidos


#### ¿Qué teorías subyacen a este análisis?
#### ¿Cómo nos ayuda la evolución a explicar sus similitudes y diferencias?

>Podemos decir que las similitudes entre las cadenas de aminoacidos nos podria indicar que tanto Humano como Gallo poseen un ancestro evolutivo comun,
en tanto las diferencias nos indican especies mas alejadas dentro del arbol filogenetico (por ejemplo la rana tiene una secuencia muy distinta respecto del
humano y gallo)

### Recurso: Clustal Omega

#### ¿Qué indican los colores? (Show Colors)
>R:los colores nos indican el tipo de aminoacidos

#### ¿Qué indican el guión (-), los dos puntos (:) y el asterisco (*)?
>R:el guion indica aminoacidos faltantes, los dos puntos los aminoacidos distintos  y el asterisco aminoacidos que son iguales para todas las cadenas

#### A simple vista, ¿se conserva la secuencia del citocromo c en los organismos?

#### ¿Creeríamos que todos los organismos se asemejan por igual al resto, o se pueden identificar grupos de mayor similitud? Si es así, ¿tienen sentido?
#### ¿Qué evidencias nos aportaría este análisis, a la luz de la evolución?

#### A juzgar por los organismos participantes, ¿cuáles creería que deberían estar más agrupados en el árbol filogenético?

> https://www.ebi.ac.uk/Tools/services/web/toolresult.ebi?jobId=clustalo-I20200926-001047-0703-92061514-p2m&analysis=phylotree

#### Observemos el árbol filogenético. ¿Concuerda con lo esperado? ¿De qué organismos son los citocromos c más parecidos? ¿Cómo se explica?