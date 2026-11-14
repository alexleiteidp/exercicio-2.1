# A — Meta-prompt

> **Assistente 1:** Claude (Anthropic, modelo Claude Opus 5.5), com busca na web.
> **Data de uso:** 13/11/2026.
> **Função deste arquivo:** é o pedido que fiz ao assistente 1 para que **ele escrevesse o prompt** de deep research. O prompt gerado está no Apêndice, ao final.

---

## Meta-prompt enviado ao assistente 1

Sou advogado e aluno da disciplina "Governo Digital e Transformação de Serviços Públicos no Brasil" (IDP, 2026). Preciso que você **elabore um prompt para um assistente de deep research** realizar uma pesquisa. Não faça a pesquisa agora: escreva o prompt.

**O problema.** Vou desenhar um **mapa de atores** da jornada do serviço **"Atendimento ao Seguro-Desemprego pela URA da Caixa"** — ou seja, o cidadão que liga para a central telefônica da Caixa Econômica Federal (Atendimento CAIXA ao Cidadão, 0800 726 0207), navega pelo menu de voz (URA/IVR), é roteado entre canais automatizados e atendentes, e obtém (ou não) uma resposta: situação do requerimento, data e valor das parcelas, motivo de bloqueio, encaminhamento para agência, para a Carteira de Trabalho Digital, para o gov.br ou para o posto do Sine/Superintendência Regional do Trabalho. Depois da pesquisa, farei uma sessão de entrevista adversarial (`/grill-me`) com um agente de IA para decidir quais atores entram no mapa e qual o papel (RACI) de cada um. A pesquisa precisa dar **contexto suficiente** para essa entrevista; um resumo genérico não serve.

**O que já sei (contexto).**
- O benefício é regido pela Lei nº 7.998/1990 (alterada pela Lei nº 13.134/2015) e por resoluções do CODEFAT; é custeado pelo FAT.
- O **Ministério do Trabalho e Emprego (MTE)** habilita o benefício (inclusive via Empregador Web, eSocial e Carteira de Trabalho Digital); a **Caixa** é o agente pagador.
- A URA é um canal de autoatendimento; há também atendentes humanos, e é provável que existam empresas terceirizadas de call center e fornecedores de tecnologia (plataforma de URA, reconhecimento de voz, Dataprev).
- Há atores "invisíveis": quem normatiza, quem audita (TCU, CGU), quem fiscaliza a qualidade do atendimento (ANATEL? Senacon? Ouvidorias?), quem protege dados (ANPD/LGPD).

**O que o prompt que você escrever deve exigir do pesquisador:**
1. **Escopo explícito:** Seguro-Desemprego (modalidade trabalhador formal e, se relevante, pescador artesanal e doméstico), canal URA/telefone da Caixa, órgãos MTE, Caixa, Dataprev, CODEFAT.
2. **Atores humanos E atores de IA/sistemas automatizados, explicitamente:** cidadão, terceiros que ligam em nome dele, operadores, supervisores, gestores do contrato, auditores, normatizadores, fornecedores; e, do lado automatizado, URA/IVR, reconhecimento de voz/fala, roteador (ACD/CTI), assistentes virtuais/chatbots (ex.: WhatsApp da Caixa), motores de regras de habilitação, bases de dados (CNIS, CAGED/eSocial).
3. **Horizonte temporal datado:** de 2015 (Lei 13.134) até novembro de 2026, destacando mudanças a partir de 2020 (pandemia, digitalização da habilitação, Carteira de Trabalho Digital).
4. **Formato de saída estruturado:** (a) sumário; (b) linha do tempo da jornada; (c) **tabela de atores** com colunas: ator, tipo (humano / IA-sistema / institucional), papel, momento em que entra e sai da jornada, base legal ou fonte; (d) lacunas e incertezas; (e) lista de fontes.
5. **Critérios de fonte verificáveis:** toda afirmação factual com URL; priorizar fontes primárias (planalto.gov.br, gov.br/trabalho-e-emprego, caixa.gov.br, portal do TCU, Diário Oficial, contratos no Portal da Transparência/Compras.gov.br); marcar explicitamente o que for **inferência** e o que for **não confirmado**; não inventar números de contrato, nomes de fornecedores ou estatísticas.
6. **Postura crítica:** apontar onde a jornada falha (filas, desistência, falta de transbordo para humano) e quem responde por cada falha.

Escreva o prompt em português, pronto para colar, com persona, objetivo, escopo, perguntas de pesquisa, formato de saída e regras de evidência.

---

## Apêndice — Prompt de deep research gerado pelo assistente 1

> Colado aqui apenas para rastreabilidade; o entregável da Parte A é o meta-prompt acima.

```
PERSONA: Você é um pesquisador sênior em governo digital e desenho de serviços públicos,
com experiência em centrais de atendimento (URA/IVR, contact center) e em direito
administrativo brasileiro.

OBJETIVO: Produzir um relatório que identifique TODOS os atores — humanos, institucionais
e de IA/sistemas automatizados — que participam da jornada "Atendimento ao
Seguro-Desemprego pela URA da Caixa" (Caixa Econômica Federal, telefone 0800 726 0207 e
números correlatos), servindo de insumo para um mapa de atores com papéis RACI.

ESCOPO:
- Serviço: Seguro-Desemprego (trabalhador formal; mencione doméstico e pescador
  artesanal só quando mudarem a jornada telefônica).
- Canal principal: URA/telefone da Caixa; canais para onde o cidadão é encaminhado
  (agência, app CAIXA Trabalhador, WhatsApp, Carteira de Trabalho Digital, gov.br,
  Sine/SRTE, central 158 do MTE).
- Órgãos: MTE, Caixa, Dataprev, CODEFAT/FAT, órgãos de controle e de defesa do usuário.
- Período: 2015 (Lei 13.134/2015) a novembro de 2026; destaque mudanças pós-2020.

PERGUNTAS DE PESQUISA:
1. Qual é o fluxo da jornada telefônica, passo a passo (entrada na URA, menus,
   autenticação, consulta, transbordo, encerramento)?
2. Quem habilita, quem paga, quem processa dados, quem opera o atendimento?
3. Que sistemas automatizados/IA atuam (URA, reconhecimento de fala, roteamento,
   chatbots, regras de habilitação, cruzamento de bases como CNIS/eSocial)?
4. Quem normatiza, contrata, fiscaliza, audita e recebe reclamações?
5. Onde a jornada falha e quem responde por cada falha?

FORMATO DE SAÍDA:
1. Sumário executivo (≤ 10 linhas)
2. Linha do tempo da jornada
3. Tabela de atores: | Ator | Tipo (humano / IA-sistema / institucional) | Papel |
   Entra na jornada | Sai da jornada | Fonte (URL) |
4. Pontos de falha e responsáveis
5. Lacunas, incertezas e inferências (rotuladas)
6. Lista de fontes com URL

REGRAS DE EVIDÊNCIA:
- Toda afirmação factual com URL; prefira fontes primárias (planalto.gov.br,
  gov.br, caixa.gov.br, portal.tcu.gov.br, in.gov.br, Portal da Transparência).
- Marque [INFERÊNCIA] quando deduzir sem fonte direta e [NÃO CONFIRMADO] quando a
  informação existir só em fonte secundária.
- Não invente números de contrato, nomes de empresas, estatísticas ou acórdãos.
- Se não encontrar algo, diga que não encontrou.
```
