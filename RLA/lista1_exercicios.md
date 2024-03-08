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
