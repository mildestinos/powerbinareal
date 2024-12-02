# **Simulador de Pôquer Texas Hold'em**

Este projeto é uma **simulação de pôquer Texas Hold'em** criada para fins de aprendizado em **HTML, CSS e JavaScript**. Ele foi desenvolvido como uma forma prática de entender conceitos básicos de desenvolvimento web enquanto exploro as regras e mecânicas do pôquer.



## **Funcionalidades**
- Exibição de cartas comunitárias (Flop, Turn e River).
- Distribuição automática de cartas para o jogador.
- Identificação de combinações básicas de pôquer (Par, Dois Pares, Trinca, etc.).
- Interface visual com destaque para jogadas interessantes.
- Design responsivo para diferentes dispositivos.


## **Principais Funções do Código**

### **1. `initializeDeck()`**
- **O que faz:** Cria e embaralha um baralho completo de cartas (52 cartas, com valores e naipes).
- **Como funciona:** 
  - Combina os valores (`A, 2, 3... K`) com os naipes (`♠, ♥, ♦, ♣`) para formar todas as cartas possíveis.
  - Chama a função `shuffle` para embaralhar o baralho.


### **2. `shuffle(array)`**
- **O que faz:** Embaralha as cartas do baralho usando o algoritmo de Fisher-Yates.
- **Como funciona:** 
  - Troca os elementos do array de forma aleatória.
  - Garante que o baralho esteja em uma ordem diferente a cada vez que o jogo for reiniciado.


### **3. `resetGame()`**
- **O que faz:** Reinicia o jogo, redefinindo as cartas do jogador e comunitárias, além de reabilitar os botões para iniciar uma nova rodada.
- **Como funciona:** 
  - Limpa as áreas de exibição (`communityCardsContainer` e `playerCardsContainer`).
  - Exibe mensagens padrão nas áreas de explicação e sugestões.
  - Recria o baralho chamando `initializeDeck()` e distribui novas cartas ao jogador.


### **4. `distributePlayerHand()`**
- **O que faz:** Distribui duas cartas ao jogador.
- **Como funciona:** 
  - Remove duas cartas do topo do baralho.
  - Exibe essas cartas na seção de "Suas Cartas" (`playerCardsContainer`).


### **5. `dealCommunityCards(number)`**
- **O que faz:** Distribui as cartas comunitárias (Flop, Turn ou River) conforme o número especificado.
- **Como funciona:** 
  - Remove a quantidade de cartas do baralho (`number`).
  - Exibe essas cartas na seção "Cartas Comunitárias" (`communityCardsContainer`).


### **6. `checkBestHand()`**
- **O que faz:** Avalia a melhor combinação de cartas entre as do jogador e as comunitárias.
- **Como funciona:** 
  - Combina as cartas do jogador com as comunitárias.
  - Chama a função `identifyBestHand()` para determinar a melhor combinação possível.
  - Exibe o resultado na área de explicação.


### **7. `identifyBestHand(cards)`**
- **O que faz:** Analisa todas as cartas disponíveis e identifica combinações, como Par, Trinca, Full House, etc.
- **Como funciona:** 
  - Conta a frequência de cada valor de carta.
  - Usa as contagens para identificar combinações específicas (Par, Trinca, Quadra, etc.).
  - Retorna o nome da melhor combinação encontrada.


### **8. Botões de Controle**
- **`dealFlopButton`:** Exibe as 3 primeiras cartas comunitárias (Flop).
- **`dealTurnButton`:** Exibe a 4ª carta comunitária (Turn), ativado após o Flop.
- **`dealRiverButton`:** Exibe a 5ª carta comunitária (River), ativado após o Turn.
- **`resetGameButton`:** Reinicia o jogo, ativando o ciclo novamente.


## **Como Usar**
1. **Clone ou baixe o repositório:**
   ```bash
   git clone https://github.com/SEU_USUARIO/NOME_DO_REPOSITORIO.git
   ```
2. **Abra o arquivo `index.html`** no navegador.


## **Próximos Passos**
- Adicionar funcionalidades para múltiplos jogadores.
- Implementar regras completas de avaliação de mãos.
- Melhorar o design visual e as animações.


## **Contribua**
Se você tem sugestões ou deseja ajudar a melhorar o projeto, fique à vontade para abrir uma **issue** ou enviar um **pull request**. Sua colaboração é muito bem-vinda!


**Autor**: Eric Vieira  
