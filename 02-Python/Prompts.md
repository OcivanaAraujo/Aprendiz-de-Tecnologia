# Prompts Aula 1

##🟢 Passo 1 — Verificar se o Python já está instalado
Windows + R
Vai aparecer uma pequena janela chamada Executar.

Digite: cmd
python --version

##🧪 Passo 2 — Nosso primeiro programa
Ainda nessa janela preta, digite: python 
>Enter

print("Olá, Python!") 
>Enter

##💻 Agora vamos preparar seu ambiente

Você já provou que o Python está funcionando. O próximo passo é instalar/configurar um editor para criar arquivos .py.

Saia do interpretador Python digitando:
exit()
>Enter

Você deve voltar para uma tela parecida com:
C:\Users\SeuNome>

## 🟢 Passo 3 — Criar a pasta das aulas

No prompt:
C:\Users\ociva>

digite exatamente:
mkdir Aprendendo_Python
>Enter

O que esse comando significa?
mkdir vem de make directory:
make = criar
directory = diretório/pasta

cd Aprendendo_Python
>Enter

cd significa change directory:
"Mude para esta pasta."
Seu prompt deverá ficar parecido com:
C:\Users\ociva\Aprendendo_Python>

Agora: primeiro arquivo Python 🐍
Como estamos começando, vamos usar primeiro uma ferramenta que já existe no Windows, sem instalar outro programa ainda.
Digite no terminal:
notepad aula_01.py
>Enter

Depois pressione Ctrl + S para salvar e feche o Bloco de Notas.

### PROMPT 
temperatura_1 = 28.5
temperatura_2 = 30.2
temperatura_3 = 29.1

soma = temperatura_1 + temperatura_2 + temperatura_3

media = soma / 3

print(media)
print("Temperatura média:", round(media, 2), "°C")
print("Temperatura:", temperatura_1, "°C")

### PROMPT Temperatura
temperaturas = [28.5, 30.2, 29.1]
print(temperaturas)
print(temperaturas[0])


temperaturas = [28.5, 30.2, 29.1]

soma = temperaturas[0] + temperaturas[1] + temperaturas[2]
media = soma / 3
print("Temperatura média:", round(media, 2), "°C")


temperaturas = [28.5, 30.2, 29.1, 27.9]
soma = 0

for temperatura in temperaturas:
    soma = soma + temperatura

quantidade = len(temperaturas)
media = soma / quantidade
print("Temperatura média:", round(media, 2), "°C")


maior_temperatura = temperaturas[0]
for temperatura in temperaturas:
    if temperatura > maior_temperatura:
        maior_temperatura = temperatura

print("Maior temperatura:", maior_temperatura, "°C")

menor_temperatura = temperaturas[0]

for temperatura in temperaturas:
    if temperatura < menor_temperatura:
        menor_temperatura = temperatura

print("Menor temperatura:", menor_temperatura, "°C")

### PROMPT 
ph = [7.1, 6.8, 7.3, 7.0]

menor_ph = ph[0]

for valor in ph:
    if valor < menor_ph:
        menor_ph = valor

print(menor_ph)

### PROMPT Oxigênio
oxigenio = [7.8, 6.9, 8.1, 7.4]
print(oxigenio[2])

### PROMPT Turbidez
turbidez = [4.2, 5.1, 3.8, 6.0, 4.5]

soma = 0

for valor in turbidez:
    soma = soma + valor

quantidade = len(turbidez)
media = soma / quantidade

round(media, 1)

print("Média:", round(media, 1))

media = 7.386
print(round(media, 2))
print(media)
