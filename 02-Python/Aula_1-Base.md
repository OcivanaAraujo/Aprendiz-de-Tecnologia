# Aula 01 — Fundamentos de Programação com Python

Data: 07/08/2026
Nível: iniciante
Objetivo: construir uma base de lógica de programação e começar a preparar o caminho para análise de dados ambientais.

Resumo

Nesta aula foram trabalhados conceitos fundamentais de Python por meio de exercícios curtos. 
foco foi entender o que o computador guarda, compara, repete, calcula e mostra.

Conceitos consolidados

Variáveis e atribuição com =
Saída com print()
Entrada com input()
Conversão para inteiro com int()
Operações matemáticas: +, -, *, /
Comparações: ==, >=
Decisões: if e else
Repetições: for e range()
Listas
append()
len()
Dicionários
Acesso e atualização de valores em dicionários
Listas de dicionários
Acumuladores
Processamento de uma lista para gerar outra lista
Conceitos introduzidos, mas ainda precisam de avaliação
Funções com def e return
Arquivos com open(), write() e close()
Classes e objetos

Regra de aprendizagem: um conceito não será considerado definitivamente dominado por apenas um acerto. 
Ele será revisitado em situações diferentes.

Exemplo integrado estudado

alunos = [
    {"nome": "Ana", "nota": 8},
    {"nome": "João", "nota": 5},
    {"nome": "Maria", "nota": 10}
]

for aluno in alunos:
    if aluno["nota"] >= 7:
        print(aluno["nome"] + " aprovado")
    else:
        print(aluno["nome"] + " reprovado")

Saída:

Ana aprovado
João reprovado
Maria aprovado

Esse exercício combinou lista + dicionários + for + if/else + comparação + acesso a dados + print().
Situação dos exemplos
🔵 Exemplo fictício/didático. Os exemplos da aula foram criados para treinamento e não representam uma base ambiental real.
Nenhum dado sensível foi utilizado.
Direção para as próximas aulas
A aprendizagem será progressivamente direcionada para análise de dados ambientais, usando situações como:
temperatura e precipitação;
qualidade da água;
qualidade do ar;
monitoramento ambiental;
séries temporais;
indicadores ambientais;
limpeza e organização de dados;
estatística e visualização.

Quando possível, serão utilizados casos e bases reais. 
houver dados sensíveis, eles serão alterados e isso será explicitamente informado.

Próximo passo

Construir um pequeno projeto de cadastro/análise e, em seguida, migrar gradualmente para estruturas de dados usadas em análise ambiental, incluindo Pandas, limpeza de dados, estatística e visualização.
