# QA_REPORT

Status: `passed-local`
Branch: `feat/fabio-capiao-piloto-v2`
Rota local: `http://127.0.0.1:4186/fabio-capiao-piloto-v2/`
Data: 27/08/2026

## Escopo

Nova landing page controlada para Fábio Péricles sobre usucapião. A página original `fabio-capiao.html`, CNAME, DNS e tracking externo permaneceram intactos.

## Assets

- logo oficial obtida no site público do escritório e salva em WebP;
- foto do Dr. Fábio já usada nas páginas existentes e salva em WebP;
- logo: 434×343, 23.784 bytes;
- foto: 701×864, 22.362 bytes.

## Validação estática

- HTML: passou, zero erros e warnings;
- JavaScript inline: passou;
- assets locais: passou;
- logo e copy: marcadores confirmados;
- `git diff --check`: passou;
- página original: sem alteração.

## Browser

- Chromium: 360×640, 390×844, 768×1024 e 1440×900;
- Firefox: 390×844 e 1440×900;
- WebKit: 390×844 e 1440×900;
- 8 combinações aprovadas;
- zero falha séria ou crítica no axe;
- zero erro de console ou overflow horizontal detectado.

## Lighthouse mobile

Mediana de 3 execuções:

| Métrica | Resultado | Gate |
|---|---:|---:|
| Performance | 100 | ≥95 |
| Acessibilidade | 100 | 100 |
| Boas práticas | 96 | ≥95 |
| SEO | 100 | ≥95 |
| LCP | 903 ms | ≤2500 ms |
| CLS | 0 | ≤0,1 |
| TBT | 7,5 ms | ≤200 ms |

## Revisão visual

A primeira versão apresentou logo pequena e card do hero com peso excessivo. Foram aplicadas três correções:

1. logo ampliada no desktop e mobile;
2. remoção da inclinação do documento;
3. remoção do selo decorativo.

A captura final confirmou logo oficial legível, CTA acima da dobra, conteúdo completo e ausência de quebra bloqueadora.

## Revisão especializada

- copy: hero tornou o problema e a atuação jurídica mais explícitos;
- design: logo vertical exige escala mínima, já aplicada; a proposta de azul e terracota não foi adotada porque a marca oficial do cliente usa preto e dourado;
- arquitetura: os cinco CTAs agora registram `cta_location` sem PII e preservam a navegação nativa.

Todos os gates foram repetidos após essas alterações.

## Resultado

Gate técnico local aprovado. Próximo gate: preview isolada e aprovação do Rafael antes de qualquer merge.
