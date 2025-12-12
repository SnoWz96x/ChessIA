# Chess AI for Chess.com

♟️🤖 Uma poderosa extensão que integra o Stockfish ao Chess.com, oferecendo análise avançada, sugestões de jogadas, automação opcional e uma interface externa profissional!

---

## 🚀 Demonstração

![Demo GIF](https://raw.githubusercontent.com/allanaltarugio/ChessIA/refs/heads/main/demo.gif)

---

*Inclua aqui uma imagem ou GIF da ferramenta em ação (opcional)*

---

## ✨ Funcionalidades

* **Análise Avançada de Lance**: Stockfish integrado avaliando posições em tempo real ⚡️
* **Indicadores Visuais**: Destaques e setas mostrando o melhor movimento 🎯
* **Força Ajustável**: Escolha níveis de ELO entre 1000 e 3000 🏆
* **Barra de Avaliação Dinâmica**: Visual moderno e personalizável 📊
* **Histórico de Análise**: Registra profundidade, avaliação e melhores lances 📜
* **Human Mode**: A engine joga como um humano — com pausas e erros ocasionais 🧑‍🦱
* **Fusion Mode**: Adapta automaticamente a força ao rating do oponente ⚖️
* **Auto Run & Auto Move**: Análise e jogadas automáticas opcionais 🤖
* **Atalhos de Teclado**: Controle completo com teclas de Q até = ⌨️
* **Interface Externa**: Painel avançado em outra janela ou aba 🪟
* **Exibição de Múltiplos Lances**: Veja os 3–5 melhores movimentos 🔢
* **Configurações Completas**: Interface totalmente customizável ⚙️

---

## 📥 Instalação

1. Instale um gerenciador de userscripts:

   * **Tampermonkey** (Chrome, Firefox, Edge, Safari) 🐒
   * **Violentmonkey** (Chrome, Firefox) 🙈
2. Instale o script pelo link (adicione quando houver) 🔗
3. Acesse Chess.com — a ferramenta ativa automaticamente 🎉

---

## 📖 Guia de Uso

### 🔹 Início Rápido

1. Abra um jogo no Chess.com
2. Pressione qualquer letra entre **Q e M** para rodar análises em profundidades diferentes
3. O melhor movimento será mostrado no tabuleiro
4. Veja a barra de avaliação à esquerda

---

## 🔧 Controles Detalhados

### Profundidade da Engine

de **Q até Z** = profundidades 1 a 20

* **Q** → depth 1 (rápido, raso) 💨
* **Z** → depth 20 (mais profundo) 🐢
* **=** → profundidade máxima ♾️

---

## ⚙️ Painel de Configurações

### **Engine**

* Profundidade
* Rating ELO
* Aberturas e repertórios

### **Ações**

* Iniciar/parar engine
* Salvar configurações

### **Visual**

* Barra de avaliação
* Setas e destaques
* Interface externa

### **Estilo de Jogo**

* Human Mode
* Fusion Mode

### **Auto**

* Auto-run
* Auto-move

---

## 📚 Livro de Aberturas & Repertórios

Categorias criadas dinamicamente:

* **Repertório Misto**
* **1.e4 (King's Pawn)**
* **1.d4 (Queen's Pawn)**
* **Inglês (1.c4)**
* **Flanco / Hipermodernas**

O sistema detecta automaticamente quando um lance é "in book" ou calculado pela engine.

---

## 🧑‍🦱 Human Mode

O motor joga como um humano:

* Variação de tempo
* Pequenos erros
* Raríssimos blunders
* Níveis de 800 a 2400 ELO

---

## ⚖️ Fusion Mode

Adapta a força do motor ao rating do seu oponente automaticamente.

---

## 🪟 Interface Externa

Permite controlar tudo por uma segunda janela.

### Requer:

* Arquivo Python `chess_ai_server.py`
* Rodar o servidor local
* Clicar em **Start Local Server** e depois **Open External Window**

### Benefícios:

* Tabuleiro virtual
* Visualização isolada
* Menos risco de detecção
* Interface limpa no Chess.com

---

## ⌨️ Atalhos de Teclado

| Tecla | Função      | Força        |
| ----- | ----------- | ------------ |
| Q–E   | Depth 1–3   | Beginner     |
| R–P   | Depth 4–10  | Intermediate |
| A–G   | Depth 11–15 | Advanced     |
| H–L   | Depth 16–19 | Expert       |
| Z–M   | Depth 20–26 | Master       |
| =     | Max depth   | Grandmaster  |

---

## 👍 Dicas

* Depth 5–10 = melhor velocidade x precisão
* Depth 15+ = posições críticas
* Use a janela externa para evitar poluição na tela
* Habilite múltiplos lances para ver opções avançadas
* Ajuste as cores e estilos das setas

---

## ⚠️ Disclaimer

Este projeto é para estudo, análise e uso casual.
O uso em partidas **ranqueadas** pode violar os termos do Chess.com.
Use por sua conta e risco.

---

## 🙌 Créditos

Criado por **allanaltarugio**
Motor: **Stockfish**, o engine open‑source mais forte do mundo

---

## 📜 Licença


Somente para uso pessoal. Não redistribuir.
