# 🧩 RAC Quebra-Cabeça: Reconstruindo Nossas Memórias

Um web game de quebra-cabeça romântico e interativo, criado especialmente como presente de aniversário de namoro. Este projeto faz parte do "multiverso" **RAC Games**.

O objetivo do jogo é simples, mas cheio de significado: o jogador deve arrastar as peças embaralhadas para reconstruir fotos de momentos marcantes do casal. Ao finalizar a imagem, uma declaração de amor e a memória daquele dia são reveladas!

## ✨ Destaques e Funcionalidades

* **Mecânica Drag & Drop Híbrida:** O jogo foi programado do zero em JavaScript puro para suportar tanto o clique e arraste do mouse (no computador) quanto o toque e deslize (em telas *touch* de celulares).
* **Fases Ilimitadas:** O código permite adicionar quantas fotos/fases você quiser de forma muito simples.
* **Auto-Recorte (CSS):** Não é necessário recortar as imagens em quadradinhos no Photoshop. O jogo utiliza a propriedade `background-position` do CSS para fatiar a foto perfeitamente.
* **Design Glassmorphism:** O visual segue a identidade do hub **RAC Games**, com efeito de vidro fosco, degradê animado e uma chuva de confetes na vitória.

## 🎮 Como Jogar

1. A tela exibirá um grid de 3x3 com partes de uma foto embaralhadas.
2. Toque/clique em uma peça e arraste-a para cima da peça que deseja trocar de lugar.
3. Quando todas as peças estiverem na posição correta, o grid some, a foto brilha e a mensagem especial aparece.
4. Clique em "Próxima Memória" para ir para a foto seguinte!

## 🛠️ Tecnologias Utilizadas

* **HTML5 & CSS3**
* **JavaScript Vanilla** (Lógica de estados, validação e manipulação de eventos *drag* e *touch*).
* **Tailwind CSS** (Via CDN para estilização ágil e responsividade).
* **Canvas Confetti** (Biblioteca externa para os efeitos de celebração).

## ⚙️ Como Personalizar com Suas Fotos

Se você quer utilizar este código para presentear alguém, é muito fácil colocar as suas próprias fotos:

1. Salve as suas fotos (preferencialmente no formato **quadrado**, proporção 1:1) na mesma pasta do arquivo `index.html`. Exemplo: `casal.jpg`.
2. Abra o arquivo HTML e vá até a variável `const levels` no script.
3. Substitua o campo `image` pelo nome do seu arquivo (usando caminho relativo) e o campo `message` pela sua declaração:

```javascript
const levels = [
    {
        image: "casal.jpg", 
        message: "O melhor dia das nossas vidas! Te amo."
    }
];
```

**Importante:** Na hora de hospedar (como no GitHub Pages), certifique-se de fazer o upload das imagens junto com o código HTML.

---
*Feito com muito amor, café e código. Feliz Aniversário de Namoro!* ❤️
