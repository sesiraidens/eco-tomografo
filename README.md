<img width="100%" alt="dsgdsg" src="https://github.com/user-attachments/assets/c032532a-41e5-4230-8931-18e94b3f8a2a" />

# E.C.O. · Estudo de Cavidades Ocultas

**PT** · Tomógrafo sônico de baixo custo e código aberto para investigar o interior de árvores urbanas. Um pêndulo bate de leve no tronco, sensores piezoelétricos escutam a vibração do outro lado e o programa **Raidens Campo** transforma os atrasos do som num mapa de possíveis cavidades, sem cortar a árvore.

**EN** · A low-cost, open-source sonic tomograph to look inside urban trees. A pendulum gently taps the trunk, piezoelectric sensors listen on the other side and the **Raidens Campo** app turns the sound delays into a map of possible cavities, without cutting the tree.

Projeto de Inovação da equipe **RAIDENS** · FIRST® LEGO® League BIOGLOW 2026/2027 · Sorocaba/Alumínio (SP), Brasil.

## Como funciona · How it works
1. **Medir o tronco** · measure the trunk (circunferência, diâmetros, forma).
2. **Instalar os sensores** · install 8 to 16 sensors on thin nails, evenly spaced from north.
3. **Bater com o pêndulo** · tap each nail; the Raspberry Pi Pico timestamps the arrivals in microseconds.
4. **Ler o mapa** · the app compares every path with a healthy tree and maps where sound slowed down.

> ⚠️ Triagem experimental feita por estudantes com um protótipo em validação. Não é laudo técnico e não substitui a avaliação de profissional habilitado. · Experimental student screening, not a technical report.

## Estrutura · Structure
| Pasta / Folder | Conteúdo / Contents |
|---|---|
| `software/` | Raidens Campo (HTML único, Web Serial) · field app |
| `firmware/` | Firmware MicroPython da Pico (`tomografo_pico.py`) |
| `hardware/3d/` | Modelos 3D (STL/STEP) · 3D models |
| `hardware/eletronica/` | Esquema elétrico · schematics |
| `hardware/BOM.md` | Lista de materiais · bill of materials |
| `docs/montagem/` | Guia de montagem · assembly guide |
| `docs/protocolo/` | Protocolo de medição e USB · measurement & USB protocol |
| `dados/` | Medições de exemplo (CSV) · sample data |

## Contribua · Contribute
Abra uma *issue*, faça um *fork* e envie um *pull request*, ou compartilhe o CSV das suas medições. · Open an issue, fork and send a pull request, or share your measurement CSV.

Contato · Contact: sesiraidens@gmail.com · Instagram/YouTube/TikTok: @sesiraidens

## Licenças · Licenses
- Software (Raidens Campo, firmware): [MIT](LICENSE)
- Hardware (modelos 3D, eletrônica): [CERN-OHL-P-2.0](LICENSES/CERN-OHL-P-2.0.txt)
- Documentação, textos e imagens · docs, text and images: [CC BY 4.0](LICENSES/CC-BY-4.0.txt)

FIRST® e FIRST® LEGO® League são marcas registradas da FIRST. LEGO® é marca registrada do LEGO Group. Projeto da equipe, sem endosso delas.
