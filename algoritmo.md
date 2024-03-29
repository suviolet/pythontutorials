# ----- Tutorial Python -----
##  Conceitos
### 1. Algorítmo
Algoritmo é um conceito matemático antigo, composto geralmente por uma sequência finita de ações executáveis explícitas com o intuito de obter uma solução para um problema, como por exemplo: um algoritmo capaz de calcular números de 1 a 10 e retornar à visualização de uma tabuada diagramada, permitindo fácil leitura do usuário.

Ou até mesmo instruções passo a passo para executarmos uma tarefa, como por exemplo: uma receita de bolo ou uma simples troca de lâmpada.

Alguns algoritmos são mais complexos do que outros, sendo possível criar processos de decisões através da lógica e até mesmo repetir alguns trechos de acordo com a necessidade, como no exemplo da tabuada (colocarei exemplo do código em breve).

***

- **Exemplo de algorítmo: Como abrir uma porta**
```
1   tento com uma mão girar a maçaneta,

2   está trancada? Sim/ Não?(estrutura de condição) -- Sim
(executo o comando da condição verdadeira -- Sim)

3   possuo a chave dela? Sim/ Não?(condição) -- Sim

4   está no bolso? Sim/ Não?(condição) -- Não
(executo o comando da condição falsa -- Não)

5   na mochila? Sim/ Não?(condição) -- Sim

6   abro o zíper da mochila, pego a chave com a minha mão.
(Se a mochila tiver muitos bolsos, capaz de ter que abrir todas e
verificar onde está a chave, com isso teria que repetir trechos
do código (estrutura de repetições) até a condição ser verdadeira.)

7   puutz num mesmo chaveiro possui várias chaves.
(caso não soubesse a chave correta, teria outro laço de repetição
testando uma por uma até achar a correta)

8   pego a chave correta,

9   coloco a chave no trinco,

10  giro a chave até destrancar
(geralmente lado direito)

11  seguro a maçaneta com a mão

12  giro a maçaneta até destravar a porta

13  com a mesma mão empurro a porta
```

*Está pronto =)*

***
- Cansativo e robótico não?

Num algoritmo precisamos levar em conta todos os passos necessários a serem executados para atingir o objetivo. Caso não esteja correto os dados finais, refinamos o código até tudo funcionar corretamente.

- Como um algorítmo é interpretado (por pessoas / computador)?

Linha por linha, seguindo a ordem pela qual é apresentada, respeitando laços de repetição e condições.

***
Mas para que o computador consiga ler um algoritmo precisamos utilizar uma `linguagem de programação`.


***
#### Diferentes tipos de algoritmos:

- algoritmo determinístico  

Algoritmo que sempre produz o mesmo resultado/valor dado uma determinada entrada de dados, ou seja, se comporta da mesma maneira em distintas execuções de um mesmo algoritmo.
Considerado um dos tipos mais comuns. 

ex:  
```python
>>> a = 2
>>> b = 3
>>> c = a + b
>>> c
5
```


- algoritmo não determinístico  

Algoritmo que produz resultados diferentes mesmo com a mesma entrada de dados, ou seja, se comporta de maneira distinta em diversas execuções do mesmo algoritmo.
Se um código necessita de um fator externo aleatório para uma execução ele é considerado não determinístico.

ex  

```python
>>> import datetime # módulo do python para tipos básicos de data e hora
>>> a = datetime.datetime.now()
>>> a = a.day
>>> a # código escrito num dia 21
21 
>>> b = 3
>>> c = a + b
>>> c
24
# o resultado desse código varia de acordo com a data em que será executado
```

- algoritmo probabilístico  

Algoritmo que produz resultados diferentes devido à entrada de dados ser gerada com base em números pseudo-aleatórios, ou seja, se comporta de forma distinta em diversas execuções justamente por receber dados aleatórios como entrada, tendo diversas probabilidades de resultados.

ex:  
```python
>>> import random # módulo do python para geração de números pseudo-aleatórios
>>> a = random.randint(1,10)
>>> a # nessa execução saiu o número 5
5
>>> b = 3
>>> c = a + b
>>> c
8
# o resultado desse código varia de acordo o número escolhido aleatoriamente durante sua execução
```

- algoritmo concorrente  

Algoritmo que permite a execução de dois ou mais processos simultaneamente sem gerar conflitos.

ex:   
```
Diversos workers que fazem a mesma coisa, 
pegam conteúdo da fila para processar e armazenam o conteúdo processado em algum lugar X.

Como no caso do cinema, uma fila de usuários esperando ser atendidos por uma série de atendentes (workers), 
executando algoritmos concorrentes e armazenando os dados de seleção e compra de cada usuário num banco de dados no sistema.
```





