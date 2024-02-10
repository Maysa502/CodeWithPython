
## Listas em Python

Em Python, uma lista é uma estrutura de dados versátil e fundamental que permite armazenar e organizar elementos de diferentes tipos. Listas são conjuntos ordenados de itens, onde cada item tem uma posição específica, conhecida como índice.

As listas em Python podem conter elementos de diversos tipos, como strings, números, booleanos e até mesmo outras listas. Essa flexibilidade torna as listas uma escolha poderosa para armazenar e manipular coleções de dados.

### Exemplo Básico

Considere o seguinte exemplo de uma lista de planetas no sistema solar:

```python
planetasSistemaSolar = ['mercurio', 'venus', 'terra', 'marte', 'jupiter', 'urano', 'netuno', 'plutão']
```
Neste exemplo, *'planetasSistemaSolar'* é uma lista que contém nomes de planetas. Cada elemento da lista ocupa uma posição específica, começando do índice 0. Por exemplo, 'mercurio' está no índice 0, 'venus' está no índice 1, e assim por diante.

Ao longo deste aprimoramento, exploraremos diversas operações e conceitos relacionados a listas, desde acesso a elementos até inserção, remoção e manipulação de dados.

Vamos começar explorando as operações básicas de acesso a elementos em uma lista.






## Listas em Python

### Avatar

```python
avatar = ["kyoshi", "aang", "korra", "roku", "yangchen", "kurak"]
print(avatar[0].title())
```
 Python tem uma sintaxe especial para acessar o último elemento de uma lista
Essa sintaxe é bem útil, pois, com frequência, você vai querer acessar os últimos itens de uma lista sem saber exatamente o tamanho dela print(avatar[-1].title())

---
### Usando valores individuais de uma lista

Podemos usar concatenação para criar uma mensagem com base em um valor de uma lista. 
```
local = "Reino da Terra"
print("A avatar " + avatar[0].title() + " nasceu no " + local)
```

# Prática

***3.1 - Armazenar os nomes de livros e exibir um texto junto***
```
nomesLivros = ["A guerra dos Tronos", "A furia dos reis", "A canção do Sangue", "Loki", "Capitã Marvel", "Troia", "Diario de um banana"]
escritores = ["George R.R. Martin", "Anthony Ryan", "Robert Rodi", "Steve behling", "claudio moreno", "Jeffrey Patrick Kinney"]
```
```
print("O livro " + nomesLivros[0].title() + " foi escrito pelo escritor " + escritores[0].title())
#(Outros prints de livros e escritores)
```

---
### Inserindo elementos em uma lista
Você pode adicionar um novo elemento em qualquer posição de sua
lista usando o método insert(). Faça isso especificando o índice do novo
elemento e o valor do novo item
```
planeta = ['venus', 'terra', 'marte', 'jupiter', 'saturno', 'netuno']
planeta.insert(0, 'mercurio')
planeta.insert(5, 'urano')
print(planeta)
```


### Removendo elementos de uma lista
Se um usuário decidir cancelar a conta em sua aplicação web, você vai querer remover
esse usuário da lista de usuários ativos. Você pode remover um item de acordo com sua
posição na lista ou seu valor. Isso se apenas souber o valor e a posição na lista



***instrução del***
```
luas = ['Lua', 'ganimdes', 'tita', 'europa', 'io']
del luas[1]
print(luas)
```
---

### Metodo POP
 O método pop() em Python é utilizado para remover e retornar o 
