# Aula 02 — Python no Windows e primeiros cálculos com dados ambientais

Data: 09/08/2026
Tema: Instalação, execução de scripts, listas, repetição, condicionais e estatística descritiva básica.
Aplicação: Introdução à programação voltada para futura análise de dados ambientais.

🔵 Natureza dos dados: todos os dados ambientais utilizados nesta aula foram fictícios/didáticos. 
Eles foram criados para aprendizagem e não representam resultados de monitoramento ambiental real.

Objetivos da aula

Nesta aula, saímos dos comandos isolados no interpretador Python e começamos a trabalhar com um arquivo .py. 
Também utilizamos dados ambientais fictícios para aprender a calcular média, percorrer listas e encontrar valores máximos e mínimos.

O primeiro arquivo criado foi:

aula_01.py

E aprendemos a executá-lo pelo Prompt de Comando do Windows:

python aula_01.py
Principais termos aprendidos
Termo/comando	Tradução/significado	O que faz	Exemplo
print()	imprimir/exibir	Mostra informações na tela	print("Olá")
variável	variable	Guarda um valor associado a um nome	idade = 16
=	atribuição	Atribui um valor a uma variável	temperatura = 28.5
float	número de ponto flutuante	Representa números com parte decimal	28.5
list	lista	Armazena vários valores em uma estrutura	[28.5, 30.2, 29.1]
[0]	índice 0	Acessa o primeiro elemento de uma lista	temperaturas[0]
len()	length / comprimento	Conta quantos elementos existem	len(temperaturas)
for	para/cada	Percorre elementos de uma sequência	for temperatura in temperaturas:
if	se	Executa um bloco quando uma condição é verdadeira	if temperatura > maior:
>	maior que	Compara dois valores	31 > 30
<	menor que	Compara dois valores	27 < 30
round()	arredondar	Arredonda um número	round(29.266, 2)
indentação	indentation	Define os blocos de código em Python	espaços antes do código dentro de for e if
debugging	depuração	Processo de localizar e corrigir problemas no código	editar → executar → verificar → corrigir
.py	arquivo Python	Extensão utilizada para arquivos de código Python	aula_01.py
dir	directory	Lista arquivos e pastas no terminal do Windows	dir
mkdir	make directory	Cria uma pasta	mkdir Aprendendo_Python
cd	change directory	Entra/muda para outro diretório	cd Aprendendo_Python
Conceitos importantes

Uma lista permite armazenar vários valores em uma única variável:

temperaturas = [28.5, 30.2, 29.1, 27.9, 31.0]

Os índices começam em 0:

Índice:     0     1     2     3     4
Valor:    28.5  30.2  29.1  27.9  31.0

Portanto:

temperaturas[0]

retorna:

28.5
Percorrendo dados com for

Aprendemos a utilizar um acumulador:

soma = 0

for temperatura in temperaturas:
    soma = soma + temperatura

O for percorre os elementos. A instrução:

soma = soma + temperatura

é que realiza a soma a cada passagem.

Depois podemos contar automaticamente as observações:

quantidade = len(temperaturas)

e calcular:

media = soma / quantidade

Isso torna o programa adaptável: se adicionarmos novas temperaturas à lista, não precisamos alterar manualmente a quantidade usada no cálculo.

Arredondamento

Aprendemos uma distinção importante:

print(round(media, 2))

apenas apresenta naquele momento o resultado arredondado.

Já:

media = round(media, 2)

atribui o resultado arredondado novamente à variável media.

Exemplo:

valor = 12.456
valor = round(valor, 1)

print(valor)

Resultado:

12.5
Maior e menor valor

Também construímos algoritmos para localizar extremos sem informar previamente ao Python qual é a resposta.

Maior temperatura:

maior_temperatura = temperaturas[0]

for temperatura in temperaturas:
    if temperatura > maior_temperatura:
        maior_temperatura = temperatura

Menor temperatura:

menor_temperatura = temperaturas[0]

for temperatura in temperaturas:
    if temperatura < menor_temperatura:
        menor_temperatura = temperatura

O programa final conseguiu produzir:

Temperatura média: 29.34 °C
Maior temperatura: 31.0 °C
Menor temperatura: 27.9 °C
Código consolidado da aula

🔵 Exemplo fictício/didático ambiental.

temperaturas = [28.5, 30.2, 29.1, 27.9, 31.0]

soma = 0

for temperatura in temperaturas:
    soma = soma + temperatura

quantidade = len(temperaturas)
media = soma / quantidade

maior_temperatura = temperaturas[0]

for temperatura in temperaturas:
    if temperatura > maior_temperatura:
        maior_temperatura = temperatura

menor_temperatura = temperaturas[0]

for temperatura in temperaturas:
    if temperatura < menor_temperatura:
        menor_temperatura = temperatura

print("Temperatura média:", round(media, 2), "°C")
print("Maior temperatura:", maior_temperatura, "°C")
print("Menor temperatura:", menor_temperatura, "°C")
Erros que também viraram aprendizado

Durante os exercícios apareceram situações como:

nome = Maria

que gera erro porque Maria, nesse caso, não foi definida como variável. Para representar texto:

nome = "Maria"

Também vimos que Python diferencia letras maiúsculas de minúsculas:

Print(idade)   # incorreto
print(idade)   # correto

Durante a construção do algoritmo de temperatura mínima e máxima, os primeiros resultados ficaram incorretos e o código foi editado e executado novamente até produzir o resultado esperado. Esse processo introduziu o conceito de debugging (depuração).

Avaliação de aprendizagem

Ao final desta etapa, os conceitos que demonstraram boa compreensão foram: 
variáveis, 
atribuição, 
print(), 
listas, 
índices, 
len(), 
for, 
acumuladores, 
if, 
comparações com > e <, 
cálculo de média e 
busca de valores máximo e mínimo.

Um ponto que precisou ser retomado durante a aula foi round(), principalmente a diferença entre arredondar apenas para apresentação e atribuir o resultado arredondado novamente à variável. 
Esse conceito deverá reaparecer em avaliações futuras.

Próxima evolução: continuar Python progressivamente aplicado à análise de dados ambientais, avançando de listas simples para estruturas de dados mais próximas das utilizadas em conjuntos reais de monitoramento. 🌱🐍📊
