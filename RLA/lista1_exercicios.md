# UNIFOR
**Nome**: Samuel Mesquita Rocha

**Disciplina**: Raciocínio lógico algorítimo

## Lista de exercícios 01

### Exercício 3
Represente, em fluxograma e pseudocódigo, um algorítimo para determinar se um número inteiro e positivo é impar ou par

#### Fluxograma
```mermaid
flowchart TD
A([INICIO]) --> B{{Digite um número}}
B --> C[/num/]
C --> D{num >= 0}
D --False--> E{{O número deve ser positivo!}}
E --> F([FIM])
D --True--> G[resto = num % 2 ]
G --> H{num == 0}
H --False--> I{{O número é ímpar!}}
H --True--> J{{O número é par!}}
I --> F
J --> F
```
#### Pseudocódigo
```
ALGORITMO verifica_par_impar
DECLARE num: int,resto: int

INICIO
ESCREVA "Digite um número"
LEIA num
SE num >= 0 ENTAO
	resto <- num % 2
	SE resto == 0 ENTAO
		ESCREVA "O número é par!"
		
    SENAO
	    ESCREVA "O número é ímpar!"
	FIM_SE
	
SENAO 
	ESCREVA "O número deve ser positivo!"
FIM_SE

FIM
```
#### Teste

| num | num >= 0 | resto | resto == 0 | Saída |
| -- | -- | -- | -- | --|
| -1 | False | | | "O número deve ser positivo!' |
| 0 | True | 0 | True | "O número é par!" |
| 10 | True | 0 | True | "O número é par!" | 
| 11 | True | 1 | False | "O número é ímpar!"|
