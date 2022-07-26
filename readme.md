# Teste de integração

Estamos democratizando a saúde no Brasil, somos apaixonados por inovação. Vem revolucionar o mercado da saúde com a gente!

## Desafio

O objetivo desse desafio é capturar dados de pessoais para inserção em um banco de dados não relacional (MongoDB) usando Python ou NodeJS.

Requisitos:

A aplicação, que deve rodar em terminal, deve acessar a cada 1 hora a rota:
https://randomuser.me/api/?nat=br&format=csv&results=1000

A aplicação de importar os seguintes dados para um banco mongodb:
- gender
- name = first, last
- location = street [name, number], city, state
- email
- login = username, uuid
- dob (birthday) = date
- registered = date
- id (cpf) = value

Algumas regras:
- Em caso de CPF duplicado, atualizar demais dados
- Caso a url esteja fora do ar, avisa por email (ou slack, ou telegram, fique a vontade)
- A aplicação só deve parar em caso de interrupção manual

Diferenciais:
- Se usar Docker, use Dockerfile
- Rodar em ambiente Linux Alpine
- Salvar logs no banco mongo
- Código limpo e objetivo
