
# Recurso de Sincronização de Relógio

## Visão Geral
O recurso Clock Synchronization (Sincronização de Relógio) foi adicionado com sucesso ao userscript do Chess AI. Ele faz com que o tempo de execução das jogadas do AI pareça mais humano, analisando o tempo restante de ambos os jogadores e ajustando os atrasos das jogadas de forma proporcional.

## Como Funciona

### Detecção do Relógio
- **Relógio do Oponente** e **Relógio do Jogador** são detectados por seletores do Chess.com
- Suporta vários formatos: MM:SS, H:MM:SS, M:SS
- Parsing robusto, compatível com diferentes layouts

## Lógica de Tempo

### Modo Standard Range
1. Oponente tem mais tempo → jogada rápida  
2. Você tem mais tempo → atraso artificial  
3. Tempos iguais → atraso moderado  

### Modo Exact Match
1. Oponente tem igual/mais tempo → atraso mínimo  
2. Você tem mais tempo → atraso exato  
3. Fórmula: `delay = (tempoJogador - tempoOponente) - tempoDeCálculo`  
4. Limite máximo de 30s  

### Time Pressure Override
1. Detecta emergências abaixo de um limite  
2. Usa atraso mínimo (0.1–0.5s)  
3. Funciona em todos os modos  
4. Retorna ao normal automaticamente  

## Cálculo de Atraso
- Standard: baseado na diferença de tempo  
- Exact Match: atraso calculado com precisão  

## Interface do Usuário
- Local: Aba **Automation > Auto Move**
- Controles:
  - Ativar Clock Sync  
  - Ativar Exact Match  
  - Ativar Time Pressure  
  - Threshold de emergência  
  - Min/Max Delay  
- Validação automática

## Implementação Técnica
- Novas funções:
  - `parseTimeString()`
  - `getClockTimes()`
  - `calculateClockSyncDelay()`
- Integração com:
  - Auto Move  
  - Configurações  
  - Main Loop  
  - Eventos  

## Instruções de Uso

### Pré-requisitos
- Auto Move ativo  
- Partida com relógios visíveis  

### Configuração
1. Ative Auto Move  
2. Ative Clock Sync  
3. Configure Time Pressure  
4. Escolha Standard ou Exact Match  

## Comportamento
- Standard: atraso proporcional  
- Exact Match: atraso exato  
- Time Pressure: atraso mínimo em emergências  

## Casos Especiais
- Suporte a Blitz, Rápido, Clássico  
- Falta de visibilidade do relógio  
- Fim de partida e flips do tabuleiro  

## Benefícios
- Simula comportamento humano  
- Reduz suspeita de automação  
- Totalmente personalizável  
- Integração completa  

## Exemplos de Console

### Standard
```
Clock sync: Opponent time: 180s, Player time: 240s
Clock sync: Player has 60s more time, adding 3.2s delay
Auto move: Applying clock sync delay of 3200ms
```

### Exact Match
```
Clock Sync: Using Exact Match mode
Clock Sync: Time difference: 60s
Clock Sync: Final delay: 59800ms
```

### Time Pressure
```
🚨 TIME PRESSURE MODE ACTIVATED
⚡ Using emergency delay: 0.23s
```

## Melhorias Futuras
- Suporte a outros sites  
- Padrões avançados  
- Aprendizado baseado no oponente  
- Timing baseado em ELO  
