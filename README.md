**UNIVERSIDADE LUSÓFONA DE HUMANIDADES E TECNOLOGIAS**

*Linguagens de Programação I*

# Exercício Individual 1

>Na resolução deste exercício deve ser utilizada a Linguagem de Programação C. Para além da correta implementação dos requisitos, tenha em conta os seguintes aspetos:
>- O código apresentado deve ser bem indentado. 
>- O código deve compilar sem erros ou *warnings* utilizando o *gcc* com as seguintes flags:
>- `-g -Wvla -Wall -Wpedantic -Wextra -Wdeclaration-after-statement`
>- Tenha em atenção os nomes dados das variáveis, para que sejam indicadores daquilo que as mesmas vão conter.
>- O trabalho deve ser desenvolvido e submetido de forma individual.

>Este exercício deverá ser submetido na plataforma Pandora até às 10:00 do dia 06/03/2023 e será contabilizado para a nota final da unidade curricular de acordo com os critérios disponibilizados na página da disciplina, concretamente nos slides da primeira aula.

>Todos os trabalhos serão comparados utilizando um sistema de detecção de plágio.


## Descrição
A aplicacação vai ordenar quatro números inteiros e de seguida verifica se e possivel somar dois dos números e obter o valor 2023. 
Caso seja possível obter o valor 2023 então apresenta o resultado da multiplicação desses 2 números, caso contrário apresenta uma mensagem indicativa.
  
O programa inicia com a apresentação da mensagem:
```"Enter four integers:\n>"```

Depois de lidos os 4 valores inteiros, o programa pergunta ao utilizador se quer ordenar por ordem crescente ou decrescente. Para isso apresenta a seguinte mensagem:
```"Select (a) for ascending or (d) for descending?:\n>"```
E depois lê o caracter introduzido pelo utilizador. Deverá ignorar espaços e caso o utilizador introduza um caracter que não é o 'a' nem o 'd' deverá apresentar a mensagem de erro ```"Error: invalid option"``` e voltar a apresentar a mensagem que pede para introdução da opção de ordenação.

Após esta sequência, o programa deverá apresentar os números por ordem precedidos da mensagem:
```"Sorted array:\n"```

O programa deverá perguntar se o utilizador pretende continuar apresentando a seguinte mensagem:
```"Continue - (y) yes, (n) no?:\n>"```
Caso o utilizador introduza `n` o programa deverá terminar com a mensagem `"Bye\n"`. Caso o utilizador introduza `y` o programa deverá continuar.

Caso o utilizador pretenda continuar, o programa procura se há algum par de números cuja soma resulte em 2023. Caso encontre, deverá apresentar a seguinte mensagem
```"The multiplication of the pair that sums up to 2023 is: %d\n"```
Caso não encontre, deverá apresentar a mensagem
```"No pair of integers add up to 2023.\n"```

Caso haja mais do que uma combinação possível de números cuja soma resulte em 2023, a combinação apresentada deverá ser aquela cujo primeiro operando surge primeiro na lista de números ordenados.
 
## Exemplos de utilização:
### Exemplo 0
```bash
Enter four integers:
>1 5 2 3
Select (a) for ascending or (d) for descending?:
>a 
Sorted array: 
1 2 3 4
Continue - (y) yes, (n) no?:
>n
Bye
```


### Exemplo 1
```bash
Enter four integers:
>500 1023 5000 1000
Select (a) for ascending or (d) for descending?:
>a 
Sorted array: 
500 1000 1023 5000
Continue - (y) yes, (n) no?:
>y
The multiplication of the pair that sums up to 2023 is: 1023000
```

### Exemplo 2
```bash
Enter four integers:
>500 1024 5000 100
Select (a) for ascending or (d) for descending?:
>d
Sorted array: 
5000 1024 1000 500
Continue - (y) yes, (n) no?:
>y
No pair of integers add up to 2023.
```

### Exemplo 3
```bash
Enter four integers:
>1011 1012 1013 1010
Select (a) for ascending or (d) for descending?:
>a
Sorted array:
1010 1011 1012 1013 
Continue - (y) yes, (n) no?:
>y
The multiplication of the pair that sums up to 2023 is: 1023130  
```

### Exemplo 5
```bash
Enter four integers:
>1011 1012 1013 1010
Select (a) for ascending or (d) for descending?:
>a
Sorted array:
1010 1011 1012 1013
Continue - (y) yes, (n) no?:
>y
The multiplication of the pair that sums up to 2023 is: 1023130  
```

## Honestidade Académica

Nesta disciplina, espera-se que cada aluno siga os mais altos padrões de honestidade académica. Trabalhos que sejam identificados como cópias serão anulados e os alunos envolvidos terão nota zero - quer tenham copiado, quer tenham deixado copiar.
Para evitar situações deste género, recomendamos aos alunos que nunca partilhem ou mostrem o seu código.
A decisão sobre se um trabalho é uma cópia cabe exclusivamente aos docentes da unidade curricular.
Os alunos são encorajados a discutir os problemas com outros alunos mas não deverão, no entanto, copiar códigos, documentação e relatórios de outros alunos. Em nenhuma circunstância deverão partilhar os seus próprios códigos, documentação e relatórios. De facto, não devem sequer deixar códigos, documentação e relatórios em computadores de uso partilhado.

