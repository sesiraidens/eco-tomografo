# Protocolo USB · USB protocol

Uma linha por mensagem, terminada em quebra de linha; números com ponto decimal.

| Programa envia | Pico responde | Uso |
|---|---|---|
| `I` | `I RAIDENS 2 12 DEMO` | identifica firmware, canais e modo (DEMO/REAL) |
| `B 3` | `R 3 0.0 287.1 … -1 F 3` | captura do prego 3: chegadas em µs a partir do primeiro sensor; `F` = sensor que disparou primeiro; `-1` = sem sinal |
| `G 12 x1 y1 … x12 y12` | `G OK 12` | posição dos pregos em cm (leste, norte; medula na origem) |
| `W 20` | `W OK 20` | só DEMO: chance (%) de a batida sair no prego vizinho |
| — | `R 3 TIMEOUT` | ninguém bateu em 15 s |
| `X` | `X OK` | cancela a captura |
| `M DEMO` / `M REAL` | `M OK DEMO` | troca o modo |
| `PING` | `READY,RAIDENS_PICO` | teste |
