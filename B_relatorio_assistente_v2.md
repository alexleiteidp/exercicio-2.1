# B — Relatório do assistente 1 (v2)

> Assistente 1: Claude (Anthropic, Claude Opus 5.5) com busca web · v2 em 14/11/2026, revisada a partir de B_relatorio_auditoria_v1.md (ChatGPT)
>
> **Nota de rastreabilidade (14/11/2026):** a linha acima diz "(ChatGPT)", mas o assistente 2 foi o **Grok (xAI)**. O erro de atribuição foi apontado na audit_v2 (N15) e corrigido na v3. O texto da v2 foi mantido como produzido.

## v2

### 0. Tratamento das falhas da auditoria v1

Legenda: (a) corrigido; (b) defendido com evidência; (c) pendente. Cada falha foi verificada na fonte. Em casos mistos, a primeira letra é a principal.

| Falha | Tratamento (a/b/c) | O que mudou / argumento / o que fica pendente | Fonte |
|---|---|---|---|
| F1 – Pescador no INSS | (a) | **Procede.** A MP 1.323/2025 passou o defeso ao MTE a partir de 1º/11/2025; o INSS fica com os defesos até 31/10/2025. A MP virou a Lei 15.399/2026, cujo texto transfere a competência só de forma indireta; a notícia do MTE é expressa. Entram MPA, Fundacentro, entidades de pesca e Telebrás. | [MTE nov./2025](https://www.gov.br/trabalho-e-emprego/pt-br/noticias-e-conteudo/2025/novembro/seguro-defeso-passa-a-ser-administrado-pelo-ministerio-do-trabalho-e-emprego); [Lei 15.399](https://www.planalto.gov.br/ccivil_03/_ato2023-2026/2026/lei/l15399.htm) |
| F2 – Res. 467/2005 revogada | (a), com ressalva (b) | **Procede.** A Res. CODEFAT 957/2022 revogou a 467/2005 (art. 68, XLVII) e vigora desde 3/10/2022 (art. 69). Ela agora é a âncora geral do benefício. Defendo, porém, que a v1 não errou ao **relatar**: a página gov.br de **recurso** ainda cita a Res. 467/2005. Isso passou a ser registrado como ponto de falha (F10 da seção 4). | [Res. 957 – LegisWeb](https://www.legisweb.com.br/legislacao/?id=436595); [gov.br Recurso](https://www.gov.br/pt-br/servicos/cadastrar-recurso-relativo-ao-seguro-desemprego); [gov.br Solicitar](https://www.gov.br/pt-br/servicos/solicitar-o-seguro-desemprego) |
| F3 – Prazo de 120 dias | (a) | **Procede.** O art. 6º da Lei 7.998 diz só "a partir do sétimo dia". O intervalo do 7º ao 120º dia vem do art. 41 da Res. 957. | [Lei 7.998](https://www.planalto.gov.br/ccivil_03/leis/l7998.htm); [Res. 957](https://www.legisweb.com.br/legislacao/?id=436595) |
| F4 – "4 mil recursos/ano" | (a) | **Procede.** A fonte fala em cerca de 4 mil recursos por ano "referentes a situações em que já teria havido dois recursos indeferidos de um mesmo requerimento". O texto foi corrigido. | [TCU 135/2024](https://portal.tcu.gov.br/imprensa/noticias/inconsistencias-no-seguro-desemprego-causaram-prejuizo-a-administracao-publica) |
| F5 – "6 meses" | (a) | **Procede.** A lei exige salário em cada um dos 6 meses imediatamente anteriores à dispensa. | [Lei 13.134](https://www.planalto.gov.br/ccivil_03/_ato2015-2018/2015/lei/l13134.htm) |
| F6 – "eSocial gerido pelo Serpro" | (a), com ressalva (b) | **Defesa parcial:** a v1 seguiu o TCU, que diz "sistema gerido pelo Serpro". **Correção:** pela Portaria ME 300/2019 (art. 2º), o eSocial tem Comitê Gestor (Trabalho, RFB, INSS e outros), com Serpro e Dataprev em apoio (art. 8º). O Decreto 8.373, citado pelo auditor, teve os arts. 4º a 7º revogados pelo Decreto 10.087/2019. RFB e Comitê entram na tabela; a composição atual fica (c). | [TCU 1114/2025](https://portal.tcu.gov.br/imprensa/noticias/fragilidades-na-transparencia-do-esocial-aumentam-risco-de-pagamentos-indevidos); [Portaria 300/2019](https://www.gov.br/esocial/pt-br/centrais-de-conteudo/legislacao/empresas/portaria-300_textoconsolidado.pdf); [Decreto 8.373](https://www.planalto.gov.br/ccivil_03/_ato2011-2014/2014/decreto/d8373.htm) |
| F7 – Lei 14.075/2020 | (a) | **Procede.** A lei (conversão da MP 982/2020) trata da poupança social digital para "benefícios sociais" (art. 3º, V), exceto os previdenciários. Não cita o seguro-desemprego nem o CAIXA Tem e remete ao CMN e ao Banco Central. A inclusão do seguro-desemprego vem da FAQ da Caixa e da Res. 957. | [Lei 14.075](https://www.planalto.gov.br/ccivil_03/_ato2019-2022/2020/lei/L14075.htm); [FAQ Caixa](https://www.caixa.gov.br/beneficios-trabalhador/seguro-desemprego/perguntas-frequentes/Paginas/default.aspx) |
| F8 – Caixa e art. 15 | (a) | **Procede.** O art. 15 vigente fala em "Bancos Oficiais Federais". A Caixa é designada pelo art. 64, § 1º, da Res. 957: "A Caixa Econômica Federal é o agente pagador...". Também consta da página da Caixa. | [Lei 7.998](https://www.planalto.gov.br/ccivil_03/leis/l7998.htm); [Res. 957](https://www.legisweb.com.br/legislacao/?id=436595); [Caixa SD](https://www.caixa.gov.br/beneficios-trabalhador/seguro-desemprego/Paginas/default.aspx) |
| F9 – Portaria MTE 1.889/2025 | (a) | **Procede.** Extraí o texto do PDF. A portaria autoriza a Dataprev a compartilhar com a Telebrás os dados (município, UF, CPF, nome e nascimento) de pescadores beneficiários de 2024 em municípios listados. Não trata do formal. Ela deixa de ser âncora de LGPD. Os papéis de controlador e operador seguem como [INFERÊNCIA]. | [Portaria 1.889](https://www.gov.br/trabalho-e-emprego/pt-br/acesso-a-informacao/tratamento-de-dados-pessoais/PORTARIAMTEN1.889DE7DENOVEMBRODE2025.pdf) |
| F10 – Canais | (b) parcial + (a) | **Defesa:** a página gov.br aponta o "Portal de Serviços" para *portalcidadao.dataprev.gov.br*; a hospedagem é da Dataprev, o serviço é do MTE. **Correção:** o presencial é subsidiário (Res. 957, art. 5º, § 2º, em SRTE ou SINE) e agendado pela FACILITA. Sine como rede estadual/municipal: [NÃO CONFIRMADO]. | [gov.br Solicitar](https://www.gov.br/pt-br/servicos/solicitar-o-seguro-desemprego); [Res. 957](https://www.legisweb.com.br/legislacao/?id=436595) |
| F11 – Fala.BR | (b) | **Contesto.** A página gov.br Solicitar não escreve "Fala.BR", mas os itens Denúncia, Reclamação, Elogio e Sugestão apontam para *falabr.cgu.gov.br*. A atribuição tem base. Por transparência, acrescentei também a fonte da Agência Gov, que nomeia o Fala.BR. | [gov.br Solicitar](https://www.gov.br/pt-br/servicos/solicitar-o-seguro-desemprego); [Agência Gov jul./2026](https://agenciagov.ebc.com.br/noticias/202607/saiba-como-acessar-os-canais-de-atendimento-do-ministerio-do-trabalho-e-emprego) |
| F12 – "integração em 180 dias" | (a) | **Procede.** O texto do TCU é "tome medidas para integrar". O prazo é para agir, não para concluir. | [TCU 1621/2026](https://portal.tcu.gov.br/imprensa/noticias/tribunal-avalia-servico-digital-de-seguro-desemprego-para-trabalhadores-formais) |
| F13 – "Dataprev não forneceu" | (a) | **Procede.** A fonte fala em "problemas operacionais que impediram o acesso adequado". O TCU mandou o MTE, com a Dataprev, dar acesso ao DataLake em 10 dias. | [TCU 1114/2025](https://portal.tcu.gov.br/imprensa/noticias/fragilidades-na-transparencia-do-esocial-aumentam-risco-de-pagamentos-indevidos) |
| F14 – "pagamentos indevidos" | (a) | **Procede.** Passei a usar "possíveis pagamentos indevidos" e "indícios" de R$ 147 mi e de cerca de R$ 544 mil. Incluí a falta de análise dos pagamentos por ordem judicial. | [TCU 135/2024](https://portal.tcu.gov.br/imprensa/noticias/inconsistencias-no-seguro-desemprego-causaram-prejuizo-a-administracao-publica) |
| F15 – Doméstico | (a) | **Procede.** Pela LC 150/2015, o doméstico recebe 1 salário mínimo por no máximo 3 meses (art. 26) e requer do 7º ao 90º dia (art. 29). A Res. 957, art. 46, repete o prazo. | [LC 150](https://www.planalto.gov.br/ccivil_03/leis/lcp/lcp150.htm); [Res. 957](https://www.legisweb.com.br/legislacao/?id=436595) |
| F16 – Resgatado / bolsa qualificação | (a), com (b) quanto ao número | **Inclusão aceita:** as duas variantes e a Inspeção do Trabalho (Res. 957, arts. 49 a 63) entram no relatório. **Contesto o número de parcelas:** o auditor diz 3, mas o art. 2º-C da Lei 7.998, na redação da Lei 15.455/2026, prevê **6 parcelas** de 1 salário mínimo. A redação antiga, da Lei 10.608/2002, previa 3. | [Lei 7.998](https://www.planalto.gov.br/ccivil_03/leis/l7998.htm); [Res. 957](https://www.legisweb.com.br/legislacao/?id=436595) |
| F17 – Via judicial | (a) | **Procede.** O TCU 135/2024 cita pagamentos por ordem judicial. A Res. 957 aceita "documento judicial" na habilitação (art. 4º, § 1º) e reemissão por ordem judicial (art. 21, § 2º). A Justiça Federal entra na tabela como [INFERÊNCIA] de competência, por ser a União a ré. AGU e DPU também entram como [INFERÊNCIA], sem fonte lida. | [TCU 135/2024](https://portal.tcu.gov.br/imprensa/noticias/inconsistencias-no-seguro-desemprego-causaram-prejuizo-a-administracao-publica); [Res. 957](https://www.legisweb.com.br/legislacao/?id=436595) |
| F18 – CNIS presumido | (a) | **Procede, e agora com fonte.** A Res. 957, art. 4º, § 1º, lista CNIS, guia do FGTS, GFIP, eSocial e documento judicial como bases da habilitação automática. O CNIS e as bases de benefícios do INSS entram na tabela. O papel do INSS como mantenedor do CNIS fica como [INFERÊNCIA]. | [Res. 957](https://www.legisweb.com.br/legislacao/?id=436595) |
| F19 – Identidade gov.br | (a), parcial (c) | **Procede.** A conta gov.br (Prata/Ouro, exigida no recurso) entra como ator. O órgão gestor (SGD/MGI) fica [NÃO CONFIRMADO]: não li fonte. A transição de autenticação dos pescadores está confirmada (Lei 15.399, art. 7º). | [gov.br Recurso](https://www.gov.br/pt-br/servicos/cadastrar-recurso-relativo-ao-seguro-desemprego); [Lei 15.399](https://www.planalto.gov.br/ccivil_03/_ato2023-2026/2026/lei/l15399.htm) |
| F20 – Reguladores | (a) parcial + (c) | **Incluídos:** o CMN e o Banco Central, que regulam a poupança social digital (Lei 14.075, art. 2º, VII a IX), e as entidades de pesca (Lei 15.399). **Pendentes (c):** as regras do BC sobre SAC e ouvidoria de bancos, a Senacon como gestora do consumidor.gov.br e o papel da ANPD. Não li fontes sobre esses três, que constam só como [INFERÊNCIA]. | [Lei 14.075](https://www.planalto.gov.br/ccivil_03/_ato2019-2022/2020/lei/L14075.htm); [Lei 15.399](https://www.planalto.gov.br/ccivil_03/_ato2023-2026/2026/lei/l15399.htm) |
| F21 – "IA-sistema" | (a) | **Procede.** O tipo passou a ser "sistema automatizado". A presença de IA (reconhecimento de fala, NLU) é marcada [NÃO CONFIRMADO] item a item. | — |
| F22 – "opção 9 → 1" | (a) + (c) | **Procede.** Retirei a "opção 9 → 1", que vinha de fonte não lida. Restringi a consulta da conta de crédito à conta Caixa. Não localizei o comunicado primário da Caixa: (c). | [Jornal Contábil 2018](https://jornalcontabil.com.br/noticia/seguro-desemprego-fgts-e-pis-tem-novas-datas-de-pagamento/) |
| F23 – Horários | (b) | **Contesto.** A página oficial de atendimento da Caixa põe o horário humano (seg.–sex. 8h–21h; sáb. 10h–16h) no bloco "Atendimento CAIXA Cidadão ☎ 0800 726 0207"; o bloco da Central 111 vem depois. A página do WhatsApp diz "Assistente virtual disponível 24 horas por dia". O Portal Cidadão citado pelo auditor carrega via JavaScript e não pôde ser lido. | [Caixa Atendimento](https://www.caixa.gov.br/atendimento/Paginas/default.aspx); [WhatsApp Caixa](https://www.caixa.gov.br/atendimento/canais-digitais/whatsapp/Paginas/default.aspx) |
| F24 – Risco dos 67 dias | (a), parcial (c) | **Procede.** Pela Res. 957, art. 21, § 2º, a parcela devolvida pode ser reemitida a pedido do beneficiário ou por ordem judicial, em até 2 anos. Reduzi a gravidade do ponto de falha. O canal e o responsável pela reemissão (app/158/MTE) ficam [NÃO CONFIRMADO]. | [Res. 957](https://www.legisweb.com.br/legislacao/?id=436595) |
| F25 – Datas Facilita/Celeste/SRTE | (a) + (b) | **Procede** quanto à Facilita: 18/12/2025 foi o lançamento oficial, e os "238 mil atendimentos on-line em apenas dois meses" indicam operação anterior [INFERÊNCIA]. **Procede** quanto à Celeste, que já é citada em dez./2025. **Contesto** quanto à SRTE: a matéria de julho de 2026 lista as SRTE em "Canais de acesso", com link. | [Agência Gov dez./2025](https://agenciagov.ebc.com.br/noticias/202512/facilita-brasil-governo-federal-lanca-novo-canal-digital-para-simplificar-servicos-a-trabalhadores-e-empresas); [Agência Gov jul./2026](https://agenciagov.ebc.com.br/noticias/202607/saiba-como-acessar-os-canais-de-atendimento-do-ministerio-do-trabalho-e-emprego) |
| F26 – Arts. 15 e 23 | (a) | **Procede.** O art. 15 vigente é o original. A redação da MP 905/2019 está marcada como "Vigência encerrada" e "Revogada pela MP 955/2020". O art. 23 tem redação da Lei 14.261/2021: a nota da página diz "10.261", mas o link aponta para L14261. | [Lei 7.998](https://www.planalto.gov.br/ccivil_03/leis/l7998.htm) |
| F27 – Lei 13.460 | (a) | **Procede.** A lei disciplina as atribuições das ouvidorias (art. 13: "terão como atribuições precípuas") e não as cria. Ela se aplica à "administração pública direta e indireta" (art. 1º, § 1º). A Caixa, empresa pública, integra a administração indireta [INFERÊNCIA jurídica corrente, sem fonte lida aqui]. | [Lei 13.460](https://www.planalto.gov.br/ccivil_03/_ato2015-2018/2017/lei/l13460.htm) |
| NV1 – Páginas da Caixa não verificadas | (b) | Li as quatro páginas da Caixa por download direto. O redirecionamento só ocorre sem cookies. Os trechos citados acima e na v1 foram conferidos. | [FAQ Caixa](https://www.caixa.gov.br/beneficios-trabalhador/seguro-desemprego/perguntas-frequentes/Paginas/default.aspx); [Caixa Atendimento](https://www.caixa.gov.br/atendimento/Paginas/default.aspx) |
| NV2 – Artigos da Res. 957 | (a) | Verificados: art. 41 (120 dias), art. 46 (doméstico, 90 dias), art. 21 (67 dias e reemissão), art. 20 (crédito em conta), art. 12 (30 dias), arts. 27 e 28 (recurso de 120 dias em instância única), art. 64, § 1º (Caixa). Ressalva: a página da LegisWeb mostra alterações posteriores, entre elas a Res. 1.027/2025. | [Res. 957](https://www.legisweb.com.br/legislacao/?id=436595) |
| NV3 – Íntegra dos acórdãos | (c) | Continuo usando só as notícias e o sumário do TCU. Pendente. | [TCU sumário](https://portal.tcu.gov.br/publicacoes-institucionais/sumarios-executivos/auditoria-seguro-desemprego-emprega-brasil) |
| NV4 – Fim da matéria Agência Gov jul./2026 | (a) | Verificado: o corpo termina nos canais (158, Facilita, Celeste, SRTE, Fala.BR, SEI e denúncias). O que vem depois é navegação do site. | [Agência Gov jul./2026](https://agenciagov.ebc.com.br/noticias/202607/saiba-como-acessar-os-canais-de-atendimento-do-ministerio-do-trabalho-e-emprego) |
| NV5 – Composição atual do Comitê Gestor do eSocial | (c) | Só confirmei a composição da Portaria ME 300/2019, da era do Ministério da Economia. A composição atual fica pendente. | [Portaria 300/2019](https://www.gov.br/esocial/pt-br/centrais-de-conteudo/legislacao/empresas/portaria-300_textoconsolidado.pdf) |

### 1. Sumário executivo

- A jornada é **bifurcada**. O MTE habilita e concede o benefício, com sistemas operados pela Dataprev. A Caixa **paga** como agente pagador (Res. CODEFAT 957/2022, art. 64, § 1º), com recursos do FAT ([Caixa SD](https://www.caixa.gov.br/beneficios-trabalhador/seguro-desemprego/Paginas/default.aspx)).
- O 0800 726 0207 ("Atendimento CAIXA Cidadão") atende PIS, Benefícios Sociais, FGTS e Cartão Social. A URA eletrônica funciona 24h. O atendimento humano vai de segunda a sexta, das 8h às 21h, e aos sábados, das 10h às 16h ([Caixa Atendimento](https://www.caixa.gov.br/atendimento/Paginas/default.aspx)).
- Dúvidas de **concessão e valor** são remetidas pela própria Caixa ao MTE: app CTPS Digital, gov.br e 158 ([FAQ Caixa](https://www.caixa.gov.br/beneficios-trabalhador/seguro-desemprego/perguntas-frequentes/Paginas/default.aspx)).
- A habilitação é **automática**, por cruzamento com CNIS, FGTS, GFIP e eSocial. O recurso vai ao MTE em 120 dias, em instância única (Res. 957, arts. 4º, 27 e 28).
- Desde 1º/11/2025, o **seguro-defeso** do pescador também é gerido pelo MTE (MP 1.323/2025, convertida na Lei 15.399/2026).
- O TCU aponta falhas (Acórdãos 135/2024, 1114/2025 e 1621/2026). Menus da URA, tecnologia de voz e fornecedores seguem sem fonte primária.

### 2. Linha do tempo da jornada

**2.1 Marcos (2015–2026)**

| Data | Marco | Fonte |
|---|---|---|
| 2015 | A Lei 13.134/2015 escalona a carência. O 1º pedido exige 12 meses nos últimos 18. O 2º exige 9 nos últimos 12. A partir do 3º, exige salário em cada um dos 6 meses imediatamente anteriores à dispensa. O benefício passa a ter de 3 a 5 parcelas. O INSS passa a processar o defeso. | [Lei 13.134](https://www.planalto.gov.br/ccivil_03/_ato2015-2018/2015/lei/l13134.htm) |
| 2015 | A LC 150/2015 fixa o seguro do doméstico: 1 salário mínimo, por no máximo 3 meses, requerido do 7º ao 90º dia. | [LC 150](https://www.planalto.gov.br/ccivil_03/leis/lcp/lcp150.htm) |
| 2020 | A Lei 14.075/2020 cria a poupança social digital para benefícios sociais, com regulação do CMN e do Banco Central. A Caixa a usa para o seguro-desemprego (CAIXA Tem). | [Lei 14.075](https://www.planalto.gov.br/ccivil_03/_ato2019-2022/2020/lei/L14075.htm); [FAQ Caixa](https://www.caixa.gov.br/beneficios-trabalhador/seguro-desemprego/perguntas-frequentes/Paginas/default.aspx) |
| 03/10/2022 | Entra em vigor a Res. CODEFAT 957/2022, que revoga a Res. 467/2005 e se torna a norma geral do benefício. | [Res. 957](https://www.legisweb.com.br/legislacao/?id=436595) |
| 31/01/2024 | O Acórdão 135/2024 aponta possíveis pagamentos indevidos e falhas de governança na relação entre o MTE e a Dataprev. | [TCU 135/2024](https://portal.tcu.gov.br/imprensa/noticias/inconsistencias-no-seguro-desemprego-causaram-prejuizo-a-administracao-publica) |
| 21/05/2025 | O Acórdão 1114/2025 trata da integridade dos dados do eSocial e do acesso ao DataLake em 10 dias. | [TCU 1114/2025](https://portal.tcu.gov.br/imprensa/noticias/fragilidades-na-transparencia-do-esocial-aumentam-risco-de-pagamentos-indevidos) |
| 01/11/2025 | O seguro-defeso passa ao MTE (MP 1.323, de 4/11/2025). | [MTE](https://www.gov.br/trabalho-e-emprego/pt-br/noticias-e-conteudo/2025/novembro/seguro-defeso-passa-a-ser-administrado-pelo-ministerio-do-trabalho-e-emprego) |
| 18/12/2025 | Lançamento oficial da Facilita Brasil, desenvolvida pela Dataprev. Ela já somava 238 mil atendimentos em 2 meses. A Celeste é citada na mesma matéria. | [Agência Gov dez./2025](https://agenciagov.ebc.com.br/noticias/202512/facilita-brasil-governo-federal-lanca-novo-canal-digital-para-simplificar-servicos-a-trabalhadores-e-empresas) |
| 04/05/2026 | A Lei 15.399/2026 converte a MP 1.323. O art. 7º cria uma transição de autenticação para os defesos de 1º/11/2025 a 31/10/2026. | [Lei 15.399](https://www.planalto.gov.br/ccivil_03/_ato2023-2026/2026/lei/l15399.htm) |
| 2026 | A Lei 15.455/2026 eleva para 6 as parcelas do trabalhador resgatado (art. 2º-C da Lei 7.998). | [Lei 7.998](https://www.planalto.gov.br/ccivil_03/leis/l7998.htm) |
| 24/06/2026 | O Acórdão 1621/2026 trata de sistemas paralelos, atendimento e recursos. O MTE deve "tomar medidas para integrar" o benefício ao eSocial em 180 dias. | [TCU 1621/2026](https://portal.tcu.gov.br/imprensa/noticias/tribunal-avalia-servico-digital-de-seguro-desemprego-para-trabalhadores-formais) |

**2.2 Jornada do cidadão (trabalhador formal)**

1. **Dispensa.** O empregador entrega o requerimento e transmite os dados pelo Empregador Web, com certificado ICP-Brasil (Res. 957, art. 40, § 1º), ou pelo eSocial ([TCU 1621/2026](https://portal.tcu.gov.br/imprensa/noticias/tribunal-avalia-servico-digital-de-seguro-desemprego-para-trabalhadores-formais)).
2. **Requerimento, do 7º ao 120º dia** (Lei 7.998, art. 6º; Res. 957, art. 41). Os canais são o "Portal de Serviços" (link na Dataprev) ou o gov.br e o app CTPS Digital. O presencial é subsidiário: SRTE ou SINE, quando o acesso digital é impossível (Res. 957, art. 5º), com agendamento pela Facilita ([gov.br Solicitar](https://www.gov.br/pt-br/servicos/solicitar-o-seguro-desemprego)). A URA da Caixa não recebe requerimentos [INFERÊNCIA: não está na lista oficial de canais].
3. **Habilitação automática.** O sistema cruza CNIS, guia do FGTS, GFIP, eSocial ou documento judicial (Res. 957, art. 4º, § 1º). Inconsistência gera notificação digital a quem tem gov.br (art. 8º). O recurso cabe em 120 dias e é decidido em instância única pela Secretaria do Trabalho do MTE (arts. 27 e 28). Recurso exige conta gov.br Prata ou Ouro ([gov.br Recurso](https://www.gov.br/pt-br/servicos/cadastrar-recurso-relativo-ao-seguro-desemprego)).
4. **Liberação e pagamento.** A 1ª parcela sai 30 dias após o requerimento, e as demais a cada 30 dias (Res. 957, art. 12). A ordem é: conta indicada; poupança Caixa; poupança social digital (CAIXA Tem); terminais, lotéricas e correspondentes, com Cartão Social e senha ou biometria; agência, com documento ([gov.br Solicitar](https://www.gov.br/pt-br/servicos/solicitar-o-seguro-desemprego); [FAQ Caixa](https://www.caixa.gov.br/beneficios-trabalhador/seguro-desemprego/perguntas-frequentes/Paginas/default.aspx)). A parcela fica disponível por 67 dias e depois volta ao FAT. Pode ser reemitida em até 2 anos (Res. 957, art. 21).
5. **Chamada à URA 0800 726 0207.**
   - (a) **Entrada:** URA eletrônica 24h ([Caixa Atendimento](https://www.caixa.gov.br/atendimento/Paginas/default.aspx)).
   - (b) **Menu:** "opção 5" para o seguro-desemprego, segundo matéria de 2018 que reproduz comunicado da Caixa ([Jornal Contábil 2018](https://jornalcontabil.com.br/noticia/seguro-desemprego-fgts-e-pis-tem-novas-datas-de-pagamento/)) [NÃO CONFIRMADO para 2026].
   - (c) **Autenticação:** NIS e "identificação positiva" com dados cadastrais (mesma fonte) [NÃO CONFIRMADO para 2026]. Se a URA usa só teclas (DTMF) ou também reconhecimento de voz, não foi apurado: [NÃO CONFIRMADO].
   - (d) **Consulta:** liberação, agendamento ou pagamento da parcela e data da próxima. A confirmação da conta de crédito só vale para conta Caixa (mesma fonte).
   - (e) **Transbordo:** para atendente humano no horário oficial, ou para os canais do MTE, quando a dúvida é de concessão ou valor (FAQ Caixa). A forma de transferência ao atendente não foi confirmada.
   - (f) **Encerramento:** resposta, ou encaminhamento a apps Caixa, agência, 158/gov.br/Facilita ou SRTE/SINE.
6. **Pós-atendimento.** No lado bancário: SAC Caixa 0800 726 0101 (24h), Ouvidoria Caixa 0800 725 7474 (dias úteis, 9h às 18h, para "reclamações não solucionadas") e consumidor.gov.br, que tem link no rodapé da Caixa ([Caixa Atendimento](https://www.caixa.gov.br/atendimento/Paginas/default.aspx)). No lado do MTE: Fala.BR/CGU ([gov.br Solicitar](https://www.gov.br/pt-br/servicos/solicitar-o-seguro-desemprego)). Fora da esfera administrativa: ação judicial (ver a tabela de atores).

**2.3 Variantes que mudam a jornada telefônica**

- **Doméstico:** 1 salário mínimo, no máximo 3 meses, requerido do 7º ao 90º dia (LC 150, arts. 26 e 29; Res. 957, art. 46). A URA da Caixa atende igual na fase de pagamento [INFERÊNCIA].
- **Pescador artesanal:** MTE desde 1º/11/2025 (CTPS Digital/Emprega Brasil); INSS só para defesos até 31/10/2025; Fundacentro faz entrevistas em BA, AM, PI, PA e MA ([MTE](https://www.gov.br/trabalho-e-emprego/pt-br/noticias-e-conteudo/2025/novembro/seguro-defeso-passa-a-ser-administrado-pelo-ministerio-do-trabalho-e-emprego)). Entidades de pesca apoiam a revisão; a autenticação está em transição ([Lei 15.399](https://www.planalto.gov.br/ccivil_03/_ato2023-2026/2026/lei/l15399.htm)). Dúvida de concessão: MTE (defesos novos) ou INSS (antigos) [INFERÊNCIA].
- **Resgatado:** a Inspeção do Trabalho registra os dados em até 90 dias (Res. 957, art. 49, § 3º); 6 parcelas de 1 salário mínimo (Lei 7.998, art. 2º-C, redação da Lei 15.455/2026).
- **Bolsa qualificação:** contrato suspenso (CLT, art. 476-A); parcelas da bolsa descontadas do seguro em dispensa posterior, garantida ao menos uma (Res. 957, arts. 53 a 63).

### 3. Tabela de atores

Tipos: H = humano; I = institucional; S = sistema automatizado. Presença de IA = [NÃO CONFIRMADO], salvo indicação.

| Ator | Tipo | Papel | Entra na jornada | Sai da jornada | Fonte (URL) |
|---|---|---|---|---|---|
| Trabalhador requerente | H | Requer, consulta, saca e recorre | Na dispensa | Na última parcela ou no recurso/ação | https://www.gov.br/pt-br/servicos/solicitar-o-seguro-desemprego |
| Empregador | H/I | Entrega o requerimento e transmite os dados (Empregador Web/eSocial) | Na dispensa | Após o envio (volta se houver divergência) | https://portal.tcu.gov.br/imprensa/noticias/tribunal-avalia-servico-digital-de-seguro-desemprego-para-trabalhadores-formais |
| MTE (Secretaria do Trabalho) | I | Responsável pelo serviço: habilita, decide recursos em instância única e fiscaliza (art. 23) | No requerimento | Na decisão final | https://www.legisweb.com.br/legislacao/?id=436595 |
| Caixa Econômica Federal | I | Agente pagador (Res. 957, art. 64, § 1º); opera a URA, os apps e a rede | Na liberação / ligação | No pagamento ou no transbordo | https://www.caixa.gov.br/beneficios-trabalhador/seguro-desemprego/Paginas/default.aspx |
| Atendente humano CAIXA Cidadão | H | Atende o transbordo (seg.–sex. 8h–21h; sáb. 10h–16h) | No transbordo | No encerramento | https://www.caixa.gov.br/atendimento/Paginas/default.aspx |
| URA 0800 726 0207 | S | Autoatendimento 24h: menu, identificação, consulta (voz/IA: [NÃO CONFIRMADO]) | Na ligação | No encerramento ou transbordo | https://www.caixa.gov.br/atendimento/Paginas/default.aspx |
| Assistente virtual WhatsApp Caixa | S | Chatbot 24h (escopo para o seguro-desemprego: [NÃO CONFIRMADO]) | Canal alternativo | Ao responder | https://www.caixa.gov.br/atendimento/canais-digitais/whatsapp/Paginas/default.aspx |
| Apps CAIXA Tem / Benefícios Sociais CAIXA | S | Consulta da parcela; poupança social digital | Após a liberação | No saque | https://www.caixa.gov.br/beneficios-trabalhador/seguro-desemprego/perguntas-frequentes/Paginas/default.aspx |
| Lotéricas, correspondentes e terminais (biometria) | H/S | Saque com cartão e senha ou biometria | No saque | Após o saque | https://www.caixa.gov.br/beneficios-trabalhador/seguro-desemprego/perguntas-frequentes/Paginas/default.aspx |
| SAC e Ouvidoria Caixa | I | Reclamações bancárias; a Ouvidoria cuida das "não solucionadas" | Após falha | Na resposta | https://www.caixa.gov.br/atendimento/Paginas/default.aspx |
| Intérprete de Libras (parceiro Caixa) | H | Atendimento acessível | Sob demanda | Ao fim | https://www.caixa.gov.br/atendimento/Paginas/default.aspx |
| Dataprev | I | Opera os sistemas e o portal; transforma o eSocial na base "eSocial Negócio"; desenvolveu a Facilita | No requerimento | Na geração do pagamento [INFERÊNCIA] | https://portal.tcu.gov.br/imprensa/noticias/fragilidades-na-transparencia-do-esocial-aumentam-risco-de-pagamentos-indevidos |
| Motor de habilitação automática | S | Cruza bases e gera notificações | Após o requerimento | Na habilitação ou notificação | https://www.legisweb.com.br/legislacao/?id=436595 |
| CNIS / bases de benefícios (INSS) | S/I | Vínculos, remunerações e benefícios incompatíveis (art. 3º, V) | Na habilitação | Na habilitação | https://www.legisweb.com.br/legislacao/?id=436595 |
| eSocial e seu Comitê Gestor (Trabalho, RFB, INSS e outros); Serpro e Dataprev em apoio | S/I | Fonte dos dados do vínculo; governança do sistema | Na dispensa | Na habilitação | https://www.gov.br/esocial/pt-br/centrais-de-conteudo/legislacao/empresas/portaria-300_textoconsolidado.pdf |
| Receita Federal (RFB) | I | Coordena o Comitê Gestor do eSocial junto com a área do Trabalho | Fora do fluxo (governança dos dados) | — | https://www.gov.br/esocial/pt-br/centrais-de-conteudo/legislacao/empresas/portaria-300_textoconsolidado.pdf |
| Empregador Web | S | Sistema paralelo ao eSocial (duplicidade) | Na dispensa | Na habilitação | https://portal.tcu.gov.br/imprensa/noticias/tribunal-avalia-servico-digital-de-seguro-desemprego-para-trabalhadores-formais |
| Conta gov.br (identidade digital) | S | Login Prata/Ouro; notificações digitais (gestor: [NÃO CONFIRMADO]) | No requerimento/recurso | — | https://www.gov.br/pt-br/servicos/cadastrar-recurso-relativo-ao-seguro-desemprego |
| App CTPS Digital / Portal de Serviços | S | Requerimento, acompanhamento e recurso | No requerimento | No acompanhamento | https://www.gov.br/pt-br/servicos/solicitar-o-seguro-desemprego |
| Central Alô Trabalho 158 | H/S | Orientação e contato do MTE (operador: [NÃO CONFIRMADO]) | No transbordo da Caixa | Ao orientar | https://agenciagov.ebc.com.br/noticias/202607/saiba-como-acessar-os-canais-de-atendimento-do-ministerio-do-trabalho-e-emprego |
| Assistente virtual Celeste (MTE) | S | Orientações sobre serviços do MTE | Canal alternativo | Ao orientar | https://agenciagov.ebc.com.br/noticias/202607/saiba-como-acessar-os-canais-de-atendimento-do-ministerio-do-trabalho-e-emprego |
| Plataforma Facilita (MTE/Dataprev) | S | Atendimento remoto e agendamento presencial | Em pendência | Na resolução | https://www.gov.br/pt-br/servicos/solicitar-o-seguro-desemprego |
| SRTE e unidades SINE | H/I | Atendimento presencial subsidiário (Res. 957, art. 5º, § 2º) | Por agendamento | Ao concluir | https://www.legisweb.com.br/legislacao/?id=436595 |
| Inspeção do Trabalho | H/I | Resgate e registro de dados do trabalhador resgatado | Variante resgatado | Após o registro | https://www.legisweb.com.br/legislacao/?id=436595 |
| CODEFAT / FAT | I | Gere o FAT e edita a Res. 957 | Fora do fluxo | — | https://www.planalto.gov.br/ccivil_03/leis/l7998.htm |
| INSS | I | Defesos até 31/10/2025; bases de benefícios | Variante pescador antiga; habilitação | — | https://www.gov.br/trabalho-e-emprego/pt-br/noticias-e-conteudo/2025/novembro/seguro-defeso-passa-a-ser-administrado-pelo-ministerio-do-trabalho-e-emprego |
| MPA, Fundacentro, entidades de pesca e Telebrás | I | Variante pescador: autenticação (MPA), entrevistas (Fundacentro), apoio à revisão (entidades), recebe dados (Telebrás) | Variante pescador | — | https://www.planalto.gov.br/ccivil_03/_ato2023-2026/2026/lei/l15399.htm |
| CMN e Banco Central | I | Regulam a poupança social digital | Fora do fluxo | — | https://www.planalto.gov.br/ccivil_03/_ato2019-2022/2020/lei/L14075.htm |
| TCU | I | Controle externo | Fora do fluxo | — | https://portal.tcu.gov.br/imprensa/noticias/inconsistencias-no-seguro-desemprego-causaram-prejuizo-a-administracao-publica |
| CGU / Fala.BR | I | Manifestações sobre o serviço do MTE | Após falha | Na resposta | https://www.gov.br/pt-br/servicos/solicitar-o-seguro-desemprego |
| Justiça Federal (com AGU/DPU [INFERÊNCIA]) | I | Ordens judiciais de habilitação ou reemissão | Após o indeferimento | Na sentença | https://portal.tcu.gov.br/imprensa/noticias/inconsistencias-no-seguro-desemprego-causaram-prejuizo-a-administracao-publica |

### 4. Pontos de falha e responsáveis

| # | Falha | Evidência | Quem responde |
|---|---|---|---|
| F1 | Dúvida de concessão chega à Caixa, que só informa o pagamento | [FAQ Caixa](https://www.caixa.gov.br/beneficios-trabalhador/seguro-desemprego/perguntas-frequentes/Paginas/default.aspx) | MTE (Carta de Serviços, Lei 13.460, art. 7º) e Caixa (script de transbordo). Falta de transferência direta 0800→158: [INFERÊNCIA] |
| F2 | Duplicidade Empregador Web × eSocial, que gera bloqueios e recursos | [TCU 1621/2026](https://portal.tcu.gov.br/imprensa/noticias/tribunal-avalia-servico-digital-de-seguro-desemprego-para-trabalhadores-formais) | MTE (medidas em 180 dias); empregador |
| F3 | Base inconsistente, com possíveis pagamentos indevidos (indícios de R$ 147 mi e de cerca de R$ 544 mil) | [TCU 135/2024](https://portal.tcu.gov.br/imprensa/noticias/inconsistencias-no-seguro-desemprego-causaram-prejuizo-a-administracao-publica) | MTE (governança do contrato); Dataprev |
| F4 | Recursos repetitivos: cerca de 4 mil por ano em casos com dois indeferimentos anteriores; um caso analisado 15 vezes; instância única; sem análise dos pagamentos judiciais | TCU 135/2024; Res. 957, art. 28 | MTE |
| F5 | Sem base de conhecimento única: respostas divergentes e encaminhamentos sucessivos | TCU 1621/2026 | MTE (e, por extensão, a Caixa [INFERÊNCIA]) |
| F6 | Problemas operacionais impediram o acesso do TCU aos dados do eSocial | [TCU 1114/2025](https://portal.tcu.gov.br/imprensa/noticias/fragilidades-na-transparencia-do-esocial-aumentam-risco-de-pagamentos-indevidos) | MTE e Dataprev |
| F7 | Parcela devolvida ao FAT após 67 dias. O risco é mitigado pela reemissão em até 2 anos, mas o cidadão precisa saber pedi-la | Res. 957, art. 21 | Caixa (meios de pagamento); MTE (reemissão — canal [NÃO CONFIRMADO]) |
| F8 | Atendimento humano limitado a horários fixos; menus conhecidos só por fontes de 2018 | [Caixa Atendimento](https://www.caixa.gov.br/atendimento/Paginas/default.aspx) | Caixa |
| F9 | Golpes em canais de mensagem | [WhatsApp Caixa](https://www.caixa.gov.br/atendimento/canais-digitais/whatsapp/Paginas/default.aspx) | Caixa; cidadão |
| F10 | **(novo)** Carta de Serviços desatualizada: a página gov.br de recurso cita a Res. 467/2005, revogada em 2022 | [gov.br Recurso](https://www.gov.br/pt-br/servicos/cadastrar-recurso-relativo-ao-seguro-desemprego); [Res. 957](https://www.legisweb.com.br/legislacao/?id=436595) | MTE (Lei 13.460, art. 7º) |
| F11 | **(novo)** Transição do defeso: pescadores com defesos antigos (INSS) e novos (MTE), autenticação provisória e exclusões por falha biométrica | [Lei 15.399](https://www.planalto.gov.br/ccivil_03/_ato2023-2026/2026/lei/l15399.htm) | MTE, INSS, MPA |

### 5. Lacunas, incertezas e inferências

- **[LACUNA]** Menus vigentes da URA, tecnologia de voz, fornecedor do call center, operador do 158, comunicado primário da Caixa de 2018, íntegra dos acórdãos e composição atual do Comitê Gestor do eSocial.
- **[NÃO CONFIRMADO]** Gestor do gov.br; natureza federativa do Sine; canal da reemissão; escopo do WhatsApp Caixa.
- **[INFERÊNCIA]** Papéis LGPD (MTE controlador, Dataprev operadora); ANPD, Senacon e regras do BC sobre SAC; Caixa sujeita à Lei 13.460; Justiça Federal/AGU/DPU; fluxo do lote Dataprev→Caixa.
- **[INCERTEZA]** A Res. 957 foi alterada depois de publicada (ex.: Res. 1.027/2025); reconferir no DOU. A Lei 15.399 transfere a competência ao MTE só de forma indireta; a transferência expressa está na notícia do MTE.

### 6. Lista de fontes consultadas

1. https://www.caixa.gov.br/beneficios-trabalhador/seguro-desemprego/Paginas/default.aspx
2. https://www.caixa.gov.br/beneficios-trabalhador/seguro-desemprego/perguntas-frequentes/Paginas/default.aspx
3. https://www.caixa.gov.br/atendimento/Paginas/default.aspx
4. https://www.caixa.gov.br/atendimento/canais-digitais/whatsapp/Paginas/default.aspx
5. https://www.gov.br/pt-br/servicos/solicitar-o-seguro-desemprego
6. https://www.gov.br/pt-br/servicos/cadastrar-recurso-relativo-ao-seguro-desemprego
7. https://www.gov.br/trabalho-e-emprego/pt-br/noticias-e-conteudo/2025/novembro/seguro-defeso-passa-a-ser-administrado-pelo-ministerio-do-trabalho-e-emprego
8. https://www.gov.br/trabalho-e-emprego/pt-br/acesso-a-informacao/tratamento-de-dados-pessoais/PORTARIAMTEN1.889DE7DENOVEMBRODE2025.pdf
9. https://www.gov.br/esocial/pt-br/centrais-de-conteudo/legislacao/empresas/portaria-300_textoconsolidado.pdf
10. https://www.planalto.gov.br/ccivil_03/leis/l7998.htm
11. https://www.planalto.gov.br/ccivil_03/_ato2015-2018/2015/lei/l13134.htm
12. https://www.planalto.gov.br/ccivil_03/_ato2015-2018/2017/lei/l13460.htm
13. https://www.planalto.gov.br/ccivil_03/leis/lcp/lcp150.htm
14. https://www.planalto.gov.br/ccivil_03/_ato2019-2022/2020/lei/L14075.htm
15. https://www.planalto.gov.br/ccivil_03/_ato2023-2026/2026/lei/l15399.htm
16. https://www.planalto.gov.br/ccivil_03/_ato2011-2014/2014/decreto/d8373.htm
17. https://www.legisweb.com.br/legislacao/?id=436595 (Res. CODEFAT 957/2022 — reprodução secundária do texto normativo)
18. https://portal.tcu.gov.br/imprensa/noticias/inconsistencias-no-seguro-desemprego-causaram-prejuizo-a-administracao-publica
19. https://portal.tcu.gov.br/imprensa/noticias/fragilidades-na-transparencia-do-esocial-aumentam-risco-de-pagamentos-indevidos
20. https://portal.tcu.gov.br/imprensa/noticias/tribunal-avalia-servico-digital-de-seguro-desemprego-para-trabalhadores-formais
21. https://portal.tcu.gov.br/publicacoes-institucionais/sumarios-executivos/auditoria-seguro-desemprego-emprega-brasil
22. https://agenciagov.ebc.com.br/noticias/202512/facilita-brasil-governo-federal-lanca-novo-canal-digital-para-simplificar-servicos-a-trabalhadores-e-empresas
23. https://agenciagov.ebc.com.br/noticias/202607/saiba-como-acessar-os-canais-de-atendimento-do-ministerio-do-trabalho-e-emprego
24. https://jornalcontabil.com.br/noticia/seguro-desemprego-fgts-e-pis-tem-novas-datas-de-pagamento/ (secundária, 2018)
