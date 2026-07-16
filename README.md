# Baralho & Probabilidade

Simulador educacional de cartas desenvolvido com HTML, CSS e JavaScript para estudo de lógica de programação, combinações e probabilidades.

> Este projeto não envolve apostas, dinheiro real ou premiações. Seu uso é exclusivamente educacional.

## Visão do projeto

A aplicação utiliza a estrutura do Texas Hold'em como contexto didático para demonstrar embaralhamento, distribuição de cartas e identificação de combinações.

## Funcionalidades

- Criação de um baralho de 52 cartas
- Embaralhamento com o algoritmo Fisher–Yates
- Distribuição das cartas do participante
- Exibição progressiva das cartas comunitárias
- Identificação de combinações
- Reinício completo da simulação
- Interface responsiva

## Competências demonstradas

- Manipulação do DOM
- Estruturas de dados em JavaScript
- Algoritmos de embaralhamento
- Eventos e controle de estado
- Regras condicionais
- Desenvolvimento web responsivo

## Como executar

1. Clone o repositório:

```bash
git clone https://github.com/mildestinos/powerbinareal.git
```

2. Abra o arquivo `index.html` em um navegador moderno.

## Estrutura lógica

- `initializeDeck()`: cria o baralho
- `shuffle(array)`: embaralha as cartas
- `distributePlayerHand()`: distribui as cartas iniciais
- `dealCommunityCards(number)`: controla as cartas comunitárias
- `identifyBestHand(cards)`: avalia a combinação disponível
- `resetGame()`: reinicia o estado da aplicação

## Roadmap

- Aprimorar a avaliação das combinações
- Exibir explicações didáticas sobre probabilidades
- Criar testes automatizados para as regras
- Renomear o repositório para refletir o posicionamento educacional

## Autor

Desenvolvido por [Eric Vieira](https://github.com/mildestinos).
