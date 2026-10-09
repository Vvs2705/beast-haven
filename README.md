# Beast Haven

**Estilo:** idle/tycoon de santuário com coleção de criaturas (cozy), retrato.

**O que é:** um santuário de criaturas fantásticas resgatadas.

**Como funciona:** você monta habitats, alimenta, limpa e trata as criaturas; elas produzem recursos naturais (sem crueldade) que pagam melhorias, cuidadores e expedições. Espécies novas chegam por "receita de habitat" com pista — nada é sorteado nem comprado — e cada espécie afeta os lotes vizinhos, então o layout vira um quebra-cabeça.

**Como vai ser jogar:** cuidar, ver os bichos felizes e completar a coleção: um idle com apego.

## Situação
Fora desta rodada; a revisão de 2026-10-09 propôs criaturas 2D com um rig por arquétipo e coleção sem sorteio (ECA Digital). Ainda não há código: este repositório guarda o GDD e a estrutura do projeto, pronta para o desenvolvimento começar.

- **GDD:** [`docs/GDD.md`](docs/GDD.md) (revisão competitiva de 2026-10-09 no topo).
- **Comparativo com jogos similares e diferenciais:** [`docs/COMPETITIVO.md`](docs/COMPETITIVO.md).

## Estrutura do repositório
| Pasta | Para quê |
|---|---|
| `docs/` | GDD, comparativo e, depois, balance, validações e contratos de cada fase |
| `client/` | projeto Unity 6 (6000.3.x), Android primeiro, retrato; código do jogo em `client/Assets/_BH/` |
| `client/Assets/_BH/Scripts/Core/` | núcleo em C# puro (regras, simulação, save), testável fora do Unity |
| `client/Assets/_BH/Scripts/View/` | MonoBehaviours, UI, câmera, entrada |
| `client/Assets/_BH/Editor/` | setup do projeto e builds por linha de comando |
| `client/Assets/_BH/Tests/EditMode/` | testes NUnit do núcleo |
| `client/Assets/_BH/Resources/` | sprites e dados carregados em tempo de execução |
| `client/tools/` | ferramentas fora do Unity (testes `dotnet`, scripts de arte, relatório de playtest) |
| `arte/` | arte-fonte; `arte/tripo/` e `arte/mixamo/` ficam fora do git |

Como contribuir: [`CONTRIBUTING.md`](CONTRIBUTING.md). Histórico: [`CHANGELOG.md`](CHANGELOG.md).

## Repositório e licença
© V-STACK / Vinicius Souza. **Todos os direitos reservados.** Código, documentos e arte visíveis para acompanhamento, sem licença de uso, cópia ou redistribuição.
