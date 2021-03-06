# Por que Python?
<img align="right" alt="engen" width="400" src="https://media2.giphy.com/media/coxQHKASG60HrHtvkt/giphy.gif">

Existem várias teorias do por que engenheiros de dados usam Python, elenquei algumas:
1. É uma linguagem de sintaxe menos complexa; isso gera menos código.
2. Tem muitas bibliotecas como Pandas, NumPy e SeaBorn; aumenta a possibilidade de explorarmos dados de uma forma mais simples.
3. Tem um grande poder de integração com outras plataformas; isso facilita a migração de dados.
<br />

* *Nesse repositório será postado linhas de estudo e resoluções pertinentes ao Engenheiro de Dados.
Lembrando quê: esse estudo é trabalhado no dia-a-dia, sendo um processo orgânico e evolutório, contando com uma linguagem que mescla facilitar a aprendizagem e troca de informações.*
<br />

### CONHECENDO MELHOR:

<details><summary><big><big><big><big><big><big><b>O QUE É PYTHON?</b></big></big></big></big></big></big></summary>
<br />
Python é blá, blá, blá.

</details>

<details><summary><big><big><big><big><big><big><b>O QUE SE FAZ COM PYTHON?</b></big></big></big></big></big></big></summary>
<br />
Python é blá, blá, blá.

</details>

<details><summary><big><big><big><big><big><big><b>QUEM USA PYTHON?</b></big></big></big></big></big></big></summary>
<br />
Python é blá, blá, blá.

</details>
<br />

### UTILIZANDO O PYTHON - PRIMEIROS PASSOS:
<details><summary><big><big><big><big><big><big><b>CONHECENDO VARIÁVEIS E TIPOS DE VALORES (STRING, INT, FLOAT E BOOLEAN)</b></big></big></big></big></big></big></summary>
<br />

:notebook: **VARIÁVEIS** *- são como caixas registradoras: recebem valores e os guardam na memória. Usamos as variáveis exatamente para isso, para guardarmos valores que serão usados mais tarde no código.*
> **A ESTRUTURA DA VARIÁVEL - variavel = valor**
```
nome = "Maria"
numero = 1
conta = n + x
```
  
Digamos que tenho uma conta para fazer, mas para resolver essa conta devo usar uma fórmula. Só que eu não lembro os valores númericos dessa fórmula. Então, para resolver isso, vim aqui no Python e usei as variavéis para guardar esses valores.

* `valor1 = 7`
* `valor2 = 9.8`
* `valor3 = 88.789`

Aí, toda vez que preciso resolver uma conta que usa essa fórmula, ao invés de usar os números que não lembro, uso os nomes que dei para esses valores, e esses nomes são as variáveis.

Ou seja, ao invés de lembrar a fórmula desse jeito: 
* `x = 7 * 9.8 / 88.789`

Eu lembro a fórmula deste jeito:
* `x = valor1 * valor2 / valor3`

E ambas as formas o retorno de valores é o mesmo, com a diferença de que em uma delas os valores estão implicitos na fórmula, e na outra, eu guardei os valores em uma variável para poder usar em outro momento sem correr o risco de esquecê-los.

<br />
<br />

:notebook: **TIPOS DE VALORES** - *toda vez que atribuimos valor a uma Variável, esse valor será de algum tipo. E é primordial sabermos os tipos desses valores, por que cada um deles exerce uma função diferente.*

* Por exemplo, se você quiser fazer uma conta, você não vai conseguir somar uma palavra com um número. E se por um acaso em uma variável um número estiver como "string" e o outro como "int", essa conta realmente não vai acontecer. Vamos ver por quê?
  
NOME DOS VALORES | O QUE ELE É | REPRESENTADO POR
----------- | ------ | ------
STRING | Texto | Letras, frases, textos, números, dentre outros caracteres escritos entre "aspas".
INT | Número inteiro | Números inteiros. Ex.: 7, 156, 95
FLOAT | Número decimal, também conhecido como Ponto Flutuante | Números com casas decimais. Ex.: 1.2, 7.999, 000.887
BOOLEAN | Condição | True ou False

* STRING também pode ser escrito ou conhecido como `str`.
* FLOAT também pode ser escrito ou conhecido como `Double`.
* BOOLEAN também pode ser escrito ou conhecido como `bool`.

[*EXEMPLOS DE USO*](https://github.com/Isiumlord/GlowUpDataEngineerStudy/blob/main/PythonNotebooks/Variavel-TiposDeValores.ipynb)

<br />
</details>

<details><summary><big><big><big><big><big><big><b>CONHECENDO PRINT E FORMAT</b></big></big></big></big></big></big></summary>
<br />

:notebook: **PRINT** *- é a função que imprime/exibe o que está sendo executado. É ela quem vai mostrar na tela os resultados daquilo que está sendo feito.*
> **A ESTRUTURA DO PRINT - print( )**
```
x = 77

print("Oi, você está me lendo.")
print(x)

#Impressão
Oi, você está me lendo.
77
```
<br />
<br />

:notebook: **FORMAT** *- é um método de formatação de String, ou seja, é com ele que conseguimos formatar strings de forma mais dinamica.*
> **A ESTRUTURA DO FORMAT - print("Mensagem { }".format(parametros)**

Para utiliza-lo você deve ter em mente que ele usa parametros, ou seja, você terá que ter:

* Variáveis que ditem quais os valores seram mutáveis.
* Um Print onde os valores dessas variáveis apareceram.

Tendo isso você consegue posicionar as chaves { }, que ditam a posição do valor dentro da mensagem no Print, e usar as Variáveis como parametros para fazer com que os valores correspondam as suas posições nas mensagens.
```
#Variável com dados editáveis
nome = "Haruka"
livro = "Python"

#Usando Format
print("Oi {}, você está lendo {}.".format(nome, livro))

#Impressão
Oi Haruka, você está lendo Python.
```

[*EXEMPLOS DE USO*](https://github.com/Isiumlord/GlowUpDataEngineerStudy/blob/main/PythonNotebooks/Print-Format.ipynb)

<br />
</details>

<details><summary><big><big><big><big><big><big><b>CONHECENDO INPUT, IF, ELIF E ELSE</b></big></big></big></big></big></big></summary>
<br />

:notebook: **INPUT** *- é a função que recebe dados do usuário. O Input sempre vai pedir algo a alguém; e quando ele receber esse algo, ele sempre retornará uma "String".*
> **A ESTRUTURA DO INPUT - variavel = input("mensagem")**
```
nome = input("Digite seu nome: ")
print(nome)

#Impressão
Digite seu nome:
```
<br />
<br />

:notebook: **IF, ELIF e ELSE** *- são condições que determinam qual ação o código vai executar.*
Essas três condições podem ser simplesmente entendidas como:
* IF = SE, faça isso;
* ELIF = MAS SE, faça isso;
* ELSE = SE NENHUMA DAS ANTERIORES, faça isso.

Para você conseguir visualizar melhor o que foi dito:

1.Imagine que você é segurança de uma festa na cidade, mas para deixar as pessoas entrarem na festa você tem que seguir algumas regras:
* SE (if) - a pessoa ter 18 anos ou +18, pode entrar;
* MAS SE (elif) - a pessoa ter 18 anos ou +18, e estiver visivelmente alterada, não pode entrar;
* SE NENHUMA DAS ANTERIORES (else) - não pode entrar;
[...]

[*EXEMPLOS DE USO*](n)

<br />
</details>
<br />

### *DOCUMENTO EM CONSTRUÇÃO.*
