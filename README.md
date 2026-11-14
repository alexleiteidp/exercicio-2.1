# Exercício 2.1 — Mapa de Atores da Jornada de um Serviço Público

**Aluno:** Alexander Andrade Leite
**Disciplina:** IDP-TD 2026 — Governo Digital e Transformação de Serviços Públicos no Brasil
**Serviço mapeado:** Atendimento ao Seguro-Desemprego pela URA da Caixa (0800 726 0207). Órgãos: Caixa Econômica Federal e Ministério do Trabalho e Emprego.

## Assistentes usados

| Papel | Assistente |
|---|---|
| Assistente 1 (pesquisa v1, v2, v3) | Claude (Anthropic, Claude Opus 5.5), com busca web |
| Assistente 2 (auditorias v1 e v2) | Grok (xAI) |
| Sessão `/grill-me` | Claude Code, com a skill `grill-me` de Matt Pocock |

## Índice

1. [A_meta_prompt.md](A_meta_prompt.md): meta-prompt (Parte A)
2. [B_relatorio_assistente_v1.md](B_relatorio_assistente_v1.md): pesquisa inicial do assistente 1
3. [B_relatorio_auditoria_v1.md](B_relatorio_auditoria_v1.md): auditoria da v1 pelo assistente 2
4. [B_relatorio_assistente_v2.md](B_relatorio_assistente_v2.md): v2, que trata cada falha da auditoria v1
5. [B_relatorio_auditoria_v2.md](B_relatorio_auditoria_v2.md): segunda auditoria
6. [B_relatorio_assistente_v3.md](B_relatorio_assistente_v3.md): versão final, com os deltas ligados aos gatilhos da auditoria v2
7. [C_grill_transcript.md](C_grill_transcript.md): transcript da sessão `/grill-me` (8 rodadas)
8. [C_mapa_atores.md](C_mapa_atores.md): mapa final, com diagrama mermaid e tabela RACI de 22 atores
