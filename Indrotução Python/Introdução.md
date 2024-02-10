


# Python Learning Notes

Bem-vindo ao meu repositório de aprendizado em Python! Este projeto contém anotações, atividades e exemplos que documentam minha jornada de estudo em Python.

## Registros de Estudo

#### ☆ Livro: Curso Intensivo de Python de Eric Matthes
---

<!--22/12/23 - Sexta-Feira-->
<!-- -->

## Primeiro HELLO WORLD!
```python
mensagem = "Hello Word!!!"
print(mensagem)

mensagem = "Ola mundo do Curso Intensivo de Python!"
print(mensagem)
```


**Contatenado variaveis**
```
nome = "Maysa"
sobrenome = "Arruda"
nomeCompleto = nome + " " + sobrenome
print(nomeCompleto)
```

**Deixando o Código Mais Elegante**
```
print("Tipos de linguagens de programação: \n\tPython\n\tC\n\tJavaScript")
```
<!--11/01/24 - Quinta-Feira -->

## Atividade Didática

***Mensagem Pessoal***
```
nome = "marcella arruda"
print("Olá " + nome + ", você gostaria de aprender python hoje?")
```
***Deixando o Nome Mais Elegante***
```
print(nome.title())
```

***Citação***
```
autor = "Martha Medeiros"
citacao = "O universo nunca entrega o que promete. Aliás, ele nunca prometeu nada, você é que escuta vozes."
print("\tA " + autor + " certa vez disse:" "\n\t" + citacao)
```


# Mini Projeto: Catálogo Avatar
```
print("☆ ☆ ☆ Seja bem-vindo ao catálogo dos Avatares! ☆ ☆ ☆ \n\nInsira os dados do seu Avatar:")
nome = input("Qual é a era deste Avatar?: ")
idade = input("Quantos anos esta era durou?: ")
local = input("Em qual nação iniciou esta nova era?: ")
antes = input("Qual foi sua era antecessora?: ")
depois = input("E qual foi sua era sucessora?: ") 
guia = input("Quem foi seu principal guia?: ")
print("\n\n\tAvatar " + nome.title() + " dono de uma jornada que ultrapassou " + str(idade) + " anos, emerge das raízes do " + local.title() +  ". Em seu ciclo prévio, desempenhou o papel de Avatar " + antes.title() + ", e após o término de seu ciclo, sua próxima sucessora será a era " + depois.title() + ". \n\tA vida desenrola-se como uma tapeçaria intricada, onde os fios do passado tecem os padrões do presente. Cada interação, cada escolha, ressoa como suaves ondulações em um lago, guiando o curso da existência. " + nome.title() + " teve vários guias espirituais que influenciaram sua era, nessa jornada fascinante, sua principal referência foi " + guia.title() + ", cuja sabedoria transcendente e orientação compassiva foram faróis a iluminar os momentos mais sombrios. Suas palavras, como pérolas de sabedoria, foram entrelaçadas no tecido da alma do avatar atual, perpetuando uma herança espiritual eterna.\n\n")
```
<!-- 25/01/24 - Quinta-Feira-->
***Operações Resultando em 8***
```
print(5+3)
print(12-4)
print(2*4)
print(16/2)
```
***Número Favorito***
```
fav = 7
print("\nMeu número favorito é",fav)
```
***Calculadora Simples***
```
n1 = input("Digite um número: ")
n2 = input("Digite outro número: ")

n1=int(n1)
n2=int(n2)

r1=n1+n2
r2=n1-n2
r3=n1*n2
r4=n1/n2

resultado = r1, r2, r3, r4
print("O resultado das operações são: ", resultado)
```

***Verificação de Números Ímpares ou Pares***
```
numero = input("Digite um número: ")
numero = int(numero) %2 ==0

if (numero):
    print("Este é um algarismo par")
else:
    print("Este algarismo é ímpar")
```

***Média dos Alunos***
```
Isemestre = float(input("Digite a nota do primeiro semestre: "))
IIsemestre = float(input("Digite a nota do segundo semestre: "))
IIIsemestre = float(input("Digite a nota do terceiro semestre: "))
IVsemestre = float(input("Digite a nota do quarto semestre: "))

media = (Isemestre + IIsemestre + IIIsemestre + IVsemestre) / 4
media = float(media)

if (media >= 6):
    print("O aluno está aprovado "):
elif (media >= 4 < 6 ):
    print("O aluno está de recuperação :")
else:
    print("O aluno está reprovado")
```
---
### Zen of Python by Tim Peters

#### Import this

*Bonito é melhor que feio.
Explícito é melhor que implícito.
Simples é melhor que complexo.
Complexo é melhor que complicado.
Linear é melhor que aninhado.
Esparso é melhor que denso.
Legibilidade conta.
Casos especiais não são especiais o bastante para quebrar as regras.
Ainda que praticidade vença a pureza.
Erros nunca devem passar silenciosamente.
A menos que sejam explicitamente silenciados.
Diante da ambiguidade, recuse a tentação de adivinhar.
Deveria haver um — e preferencialmente só um — modo óbvio de fazer algo.
Embora esse modo possa não ser óbvio a princípio, a menos que você seja holandês.
Agora é melhor que nunca.
Embora nunca seja muitas vezes melhor que *agora* mesmo.
Se a implementação é difícil de explicar, é uma má ideia.
Se a implementação é fácil de explicar, pode ser uma boa ideia.
Namespaces são uma grande ideia — vamos ter mais dessas!*


Fique à vontade para explorar, clonar o repositório e contribuir se quiser compartilhar suas próprias anotações ou melhorar as existentes. Boa jornada de aprendizado em Python!

