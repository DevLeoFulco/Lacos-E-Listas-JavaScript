# README - Estudo de JavaScript: Jogo de atravessar a rua

## Introdução

Este repositório contém um estudo básico sobre JavaScript, focado na criação de um simples jogo de Atravessar a Rua. O jogo aborda diversos conceitos fundamentais da linguagem, tais como funções, laços (loops) e listas (arrays).

## Conteúdo

### Estrutura do Código

O código foi dividido em duas partes principais: o ator (personagem do jogador) e o carro (obstáculos do jogo).

#### Ator

- **Posição**: O ator é definido pelas variáveis `xAtor` e `yAtor`, que representam suas coordenadas no canvas.
  
- **Movimentação**: Utiliza as teclas de seta (UP_ARROW e DOWN_ARROW) para movimentar o ator verticalmente.
  
- **Colisão**: Verifica se o ator colidiu com algum carro e, caso positivo, retorna o ator para sua posição inicial.

#### Carro

- **Posição e Velocidade**: Os carros são definidos por arrays (`xCarros` e `yCarros`) e possuem velocidades variáveis (`velocidadeCarros`).

- **Movimentação**: Os carros se movimentam da direita para a esquerda no canvas.

### Laços (Loops)

O código utiliza laços `for` para iterar sobre arrays e executar operações em múltiplos elementos, como movimentar os carros e verificar colisões.

Exemplo:
```javascript
for (let i = 0; i < imagemCarros.length; i++){
  image(imagemCarros[i], xCarros[i], yCarros[i], comprimentoCarro, alturaCarro);
}
```

### Listas (Arrays)

Arrays são usados para armazenar múltiplos valores relacionados, como as posições dos carros e suas velocidades.

Exemplo:
```javascript
let xCarros = [600, 600, 600, 600, 600, 600];
let yCarros = [40, 96, 150, 210, 270, 318];
```

## Lógica e Funcionalidades

- **Movimentação do Ator**: A função `movimentaAtor` verifica as teclas pressionadas pelo usuário e atualiza a posição do ator.
  
- **Verificação de Colisão**: A função `verificaColisao` verifica se o ator colidiu com algum carro, e se sim, retorna o ator para sua posição inicial e toca um som.
  
- **Pontuação**: A função `marcaPonto` atualiza a pontuação do jogador e retorna o ator para sua posição inicial ao atravessar a tela com sucesso.

- **Som e Animações**: Foram utilizadas imagens (`imagemDoAtor` e `imagemCarros`) e sons (`somDaColisao` e `somDoPonto`) para enriquecer a experiência do jogo.

## Conclusão

Este estudo oferece uma introdução prática aos conceitos fundamentais de JavaScript, utilizando um exemplo de jogo simples para demonstrar como aplicar funções, laços e listas em um projeto real.

---