elemento de uma lista em uma posição específica. A posição é passada como 
argumento para o método pop(). O método altera a lista original, 
removendo o elemento na posição indicada e ajustando automaticamente os 
índices dos elementos restantes na lista '''

***criando e exibindo a lista***
``` 
dobras = ['fogo', 'terra', 'agua', 'ar']  
print(dobras) 

poped_dobras=dobras.pop() #fazemos pop de um valor da lista e o armazenamos na variável poped_dobras
print(dobras)  # Exibimos a lista  para mostrar que um valor foi removido da lista
print(poped_dobras) # Então exibimos o valor removido 
```

*Metodo pop sem indicação de posição remove o ultimo valor e a armazena na variavel*

---
---

### DEL X POP 
Del remove permanentemente o valor de uma lista enquanto o metodo pop guarda em uma variável
Se você não tiver certeza se deve usar a instrução del ou o método
pop(), eis um modo fácil de decidir: quando quiser apagar um item de
uma lista e esse item não vai ser usado de modo algum, utilize a
instrução del; se quiser usar um item à medida que removê-lo, utilize o
método pop()

```
planetasSistemaSolar = ['mercurio', 'venus', 'terra', 'marte', 'jupiter', 'urano', 'netuno', 'plutão']
removidoPop = planetasSistemaSolar.pop()
print("Aqui está uma lista de planetas do nosso Sistema Solar: ", planetasSistemaSolar, "\nLista de corpos celestes rebaixados a pequenos planetas:", removidoPop.title() + ".")
```

---
---









### Removendo um Item de Acordo com o Valor 

Às vezes, você não saberá a posição do valor que quer remover de uma
lista. Se conhecer apenas o valor do item que deseja remover, o método
`remove()` poderá ser usado.

***Removendo um Item***

```python
planetasSistemaSolar.remove('terra')
removePlaneta = 'terra'  # Trabalhando na adição de variável após o item ter sido removido pelo método remove
print(planetasSistemaSolar)
print("Mostrar o planeta removido: ", removePlaneta.title())
```
---
## Atividades Didáticas
*1) Lista de Convidados*
```
lista = ['Cleopatra', 'Alexandre o Grande', 'Leonardo Da Vinci', 'Albert Einstein']
print("Ola sr(a) ", lista[0], "\nGostaria de participar de um jantar beneficiente neste sabado? \nAguardo o retorno, Maysa Arruda" )
print("Ola sr(a) ", lista[1], "\nGostaria de participar de um jantar beneficiente neste sabado? \nAguardo o retorno, Maysa Arruda" )
print("Ola sr(a) ", lista[2], "\nGostaria de participar de um jantar beneficiente neste sabado? \nAguardo o retorno, Maysa Arruda" )
print("Ola sr(a) ", lista[-1], "\nGostaria de participar de um jantar beneficiente neste sabado? \nAguardo o retorno, Maysa Arruda" )
```

---

*2) Alterando a Lista de Convidados*

```

lista.remove('Albert Einstein')  # Removendo Albert
convidadoRemovido = 'Albert Einstein'  # Acrescentando em uma variável de valor para que fique guardada e usada no print abaixo
lista.insert(5, 'Isaac Newton')  # Acrescentando Isaac à lista com insert
print("Infelizmente o ", convidadoRemovido, " não poderar comaprarecer. Segue a lista corrigida com um novo convidado",lista)
print("Ola sr(a) ", lista[0], "\nGostaria de participar de um jantar beneficiente neste sabado? \nAguardo o retorno, Maysa Arruda" )
print("Ola sr(a) ", lista[1], "\nGostaria de participar de um jantar beneficiente neste sabado? \nAguardo o retorno, Maysa Arruda" )
print("Ola sr(a) ", lista[2], "\nGostaria de participar de um jantar beneficiente neste sabado? \nAguardo o retorno, Maysa Arruda" )
print("Ola sr(a) ", lista[-1], "\nGostaria de participar de um jantar beneficiente neste sabado? \nAguardo o retorno, Maysa Arruda" )
```
---
*3) Exibindo uma Lista de Forma Mais Elegante*
```

listaDois = ["galileu galilei", "nicolas copérnico", "johannes kepler", "isaac newton", "edmond halley", "carl sagan"]
listaDois.append('kopper')  # Adicionando pelo método append
for astronomo in listaDois:
    print(astronomo.title())
```
---
*4) Reduzindo convidados*
```

print("\n")

print(listaDois) 
# removendo os convidados um a um e colocando uma mensagem avisando
r1 = listaDois.pop()
print("Infelizmente, o sr ",r1.title(),"foi desconvidado para o jantar")
r2 = listaDois.pop()
print("Infelizmente, o sr ",r2.title(),"foi desconvidado para o jantar")
r3 = listaDois.pop()
print("Infelizmente, o sr ",r3.title(),"foi desconvidado para o jantar")
r4 = listaDois.pop()
print("Infelizmente, o sr ",r4.title(),"foi desconvidado para o jantar")
r5 = listaDois.pop()
print("Infelizmente, o sr ",r5.title(),"foi desconvidado para o jantar")
# mostrando os dois ultimos que restaram
for convidadosReal in listaDois:
    print("O convidado para o jantar será o senhor: ",convidadosReal.title())
# removendo esses dois ultimos
del listaDois[1]
del listaDois[0]
print(listaDois)
```
---

# Atividades 

<!--29/01/24 - Segunda-Feira-->

*Usando o Método sort()*

```python
avatar2 = [
    'Wan',
    'Yangchen',
    'Kuruk',
    'Kyoshi',
    'Roku',
    'Aang',
    'Korra'
]

avatar2.sort()
print(avatar2)
```
---
**Reverse=True deixa a lista em ordem alfabética invertida**
```
avatar2.sort(reverse=True)
print(avatar2)
```

---
### ORDENANDO UMA NOVA LISTA TEMPORARIAMENTE COM A FUNÇÃO SORTED()
```
print("\n\tA lista original: ", avatar2)
print("\n\tAgora uma outra lista colocando os elementos em ordem alfabética: ", sorted(avatar2))
print("\n\tNovamente a lista original: ", avatar2)
print("\n")
```

---
---
### Sort x Sorted
Em resumo, sort() altera a lista original, enquanto sorted() cria uma nova lista 
ordenada sem modificar a lista original. Escolher entre eles depende do que você precisa 
fazer com os dados e se deseja ou não preservar a ordem original da lista.
A função sorted, também pode aceitar um argumento reverse=True se você quiser exibir 
uma lista em ordem alfabética inversa

---
---


### EXIBINDO UMA LISTA EM ORDEM INVERSA
```
avatar2.reverse()
print("\n", avatar2)
```

---
---

SORT(REVERSE) x REVERSE
```
LISTA=[2,6,3,8]
```
* sort(reverse=True) ordena os elementos em ordem decrescente [8,6,3,2] 

* enquanto reverse() inverte a ordem dos elementos sem ordená-los [8,3,6,2]. 
Ambos os métodos modificam a lista original.

---
---


###  Função len()
```
print(len(avatar2))
```
A função len mostrará quantos elementos tem uma lista. Esse método é útil para descobrir o número de usuários registrados em um site, entre outras tarefas.

----

<!---02/02/24 - Sexta-Feira-->

# Atividade
```
lugares = ['japão', 'china', 'egito', 'nova york', 'noruega']
print(lugares)
```

***usando sorted()***
```
lugaresDois = sorted(lugares)
print(lugaresDois)  # Criando uma nova lista
print(lugares)  # Lista original novamente
```

---
*usando o modo reverse()*
```
lugares.reverse()
print(lugares)
```
aqui é um jogo de troca & troca, reverte e desreverte a lista novamente

```  
lugares.reverse()
print(lugares)
```
---
*usando o método sort()*

    lugares.sort()
    print(lugares)
    lugares.sort(reverse=True)  # colocando a lista em ordem alfabética inversa
    print(lugares)

---

### Utilizando len()
O método len() em Python é utilizado para obter o comprimento (número de elementos) de um objeto iterável, como uma lista, tupla, string, dicionário, etc. Ele retorna a quantidade de elementos presentes no objeto. Exemplo:

    cientistas = [
    'Isaac Newton',
    'Albert Einstein',
    'Galileu Galilei',
    'Charles Darwin',
    'Marie Curie',
    'Niels Bohr',
    'Leonhard Euler',
    'Louis Pasteur',
    'Alan Turing',
    'Copérnico',
    'Max Planck',
    'Ada Lovelace',
    'Richard Feynman',
    'Gregor Mendel',
    'Stephen Hawking'
    ]
    print("A lista de convidados para o jantar referente ao dia 10 de novembro deste ano contém", len(cientistas), "cientistas")

------
---


---
<!-- 5/02/24 - Segunda-Feira-->

# Capitulo 3 - Trabalhando com listas 


Quando usar laços pela primeira vez, tenha em mente que o conjunto
de passos será repetido, uma vez para cada item da lista, não importa
quantos itens haja na lista. Se você tiver um milhão de itens em sua 
lista. Python repetirá esses passos um milhão de vezes – e 
geralmente o fará bem rápido.

```
avatares = ['korra', 'aang', 'kyoshi']
for avatar in avatares:  # “para todo avatar na lista de avatares, exiba o nome do avatar”
    # print(avatar.title())
    print(avatar.title()+" é um ótimo avatar ")
    print("É sempre bom ver um avatar competente como "+avatar.title()+"\n")
print("Obrigada todos pelo ótimo papel em assegurar a humanidade :")
```
---
---

### Indentação de linhas
```
mensagem = "Ola mundo"
     print(mensagem)
```
Se você, acidentalmente, indentar uma linha que não precisa ser
indetada, Python o informará a respeito da indentação inesperada:
```
hello_world.py message = "Hello Python world!"
 u print(message) Não precisamos indentar a instrução print em u, pois ela
 não pertence à linha antes dela; assim, Python informa esse erro: File
 "hello_world.py", line 2
 print(message) ^
 IndentationError: unexpected indent Você pode evitar erros inesperados de indentação ao indentar apenas quando houver um motivo específico para isso. 
 ```
 Nos programas que estamos escrevendo no momento, as únicas linhas
 que precisam ser indentadas são as ações que queremos repetir para cada
 item em um laço for.

---
---

### FAÇA VOCÊ MESMO

**1) Pense em pelo menos três tipos de pizzas favoritas. Armazene os
nomes dessas pizzas e, então, utilize um laço for para exibir o nome de cada
pizza.**
```
pizzas = ['calabreza','brocolis','portuguesa']
for pizza in pizzas:
    print(pizza.title())
```
---
**2) Modifique seu laço for para mostrar uma frase usando o nome da pizza em vez de exibir apenas o nome dela. Para cada pizza, você deve ter uma linha na saída contendo uma frase simples**
```
for pizza in pizzas:
    print("\nEu amo pizza de",pizza)
```
---
**3) Acrescente uma linha no final de seu programa, fora do laço for, que informe quanto você gosta de pizza. A saída deve ser constituída de três ou mais linhas sobre os tipos de pizza que você gosta e de uma frase adicional**
```
print("Gosto muito de pizza, mas essas em questão,", pizzas[0],",",pizzas[1],",",pizzas[2],",")
print("são as minhas preferidas :")
```
---
**3) Pense em pelo menos três animais diferentes que tenham uma característica em comum. Armazene os nomes desses animais em uma lista e, então, utilize um laço for para exibir o nome de cada animal.**
```
animais = ['gato','cachorro','hamster']
for animal in animais:
    print("\n",animal.title(),"seria um ótimo animal de estimação\n")

print("\nNa verdade, qualquer um desses seria um ótimo animal de estimação\n")
```
---
---
#### ***RANGE***
A função range() faz Python começar a contar no primeiro valor que você lhe fornecer e parar quando atingir o segundo valor especificado
```
for valor in range(1,6): # sempre subtrai -1 da sequência, isso ajuda a não dar erros de redundância
     print(valor)
```

 
Se quiser criar uma lista de números, você pode converter os resultados de range() diretamente em uma lista usando a função list()
```
numeros = list(range(1,6))
 print(numeros)
```
Utilizando a função range() para gerar uma lista de números de 7 a 37. Somando +7
```
numeros = list(range(7,37,7)) #7 é o numero inicial, 37 é o numero final e o 7 é a ordem de contagem
print(numeros) # imprimindo a lista de resultado 
```
----
### Colocando os dez primeiros quadrados perfeitos em uma lista
Quadrados perfeitos são números inteiros que são o resultado da multiplicação de um número por ele mesmo
```
quadrados = []  # lista vazia
for valor in range(1, 11):  # condicionando a for 
    quadrado = valor ** 7  # adicionando uma variável e colocando a função exponencial nela 
    quadrados.append(quadrado)  # adicionando a variável na lista através do método append 
print(quadrados)  # exibindo a saída de dados, importante tirar o print do for
```


#### código de modo mais conciso
```
quadrados = []
for quadrado in range(1, 11):
    quadrados.append(quadrado**2)  # não utilizando o modo variável e adicionando a condição dentro do append
print(quadrados)
```


---
<!--08/02/24 - Quinta-Feira-->

**Algumas funções Python são específicas para listas de números. Por
exemplo, podemos encontrar facilmente o valor mínimo, o valor
máximo e a soma de uma lista de números:** 
```
digits = [1, 2, 3, 4, 5, 6, 7, 8, 9, 0]
valorMin = min(digits)  # 0
valorMax = max(digits)  # 9
somaNum = sum(digits)  # 45
```
---
### List comprehensions 

Uma list comprehension (abrangência de lista) permite gerar essa mesma lista com apenas uma linha de código. Uma list comprehension combina o laço for e a criação de novos elementos em uma linha, e concatena cada novo elemento automaticamente
```
quadrados2 = [value**2 for value in range(1, 11)]  # value é a expressão que eleva ao 2
print(quadrados2)
```