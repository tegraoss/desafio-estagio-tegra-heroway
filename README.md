
# Desafio Estágio - Tegra + Heroway

<link rel="shortcut icon" type="image/x-icon" href="tegra.ico">

Olá Hero, bem vindo ao Desafio para estágio na Tegra.

Essa desafio é focado no desenvolvimento front-end, segundo conteúdo ministrado pela Heroway.
​
<img src="tegra.png" alt="Logo Tegra" width="250" />

## Objetivo​

Desenvolver uma Single Page Application (SPA) para a busca de voos.
​

## Requisitos

​
Sua aplicação deve:

- Ser desenvolvida utilizando `Typescript`, `React` e `Redux`.
- Conter uma tela onde o usuário possa selecionar o `Aeroporto de Origem`, `Aeroporto de Destino` e a `Data de Partida`, através de Dropdowns ou Pickers
- Exibir uma lista de vôos
​

Extras:

- Possibilitar a ordenação por `preço total`.
- Possibilitar a ordenação por `tempo total de vôo`.
- Calcular o `preço total` e o `tempo total de vôo`, considerando as esperas entre as escalas.
​

## API

​
Para desenvolver os requisitos acima, você deverá consumir as seguintes APIs:
​
**Lista de Aeroportos:**

 ```js
 const method = 'GET';
 const url = 'https://api-voadora.dev.tegra.com.br/flight/companies';
 ```

 Essa API te disponibilizará os dados necessários para que o usuario possa selecionar o `Aeroporto de Origem` e o `Aeroporto de Destino`.
​
​
**Lista de Vôos:**

 ```js
 const method = 'POST';
 const url = 'https://api-voadora.dev.tegra.com.br/flight';
 const body = {
    from: 'BSB', // aeroporto de origem
    to: 'VCP', // aeroporto de destino
    date: '2019-02-10' // data de partida
  }
 ```

Essa API te disponibilizará a lista de vôos disponíveis dado `Aeroporto de Origem`, `Aeroporto de Destino` e `Data de Partida`.
​

**Atenção:** Só existem dados na API entre: `2019-02-10` e `2019-02-18`.
​

## Entrega

A entrega deve ser feita em um repositório público no GitHub, que deve conter:
​

- O código do projeto
- Um arquivo **README** que descreva o que foi feito e as etapas para rodar o projeto
- Enviar o link do repositório para o seguinte email: **estagio@tegra.com.br**. No assunto, indicar "Desafio Estágio Heroway". Não esqueça de identificar o seu nome completo no corpo do email também.

​
**Importante:** Não se preocupe se não conseguir entregar todos os requisitos: dê o seu melhor! :muscle:

Boa sorte, Hero! =)
