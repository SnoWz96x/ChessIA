# Chess AI para Chess.com ♟️🤖

Uma poderosa extensão para navegador que aprimora o Chess.com com análise integrada do Stockfish, fornecendo sugestões profissionais de jogadas, avaliações e opções de jogo automatizado. 🚀

![Chess AI Demo](https://raw.githubusercontent.com/allanaltarugio/ChessIA/refs/heads/main/demo.gif)

> **Novo Recurso:** O Chess AI agora suporta uma interface em janela externa que permite controlar o motor em uma janela ou aba separada, oferecendo uma experiência mais limpa no Chess.com e opções avançadas de visualização!

---

## ✨ Funcionalidades

- **Análise Avançada de Movimentos:** O motor Stockfish integrado avalia posições em tempo real ⚡️  
- **Indicadores Visuais de Movimento:** Mostra os melhores lances com destaques ou setas no tabuleiro 🎯  
- **Força Ajustável do Motor:** Defina o ELO entre 1000–3000 para combinar com seu nível 🏆  
- **Barra de Avaliação Dinâmica:** Representação visual da vantagem com cores personalizáveis 📊  
- **Histórico de Movimentos:** Registra lances analisados com avaliação e profundidade 📜  
- **Modo Humano:** Faz a engine jogar como um humano, com tempo natural e erros ocasionais 🧑‍🦱  
- **Fusion Mode:** Ajusta automaticamente a força da engine para combinar com o rating do oponente ⚖️  
- **Auto Run & Auto Move:** Opcionalmente automatiza análise e execução de jogadas 🤖  
- **Controle Completo por Teclado:** Acesso rápido a todas as profundidades via atalhos ⌨️  
- **Interface em Janela Externa:** Controle o Chess AI em outra janela ou aba 🪟  
- **Exibição de Múltiplos Movimentos:** Veja os 3–5 melhores lances com opacidade indicando força 🔢  
- **Configurações Completas:** Interface e comportamento totalmente personalizáveis ⚙️  

---

## 📥 Instalação

1. Instale um gerenciador de userscript:
   - [Tampermonkey](https://www.tampermonkey.net/) (Chrome, Firefox, Edge, Safari) 🐒  
   - [Violentmonkey](https://violentmonkey.github.io/) (Chrome, Firefox) 🙈  

2. Instale o Chess AI clicando [aqui](https://github.com/SnoWz96x/ChessIA/raw/main/Chess-AI.user.js)
2. Instale o Chess AI clicando [aqui]()

3. Acesse o [Chess.com](https://www.chess.com/play) e a ferramenta será ativada automaticamente 🎉  

---

## 📖 Guia de Uso

### **Início Rápido**
1. Vá ao Chess.com e inicie ou entre em uma partida  
2. Pressione uma tecla (Q–M) para analisar em diferentes profundidades  
3. O melhor movimento será destacado no tabuleiro  
4. Use a barra de avaliação à esquerda para ver quem está melhor  

---

### **Controles Detalhados**

#### **Profundidade da Engine**
- **Teclas Q–Z**: executa análises de profundidade 1–26  
  - Q = profundidade 1 (mais rápida, mais fraca) 💨  
  - Z = profundidade 20 (mais lenta, mais forte) 🐢  
  - **=** = profundidade máxima ♾️  

#### **Painel de Configurações**  
Organizado em abas:

- **Engine:** profundidade, ELO, livro de aberturas, repertório  
- **Actions:** iniciar/parar engine, salvar configurações  
- **Visual:** cores da barra, setas, configurações da janela externa  
- **Play Style:** Modo Humano e Fusion Mode  
- **Auto:** análise automática e jogadas automáticas  

---

### **Livro de Aberturas & Repertórios**

Inclui:

- **Classificação Dinâmica**  
- **Repertório Misto**  
- **1.e4 (King's Pawn)**  
- **1.d4 (Queen's Pawn)**  
- **Inglês (1.c4 / 1.Nf3)**  
- **Aberturas de Flanco / Hipermodernas**  

---

### **Modo Humano**

- Níveis ajustáveis: 800 → 2400 ELO  
- Tempo de pensamento realista 🤔  
- Erros naturais 😕  
- Blunders raros 🤯  

---

### **Fusion Mode**

Adapta automaticamente a força do motor ao rating do oponente.

---

### **Interface Externa**

#### **Como configurar:**

1. Ative **“Open GUI in external window”**  
2. Baixe o arquivo Python  
3. Execute:
```
python chess_ai_server.py
```
4. Clique em **Start Local Server**  
5. Clique em **Open External Window**  

---

## ⌨️ Atalhos de Teclado

| Tecla | Função | Nível |
|------|--------|--------|
| Q–E | Profundidades 1–3 | Beginner |
| R–P | Profundidades 4–10 | Intermediate |
| A–G | Profundidades 11–15 | Advanced |
| H–L | Profundidades 16–19 | Expert |
| Z–M | Profundidades 20–26 | Master |
| = | Profundidade máxima | Grandmaster |

---

## 👍 Dicas & Truques

- Depths 5–10 → melhor equilíbrio  
- Depths 15+ → análises críticas  
- Ative destaques persistentes  
- Use a janela externa para organização  
- Modo Multimovimentos para estudo  
- Ajuste estilos das setas  

---

## ⚠️ Aviso

Ferramenta para estudo e uso casual.  
Evite usar em partidas ranqueadas — pode violar os termos do Chess.com.

---

## 🙌 Créditos

- Criado por [SnoWz96x](https://github.com/SnoWz96x)  
- Baseado no [Stockfish](https://stockfishchess.org/)  

---

## 📜 Licença

Uso pessoal apenas. Não distribuir.



