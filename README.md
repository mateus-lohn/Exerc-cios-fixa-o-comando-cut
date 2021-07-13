# Exerc-cios-fixa-o-comando-cut1)
#!/bin/bash # Interpretador shell
valor=$(cut -d":" -f3 /etc/passwd)
numero_user=0 # A variavel numero_user é igual a 0
for i in $valor
do # Faça
        if [[ $i -gt 999 && $i -lt 2000 ]]
        then
                numero_user=$((numero_user+1))
        fi
done # Feito
echo $numero_user 

2)

Lista_Frutas

1 Laranja 2,00
2 Maçã 3,50
3 Açaí 7,00
4 Tangerina 4,00
5 Abacaxi 4,50
6 Caju 6,00
7 Mamão 2,30
8 Pitanga 4,30
9 Romã 8,50
10 Acerola 6,30
11 Graviola 3,80

------------------------------------------------------
a)
#!/bin/bash
cut -d" " -f2 Lista_Frutas

b)
#!/bin/bash
cut -d" "f -f2,3 Lista_Frutas

c)
#!/bin/bash
cut -d" " -f2,3 Lista_Frutas | sort
