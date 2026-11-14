# B — Relatório do assistente 1 (v3, final)

> Assistente 1: Claude (Anthropic, Claude Opus 5.5) com busca web · v3 em 14/11/2026, a partir de B_relatorio_auditoria_v2.md (auditoria do Grok, xAI, sobre a v2)

## v3

### 0. Registro de mudanças v2 → v3 (gatilho na audit_v2)

Legenda: (a) corrigido; (b) defendido com evidência; (c) pendente. Conferi cada gatilho na fonte antes de alterar o texto. Quando havia texto oficial (DOU/in.gov.br, portalfat.trabalho.gov.br, planalto.gov.br), ele substituiu a LegisWeb.

| Gatilho (R/N/ponto aberto) | Delta na v3 | Tratamento (a/b/c) | Fonte |
|---|---|---|---|
| R1 – CNIS/benefícios | Corrigido. O art. 4º, § 1º, da Res. 957 lista só bases de vínculo (CNIS, FGTS, GFIP, eSocial e documento judicial). O cruzamento com benefícios previdenciários volta a ser [INFERÊNCIA], com base no art. 22, II, que suspende o benefício quando começa a percepção de benefício de prestação continuada. O papel do INSS no CNIS foi ancorado no art. 29-A da Lei 8.213/1991. | (a) | [Res. 957 – DOU](https://www.in.gov.br/web/dou/-/resolucao-codefat-n-957-de-21-de-setembro-de-2022-431328890); [Lei 8.213](https://www.planalto.gov.br/ccivil_03/leis/l8213cons.htm) |
| R2 – Senacon/ANPD/call center/158 | Corrigido em parte. Entrou na tabela a Senacon/MJSP como gestora do consumidor.gov.br. A licitação CECOT 121/2026 da Caixa foi confirmada no PNCP: concorrência eletrônica, R$ 89.685.259,68 estimados, atendimento multimeios. A API do PNCP marca "existeResultado: false", e o vencedor não foi identificado. O horário do 158 (7h às 19h) foi incluído. A ANPD continua (c). Não consegui ler o documento Conecta TCU. | (a) | [PNCP API](https://pncp.gov.br/api/consulta/v1/orgaos/00360305000104/compras/2026/315); [consumidor.gov.br](https://www.consumidor.gov.br/pages/conteudo/sobre-servico); [MTE 158](https://www.gov.br/trabalho-e-emprego/pt-br/assuntos/inspecao-do-trabalho/acesso-a-informacao/central-alo-trabalho-158) |
| R3 – Gestor do gov.br | A SGD/MGI entrou como provedora da identidade gov.br, rotulada [INFERÊNCIA forte]. As páginas oficiais da conta estão no portal Governo Digital, e o MGI divulga os dados de níveis "segundo a SGD". Nenhuma das páginas lidas diz "gestora" de forma expressa. | (a) | [Governo Digital](https://www.gov.br/governodigital/pt-br/acessibilidade-e-usuario/atendimento-gov.br/atendimento-presencial/espaco-do-atendente-balcao-gov.br/nivel-da-conta); [MGI](https://www.gov.br/gestao/pt-br/assuntos/noticias/2025/maio/mais-de-100-milhoes-de-contas-gov-br-ja-sao-prata-ou-ouro) |
| R4 – Sine | Corrigido. A Lei 13.667/2018 organiza o Sine com gestão conjunta da União e dos entes que aderem (arts. 1º e 3º). A União executa o seguro-desemprego de forma privativa (art. 7º), e os municípios fazem a habilitação (art. 9º). | (a) | [Lei 13.667](https://www.planalto.gov.br/ccivil_03/_ato2015-2018/2018/lei/l13667.htm) |
| R5 – Menu da URA | Continua pendente. Não achei comunicado primário da Caixa com o menu. O fato de o edital CECOT 121 cobrir atendimento "telefônico" e "aplicativo de mensagens" não revela a tecnologia da URA. | (c) | [PNCP API](https://pncp.gov.br/api/consulta/v1/orgaos/00360305000104/compras/2026/315) |
| N1 – "Transferência indireta" | Corrigido. O art. 2º da Lei 10.779 é expresso: "Compete ao Ministério do Trabalho e Emprego (MTE) receber e processar os requerimentos e habilitar os beneficiários". A redação foi dada pela Lei 15.265, de 21/11/2025, art. 37, que entrou na linha do tempo. O § 4º do art. 2º vem da mesma lei. | (a) | [Lei 10.779](https://www.planalto.gov.br/ccivil_03/leis/2003/l10.779.htm); [Lei 15.265](https://www.planalto.gov.br/ccivil_03/_ato2023-2026/2025/lei/l15265.htm) |
| N2 – INSS defesos antigos | Corrigido. Deixou de ser inferência: a MP 1.323 (art. 2º) e a Lei 15.399 dão ao INSS os defesos até 31/10/2025, inclusive a apuração de irregularidades. | (a) | [MP 1.323](https://www.planalto.gov.br/ccivil_03/_ato2023-2026/2025/mpv/mpv1323.htm); [Lei 15.399](https://www.planalto.gov.br/ccivil_03/_ato2023-2026/2026/lei/l15399.htm) |
| N3 – Data da MP | Corrigido. A MP 1.323 é de 4/11/2025, foi publicada no DOU de 5/11/2025 e vigora desde a publicação (art. 4º). A data de 1º/11/2025 é o corte pelo início do defeso, não a data de vigência. | (a) | [MP 1.323](https://www.planalto.gov.br/ccivil_03/_ato2023-2026/2025/mpv/mpv1323.htm) |
| N4 – Transição do resgatado | Corrigido com o texto oficial. A Res. 1.043/2026 (DOU de 31/8/2026) dá ao art. 50 a redação "até 6 (seis) parcelas", e o § 3º restringe a regra a dispensas por resgate "a partir de 2 de julho de 2026". Uma fonte secundária falava em 2/6, o que estava errado. | (a) | [Res. 1.043](https://portalfat.trabalho.gov.br/wp-content/uploads/2026/09/Resolucao-Codefat-MTE-no-1043-de-26-de-agosto-de-2026-Altera-a-957-SD.pdf) |
| N5 – Alterações da 957 e norma do defeso | Corrigido. A Res. 1.031/2025 (DOU de 19/12/2025) alterou o art. 51. A Res. 1.043/2026 alterou o art. 50. A Res. 987/2023 alterou a bolsa qualificação. A Res. 1.027/2025, de 10/11/2025 (DOU extra de 24/11/2025), rege hoje o defeso. Seu art. 32 revogou na 957 o § 5º do art. 3º, o inciso V do art. 12 e o parágrafo único do art. 14. A 1.027 foi depois alterada pelas Res. 1.035/2026, 1.045/2026 e 1.046/2026. | (a) | [Portal FAT – resoluções](https://portalfat.mte.gov.br/resolucoes-2/resolucoes-por-assunto/seguro-desemprego/); [Res. 1.027](https://portalfat.trabalho.gov.br/wp-content/uploads/2026/11/Resolucao-no-1027-de-10.11.2025-SDPA.docx); [Res. 1.031](https://portalfat.trabalho.gov.br/wp-content/uploads/2026/01/Resolucao-no-1031-de-16.12.2025-SD_Altera-a-957-Trabalhador-Resgatado.docx) |
| N6 – Dependência da LegisWeb | Corrigido. Todas as citações da Res. 957 foram reconferidas no DOU (in.gov.br) e as alterações no Portal FAT. A LegisWeb saiu da lista de fontes. | (a) | [Res. 957 – DOU](https://www.in.gov.br/web/dou/-/resolucao-codefat-n-957-de-21-de-setembro-de-2022-431328890) |
| N7 – Empregador Web "ou" eSocial | Corrigido. O art. 40, § 1º, diz "exclusivamente por meio eletrônico no portal 'empregador web'". Na prática, o empregador alimenta Empregador Web **e** eSocial, a duplicidade apontada pelo TCU. | (a) | [Res. 957 – DOU](https://www.in.gov.br/web/dou/-/resolucao-codefat-n-957-de-21-de-setembro-de-2022-431328890); [TCU 1621/2026](https://portal.tcu.gov.br/imprensa/noticias/tribunal-avalia-servico-digital-de-seguro-desemprego-para-trabalhadores-formais) |
| N8 – Justiça do Trabalho | Corrigido. A Justiça do Trabalho entrou como emissora do "documento judicial" de vínculo (art. 4º, § 1º, V), rotulada [INFERÊNCIA], porque a resolução não diz qual Justiça emite o documento. A Justiça Federal ficou para as ações contra a União sobre o benefício, também [INFERÊNCIA]. | (a) | [Res. 957 – DOU](https://www.in.gov.br/web/dou/-/resolucao-codefat-n-957-de-21-de-setembro-de-2022-431328890) |
| N9 – FAQ e 158 | Corrigido. A FAQ da Caixa remete a concessão e valor ao "App CTPS Digital ou Portal Gov.br". O 158 aparece na FAQ só para agendar o atendimento presencial. | (a) | [FAQ Caixa](https://www.caixa.gov.br/beneficios-trabalhador/seguro-desemprego/perguntas-frequentes/Paginas/default.aspx) |
| N10 – Recurso e gov.br | Corrigido. A conta Prata/Ouro vale só para o canal digital. O art. 27, § 1º, admite recurso presencial em SRTE ou unidade do SINE. | (a) | [Res. 957 – DOU](https://www.in.gov.br/web/dou/-/resolucao-codefat-n-957-de-21-de-setembro-de-2022-431328890) |
| N11 – Notificação digital | Corrigido. A notificação digital "poderá" ser exclusiva, "mediante anuência" (art. 8º). Ao registrar recurso, o trabalhador é cientificado dessa regra (art. 27, § 3º). | (a) | [Res. 957 – DOU](https://www.in.gov.br/web/dou/-/resolucao-codefat-n-957-de-21-de-setembro-de-2022-431328890) |
| N12 – 158 como canal de requerimento | Corrigido e explicitado. A página gov.br lista "Telefone 158", e a Res. 957 (art. 5º) não o lista. A v3 registra a divergência: o 158 aparece como canal informado pela Carta de Serviços, e não como canal normativo. Não consegui confirmar se ele de fato protocola pedidos [NÃO CONFIRMADO]. | (a) | [gov.br Solicitar](https://www.gov.br/pt-br/servicos/solicitar-o-seguro-desemprego); [Res. 957 – DOU](https://www.in.gov.br/web/dou/-/resolucao-codefat-n-957-de-21-de-setembro-de-2022-431328890) |
| N13 – Papel do MPA | Corrigido. Pelo art. 2º, § 4º, da Lei 10.779, o papel legal do MPA é garantir ao MTE acesso às informações cadastrais do RGP. A autenticação nos sistemas do MPA e do MTE é só a transição do art. 7º da Lei 15.399. | (a) | [Lei 10.779](https://www.planalto.gov.br/ccivil_03/leis/2003/l10.779.htm) |
| N14 – Lei 14.075 | Corrigido. O CMN está no art. 2º, VII, e no § 1º, e o BC no inciso IX. O inciso VIII só menciona instituição autorizada pelo BC. | (a) | [Lei 14.075](https://www.planalto.gov.br/ccivil_03/_ato2019-2022/2020/lei/L14075.htm) |
| N15 – Autoria no cabeçalho da v2 | Corrigido. A atribuição "(ChatGPT)" no cabeçalho da v2 estava errada. O assistente 2, autor das auditorias v1 e v2, é o **Grok (xAI)**, como dizem os cabeçalhos das duas auditorias. O usuário confirmou isso ao coordenador. A v3 usa "Grok (xAI)" em todas as menções ao auditor. | (a) | B_relatorio_auditoria_v1.md e B_relatorio_auditoria_v2.md, linha 3 |
| N16 – Libras, deficiência auditiva e 158 | Corrigido. Incluí a ICOM como parceira de Libras nomeada pela Caixa, o canal 24h da Caixa para pessoas surdas e o horário do 158 (7h às 19h). A ligação ao 158 é gratuita só de telefone fixo. | (a) | [Caixa Atendimento](https://www.caixa.gov.br/atendimento/Paginas/default.aspx); [MTE 158](https://www.gov.br/trabalho-e-emprego/pt-br/assuntos/inspecao-do-trabalho/acesso-a-informacao/central-alo-trabalho-158) |
| PA1 – Íntegra dos acórdãos | Continua sem leitura da íntegra. Uso só as notícias e o sumário do TCU. | (c) | [TCU sumário](https://portal.tcu.gov.br/publicacoes-institucionais/sumarios-executivos/auditoria-seguro-desemprego-emprega-brasil) |
| PA2 – Comitê Gestor do eSocial atual | A busca restrita a gov.br e in.gov.br só achou a Portaria ME 300/2019, alterada pela Portaria ME 58/2020. A composição pós-2023 não foi localizada. | (c) | [Portaria 300](https://www.gov.br/esocial/pt-br/centrais-de-conteudo/legislacao/empresas/portaria-300_textoconsolidado.pdf) |
| PA3 – Data da MP 1.323 e defesos de 1º a 4/11 | A MP foi publicada no DOU de 5/11/2025. Pelo art. 2º, o INSS fica só com os defesos até 31/10, e a Res. 1.027 (art. 1º) aplica as novas regras aos defesos "iniciados a partir de 1º de novembro de 2025". Os defesos de 1º a 4/11 ficaram com o MTE, com aplicação retroativa ao início do defeso. A consequência prática fica [INFERÊNCIA]. | (a) | [MP 1.323](https://www.planalto.gov.br/ccivil_03/_ato2023-2026/2025/mpv/mpv1323.htm); [Res. 1.027](https://portalfat.trabalho.gov.br/wp-content/uploads/2026/11/Resolucao-no-1027-de-10.11.2025-SDPA.docx) |
| PA4 – Resolução do pescador | Resolvido: Res. CODEFAT/MTE 1.027/2025 (ver N5). | (a) | [Res. 1.027](https://portalfat.trabalho.gov.br/wp-content/uploads/2026/11/Resolucao-no-1027-de-10.11.2025-SDPA.docx) |
| PA5 – Texto consolidado da 957 em fonte oficial | Usei o original no DOU e os atos de alteração no Portal FAT. O Portal FAT não exibe versão consolidada. | (a) | [Portal FAT](https://portalfat.mte.gov.br/resolucoes-2/resolucoes-por-assunto/seguro-desemprego/) |
| PA6 – Data da Lei 15.455/2026 | Lei de 1º/7/2026, publicada no DOU de 2/7/2026 e em vigor na publicação (art. 10). O art. 5º altera o art. 2º-C. | (a) | [Lei 15.455](https://www.planalto.gov.br/ccivil_03/_ato2023-2026/2026/lei/l15455.htm) |
| PA7 – Canal de reemissão | Resolvido só em parte. Para defesos do INSS, a reemissão é pedida no Meu INSS (ou pelo 135), com prazo de até 45 dias. Para o trabalhador formal, não achei serviço gov.br de reemissão. A Res. 957, art. 21, § 2º, só diz "a partir de solicitação do beneficiário". | (c) | [gov.br Reemitir defeso](https://www.gov.br/pt-br/servicos/reemitir-parcelas-seguro-defeso) |
| PA8 – INSS no CNIS | Resolvido: art. 29-A da Lei 8.213 ("O INSS utilizará as informações constantes no CNIS..."). | (a) | [Lei 8.213](https://www.planalto.gov.br/ccivil_03/leis/l8213cons.htm) |
| PA9 – Lei 13.667/2018 | Resolvido (ver R4). | (a) | [Lei 13.667](https://www.planalto.gov.br/ccivil_03/_ato2015-2018/2018/lei/l13667.htm) |
| PA10 – SGD/MGI | Resolvido em parte (ver R3). | (a) | [Governo Digital](https://www.gov.br/governodigital/pt-br/acessibilidade-e-usuario/atendimento-gov.br/atendimento-presencial/espaco-do-atendente-balcao-gov.br/nivel-da-conta) |
| PA11 – Vencedor da CECOT 121/2026 e operador do 158 | **Não confirmei o vencedor.** O PNCP mostra situação "Divulgada", sem resultado. A página do 158 não diz se o serviço é terceirizado. | (c) | [PNCP API](https://pncp.gov.br/api/consulta/v1/orgaos/00360305000104/compras/2026/315); [MTE 158](https://www.gov.br/trabalho-e-emprego/pt-br/assuntos/inspecao-do-trabalho/acesso-a-informacao/central-alo-trabalho-158) |
| PA12 – Menu e tecnologia de voz da URA | Continua pendente (ver R5). Recomendo uma ligação de teste documentada. | (c) | — |

### 1. Sumário executivo

- A jornada é **bifurcada**. O **MTE** concede o benefício, com habilitação automática nos sistemas operados pela Dataprev. A **Caixa** paga, como agente pagador fixado pela Res. CODEFAT 957/2022, art. 64, § 1º ([DOU](https://www.in.gov.br/web/dou/-/resolucao-codefat-n-957-de-21-de-setembro-de-2022-431328890)).
- A URA **0800 726 0207** (CAIXA Cidadão) tem atendimento eletrônico 24h. O atendimento humano funciona de segunda a sexta, das 8h às 21h, e aos sábados, das 10h às 16h ([Caixa](https://www.caixa.gov.br/atendimento/Paginas/default.aspx)). Ela informa **pagamento**. Dúvidas de concessão vão para a CTPS Digital ou o gov.br ([FAQ](https://www.caixa.gov.br/beneficios-trabalhador/seguro-desemprego/perguntas-frequentes/Paginas/default.aspx)).
- O **158** do MTE funciona das 7h às 19h, com atendimento eletrônico ou humano ([MTE](https://www.gov.br/trabalho-e-emprego/pt-br/assuntos/inspecao-do-trabalho/acesso-a-informacao/central-alo-trabalho-158)).
- O **defeso** do pescador é do MTE para os defesos iniciados a partir de 1º/11/2025 (Lei 10.779, art. 2º, na redação da Lei 15.265/2025; Res. 1.027/2025). O **resgatado** tem até 6 parcelas para dispensas a partir de 2/7/2026 (Res. 1.043/2026).
- A Caixa licitou atendimento multimeios (CECOT 121/2026, R$ 89,7 mi estimados). Não há resultado publicado no PNCP.
- Continuam sem fonte primária: o menu atual da URA, a tecnologia de voz, o fornecedor e o operador do 158.

### 2. Linha do tempo da jornada

**2.1 Marcos (2015–2026)**

| Data | Marco | Fonte |
|---|---|---|
| 2015 | A Lei 13.134 fixa a carência (12/18, 9/12 e cada um dos 6 meses imediatamente anteriores) e 3 a 5 parcelas. O INSS passa a cuidar do defeso. A LC 150 cria o seguro do doméstico: 1 salário mínimo, no máximo 3 meses, do 7º ao 90º dia. | [Lei 13.134](https://www.planalto.gov.br/ccivil_03/_ato2015-2018/2015/lei/l13134.htm); [LC 150](https://www.planalto.gov.br/ccivil_03/leis/lcp/lcp150.htm) |
| 2017–2018 | A Lei 13.460 disciplina ouvidorias e a Carta de Serviços na administração direta e indireta. A Lei 13.667 organiza o Sine. | [Lei 13.460](https://www.planalto.gov.br/ccivil_03/_ato2015-2018/2017/lei/l13460.htm); [Lei 13.667](https://www.planalto.gov.br/ccivil_03/_ato2015-2018/2018/lei/l13667.htm) |
| 2019–2020 | A Portaria ME 300/2019 cria o Comitê Gestor do eSocial. A Lei 14.075/2020 cria a poupança social digital. | [Portaria 300](https://www.gov.br/esocial/pt-br/centrais-de-conteudo/legislacao/empresas/portaria-300_textoconsolidado.pdf); [Lei 14.075](https://www.planalto.gov.br/ccivil_03/_ato2019-2022/2020/lei/L14075.htm) |
| 23/09/2022 (vigência 3/10) | Publicação da Res. CODEFAT 957/2022, que revoga a 467/2005 (art. 68, XLVII). | [DOU](https://www.in.gov.br/web/dou/-/resolucao-codefat-n-957-de-21-de-setembro-de-2022-431328890) |
| 31/01/2024 | Acórdão TCU 135/2024. | [TCU](https://portal.tcu.gov.br/imprensa/noticias/inconsistencias-no-seguro-desemprego-causaram-prejuizo-a-administracao-publica) |
| 21/05/2025 | Acórdão TCU 1114/2025. | [TCU](https://portal.tcu.gov.br/imprensa/noticias/fragilidades-na-transparencia-do-esocial-aumentam-risco-de-pagamentos-indevidos) |
| 05/11/2025 | Publicação da MP 1.323 (de 4/11). O defeso passa ao MTE para defesos iniciados a partir de 1º/11/2025. | [MP 1.323](https://www.planalto.gov.br/ccivil_03/_ato2023-2026/2025/mpv/mpv1323.htm); [MTE](https://www.gov.br/trabalho-e-emprego/pt-br/noticias-e-conteudo/2025/novembro/seguro-defeso-passa-a-ser-administrado-pelo-ministerio-do-trabalho-e-emprego) |
| 21/11/2025 | O art. 37 da Lei 15.265 dá nova redação ao art. 2º da Lei 10.779: competência expressa do MTE, biometria e acesso ao RGP pelo MPA. | [Lei 15.265](https://www.planalto.gov.br/ccivil_03/_ato2023-2026/2025/lei/l15265.htm) |
| 24/11/2025 | Publicação da Res. 1.027/2025 (defeso), em DOU extra. | [Res. 1.027](https://portalfat.trabalho.gov.br/wp-content/uploads/2026/11/Resolucao-no-1027-de-10.11.2025-SDPA.docx) |
| 18/12/2025 | Lançamento oficial da Facilita. A Celeste é citada na mesma matéria. | [Agência Gov](https://agenciagov.ebc.com.br/noticias/202512/facilita-brasil-governo-federal-lanca-novo-canal-digital-para-simplificar-servicos-a-trabalhadores-e-empresas) |
| 19/12/2025 | A Res. 1.031 altera o art. 51 da 957 (resgatado). | [Res. 1.031](https://portalfat.trabalho.gov.br/wp-content/uploads/2026/01/Resolucao-no-1031-de-16.12.2025-SD_Altera-a-957-Trabalhador-Resgatado.docx) |
| 04/05/2026 | A Lei 15.399 converte a MP 1.323 e cria a transição de autenticação (art. 7º). | [Lei 15.399](https://www.planalto.gov.br/ccivil_03/_ato2023-2026/2026/lei/l15399.htm) |
| 15/05/2026 | A Caixa divulga no PNCP a CECOT 121/2026 (atendimento multimeios). | [PNCP](https://pncp.gov.br/api/consulta/v1/orgaos/00360305000104/compras/2026/315) |
| 24/06/2026 | Acórdão TCU 1621/2026: o MTE deve "tomar medidas para integrar" o benefício ao eSocial em 180 dias. | [TCU](https://portal.tcu.gov.br/imprensa/noticias/tribunal-avalia-servico-digital-de-seguro-desemprego-para-trabalhadores-formais) |
| 02/07/2026 | Publicação da Lei 15.455, que fixa 6 parcelas para o resgatado. | [Lei 15.455](https://www.planalto.gov.br/ccivil_03/_ato2023-2026/2026/lei/l15455.htm) |
| 31/08/2026 | Publicação da Res. 1.043, que dá ao art. 50 da 957 "até 6 parcelas" para dispensas a partir de 2/7/2026. | [Res. 1.043](https://portalfat.trabalho.gov.br/wp-content/uploads/2026/09/Resolucao-Codefat-MTE-no-1043-de-26-de-agosto-de-2026-Altera-a-957-SD.pdf) |

**2.2 Jornada do trabalhador formal**

1. **Dispensa.** O empregador transmite os dados "exclusivamente" pelo Empregador Web, com certificado ICP-Brasil (Res. 957, art. 40, § 1º), e também informa o desligamento ao eSocial. É a duplicidade apontada pelo TCU 1621/2026.
2. **Requerimento, do 7º ao 120º dia** (Lei 7.998, art. 6º; Res. 957, art. 41).
   - **Canal normativo:** gov.br ou CTPS Digital (art. 5º). O presencial em SRTE ou SINE só vale quando o meio digital é impossível (art. 5º, § 2º).
   - **Canal na Carta de Serviços:** a página gov.br aponta o "Portal de Serviços" (link na Dataprev), lista o "Telefone 158" e manda agendar o presencial pela Facilita ([gov.br](https://www.gov.br/pt-br/servicos/solicitar-o-seguro-desemprego)).
   - **Divergência:** a resolução não prevê o 158 como canal de requerimento.
   - A URA da Caixa não recebe requerimento [INFERÊNCIA: ausente das duas listas].
3. **Habilitação automática.** O sistema cruza CNIS, guia do FGTS, GFIP, eSocial ou documento judicial (art. 4º, § 1º). O cruzamento com benefícios previdenciários é [INFERÊNCIA], pelo art. 3º, V, da Lei 7.998 e pelo art. 22, II, da Res. 957. A notificação pode ser só digital, mediante anuência (art. 8º). O recurso cabe em 120 dias, em instância única pela Secretaria de Trabalho, e pode ser apresentado pelo gov.br, pela CTPS Digital ou presencialmente em SRTE ou SINE (arts. 27 e 28).
4. **Pagamento.** A 1ª parcela sai 30 dias após o requerimento (art. 12). A ordem de crédito é: conta indicada, poupança Caixa, poupança social digital (CAIXA Tem), cartão ou biometria, agência. A parcela fica disponível por 67 dias e depois volta ao FAT. Pode ser reemitida a pedido do beneficiário ou por ordem judicial, em até 2 anos (art. 21) ([FAQ Caixa](https://www.caixa.gov.br/beneficios-trabalhador/seguro-desemprego/perguntas-frequentes/Paginas/default.aspx)).
5. **URA 0800 726 0207.**
   - (a) **Entrada:** atendimento eletrônico 24h.
   - (b) **Menu:** a "opção 5" consta de matéria de 2018 [NÃO CONFIRMADO em 2026] ([Jornal Contábil](https://jornalcontabil.com.br/noticia/seguro-desemprego-fgts-e-pis-tem-novas-datas-de-pagamento/)).
   - (c) **Identificação:** NIS e "identificação positiva" [NÃO CONFIRMADO em 2026]. Uso de reconhecimento de voz: [NÃO CONFIRMADO].
   - (d) **Consulta:** situação e data da parcela; conta de crédito só se for conta Caixa.
   - (e) **Transbordo:** atendente humano no horário oficial, ou indicação dos canais do MTE (CTPS Digital/gov.br). O 158 serve para orientação, das 7h às 19h, e é gratuito só de telefone fixo.
   - (f) **Acessibilidade:** canal 24h para pessoas surdas e intérprete de Libras via ICOM, parceira da Caixa.
6. **Pós-atendimento.**
   - **Lado bancário:** SAC Caixa (24h), Ouvidoria Caixa (dias úteis, das 9h às 18h) e consumidor.gov.br, gerido pela Senacon/MJSP.
   - **Lado do MTE:** Fala.BR/CGU.
   - **Via judicial:** Justiça Federal [INFERÊNCIA].

**2.3 Variantes**

- **Doméstico:** 1 salário mínimo, no máximo 3 meses, do 7º ao 90º dia (LC 150, arts. 26 e 29; Res. 957, arts. 46 e 47).
- **Pescador:**
  - **Defesos a partir de 1º/11/2025:** MTE (Lei 10.779, art. 2º; Res. 1.027/2025), com requerimento no gov.br ou na CTPS Digital e presencial só em impossibilidade comprovada (Res. 1.027, art. 5º [número de artigo NÃO CONFIRMADO; texto lido]). O MPA garante o acesso ao RGP (art. 2º, § 4º). A biometria é exigida (art. 2º, § 10, da Lei 10.779, na redação da Lei 15.265). A Fundacentro faz entrevistas, e as entidades de pesca apoiam a revisão.
  - **Defesos até 31/10/2025:** INSS, inclusive para a reemissão no Meu INSS ou pelo 135 ([gov.br](https://www.gov.br/pt-br/servicos/reemitir-parcelas-seguro-defeso)).
- **Resgatado:** a Inspeção do Trabalho registra os dados. Desde a Res. 1.031, a relação encerrada pela fiscalização habilita a modalidade, e prevalece a modalidade mais favorável (art. 51). São até 6 parcelas para dispensas a partir de 2/7/2026; antes disso, 3.
- **Bolsa qualificação:** Res. 957, arts. 53 a 63, com alterações da Res. 987/2023.

### 3. Tabela de atores (final)

Coluna "URA": **Sim** = atua na jornada telefônica; **Indireto** = é para onde a URA encaminha ou de onde vem o dado consultado; **Variante** = só nas variantes.

**3.1 Atores humanos**

| Ator | Papel | URA | Entra | Sai | Fonte |
|---|---|---|---|---|---|
| Trabalhador formal | Requer, consulta, saca e recorre | Sim | Na dispensa | Na última parcela ou na decisão | https://www.gov.br/pt-br/servicos/solicitar-o-seguro-desemprego |
| Empregador (e seu contador) | Transmite os dados (Empregador Web e eSocial) | Indireto | Na dispensa | Após o envio | https://www.in.gov.br/web/dou/-/resolucao-codefat-n-957-de-21-de-setembro-de-2022-431328890 |
| Atendente CAIXA Cidadão | Atende o transbordo (seg.–sex. 8h–21h; sáb. 10h–16h) | Sim | No transbordo | No encerramento | https://www.caixa.gov.br/atendimento/Paginas/default.aspx |
| Intérprete de Libras (ICOM) | Atendimento acessível | Sim | Sob demanda | Ao fim | https://www.caixa.gov.br/atendimento/Paginas/default.aspx |
| Atendente do 158 | Orientação (7h–19h) | Indireto | No encaminhamento | Ao orientar | https://www.gov.br/trabalho-e-emprego/pt-br/assuntos/inspecao-do-trabalho/acesso-a-informacao/central-alo-trabalho-158 |
| Atendentes de SRTE e SINE | Requerimento e recurso presenciais | Indireto | Por agendamento | Ao concluir | https://www.planalto.gov.br/ccivil_03/_ato2015-2018/2018/lei/l13667.htm |
| Operadores de lotérica e correspondente | Pagamento com cartão e senha | Indireto | No saque | Após o saque | https://www.caixa.gov.br/beneficios-trabalhador/seguro-desemprego/perguntas-frequentes/Paginas/default.aspx |
| Auditores-fiscais do Trabalho | Resgate e registro de dados | Variante | No resgate | No registro | https://portalfat.trabalho.gov.br/wp-content/uploads/2026/01/Resolucao-no-1031-de-16.12.2025-SD_Altera-a-957-Trabalhador-Resgatado.docx |
| Pescador artesanal e entidades de pesca | Requerimento e apoio à revisão | Variante | No defeso | No pagamento | https://www.planalto.gov.br/ccivil_03/_ato2023-2026/2026/lei/l15399.htm |
| Empregado doméstico e empregador doméstico | Regras próprias (LC 150) | Variante | Na dispensa | Na 3ª parcela | https://www.planalto.gov.br/ccivil_03/leis/lcp/lcp150.htm |

**3.2 Atores de IA e sistemas automatizados** (presença de IA [NÃO CONFIRMADO] em todos)

| Ator | Papel | URA | Fonte |
|---|---|---|---|
| URA 0800 726 0207 (DTMF e/ou voz: [NÃO CONFIRMADO]) | Autoatendimento 24h e consulta da parcela | Sim | https://www.caixa.gov.br/atendimento/Paginas/default.aspx |
| URA/eletrônico do 158 | Atendimento automatizado do MTE | Indireto | https://www.gov.br/trabalho-e-emprego/pt-br/assuntos/inspecao-do-trabalho/acesso-a-informacao/central-alo-trabalho-158 |
| Assistente virtual do WhatsApp Caixa | Chatbot 24h | Indireto | https://www.caixa.gov.br/atendimento/canais-digitais/whatsapp/Paginas/default.aspx |
| Celeste (MTE) | Assistente virtual de orientação | Indireto | https://agenciagov.ebc.com.br/noticias/202607/saiba-como-acessar-os-canais-de-atendimento-do-ministerio-do-trabalho-e-emprego |
| Sistema Seguro-Desemprego (motor de habilitação) | Cruzamento automático (art. 4º) e notificações | Indireto (origina o dado consultado) | https://www.in.gov.br/web/dou/-/resolucao-codefat-n-957-de-21-de-setembro-de-2022-431328890 |
| CNIS, FGTS, GFIP, eSocial / "eSocial Negócio" | Bases de vínculo | Indireto | https://portal.tcu.gov.br/imprensa/noticias/fragilidades-na-transparencia-do-esocial-aumentam-risco-de-pagamentos-indevidos |
| Empregador Web | Transmissão obrigatória do requerimento | Indireto | https://www.in.gov.br/web/dou/-/resolucao-codefat-n-957-de-21-de-setembro-de-2022-431328890 |
| Conta gov.br (Bronze/Prata/Ouro) | Identidade digital e anuência para notificação | Indireto | https://www.gov.br/governodigital/pt-br/acessibilidade-e-usuario/atendimento-gov.br/atendimento-presencial/espaco-do-atendente-balcao-gov.br/nivel-da-conta |
| CTPS Digital / Portal de Serviços / Facilita | Requerimento, recurso e agendamento | Indireto (destino do transbordo) | https://www.gov.br/pt-br/servicos/solicitar-o-seguro-desemprego |
| Apps CAIXA Tem / Benefícios Sociais; terminais com biometria | Consulta e saque | Indireto | https://www.caixa.gov.br/beneficios-trabalhador/seguro-desemprego/perguntas-frequentes/Paginas/default.aspx |
| Meu INSS | Reemissão de defesos antigos | Variante | https://www.gov.br/pt-br/servicos/reemitir-parcelas-seguro-defeso |
| Validação biométrica do pescador | Autenticação | Variante | https://www.planalto.gov.br/ccivil_03/leis/2003/l10.779.htm |

**3.3 Atores institucionais**

| Ator | Papel | URA | Fonte |
|---|---|---|---|
| Caixa Econômica Federal | Agente pagador; dona da URA; contratante da CECOT 121/2026 | Sim | https://pncp.gov.br/api/consulta/v1/orgaos/00360305000104/compras/2026/315 |
| Fornecedor do call center Caixa | Opera o atendimento ([NÃO CONFIRMADO]: sem resultado no PNCP) | Sim | https://pncp.gov.br/api/consulta/v1/orgaos/00360305000104/compras/2026/315 |
| SAC/Ouvidoria Caixa | Reclamações bancárias | Sim (pós) | https://www.caixa.gov.br/atendimento/Paginas/default.aspx |
| MTE / Secretaria de Trabalho | Concede, julga recursos e fiscaliza | Indireto | https://www.in.gov.br/web/dou/-/resolucao-codefat-n-957-de-21-de-setembro-de-2022-431328890 |
| Dataprev | Opera os sistemas e o portal; base "eSocial Negócio"; Facilita | Indireto | https://portal.tcu.gov.br/imprensa/noticias/inconsistencias-no-seguro-desemprego-causaram-prejuizo-a-administracao-publica |
| CODEFAT / FAT | Normatiza (Res. 957 e 1.027) e financia | Indireto | https://portalfat.mte.gov.br/resolucoes-2/resolucoes-por-assunto/seguro-desemprego/ |
| Comitê Gestor do eSocial (Trabalho, RFB, INSS e outros); Serpro e Dataprev em apoio | Governança dos dados | Indireto | https://www.gov.br/esocial/pt-br/centrais-de-conteudo/legislacao/empresas/portaria-300_textoconsolidado.pdf |
| INSS | Mantém o uso do CNIS (Lei 8.213, art. 29-A); defesos até 31/10/2025 | Indireto / Variante | https://www.planalto.gov.br/ccivil_03/leis/l8213cons.htm |
| Sine (União, estados e municípios) | Habilitação municipal; atendimento | Indireto | https://www.planalto.gov.br/ccivil_03/_ato2015-2018/2018/lei/l13667.htm |
| SGD/MGI | Provedora da identidade gov.br [INFERÊNCIA forte] | Indireto | https://www.gov.br/gestao/pt-br/assuntos/noticias/2025/maio/mais-de-100-milhoes-de-contas-gov-br-ja-sao-prata-ou-ouro |
| CMN e Banco Central | Regulam a poupança social digital | Indireto | https://www.planalto.gov.br/ccivil_03/_ato2019-2022/2020/lei/L14075.htm |
| Senacon/MJSP | Gere o consumidor.gov.br | Sim (pós) | https://www.consumidor.gov.br/pages/conteudo/sobre-servico |
| CGU (Fala.BR) | Manifestações sobre o MTE | Indireto | https://www.gov.br/pt-br/servicos/solicitar-o-seguro-desemprego |
| TCU | Controle externo | Fora do fluxo | https://portal.tcu.gov.br/imprensa/noticias/tribunal-avalia-servico-digital-de-seguro-desemprego-para-trabalhadores-formais |
| Justiça do Trabalho [INFERÊNCIA] / Justiça Federal [INFERÊNCIA] | Documento judicial de vínculo / ações sobre o benefício | Indireto | https://www.in.gov.br/web/dou/-/resolucao-codefat-n-957-de-21-de-setembro-de-2022-431328890 |
| MPA, Fundacentro, Telebrás | Acesso ao RGP; entrevistas; recebe dados (Portaria MTE 1.889/2025) | Variante | https://www.planalto.gov.br/ccivil_03/leis/2003/l10.779.htm |

### 4. Pontos de falha e responsáveis

| # | Falha | Quem responde | Fonte |
|---|---|---|---|
| F1 | Dúvida de concessão chega à URA, que só informa pagamento; não há evidência de transferência direta ao 158 [INFERÊNCIA] | MTE (Carta de Serviços) e Caixa (roteiro de transbordo) | [FAQ Caixa](https://www.caixa.gov.br/beneficios-trabalhador/seguro-desemprego/perguntas-frequentes/Paginas/default.aspx) |
| F2 | Duplicidade Empregador Web × eSocial | MTE (medidas em 180 dias); empregador | [TCU 1621/2026](https://portal.tcu.gov.br/imprensa/noticias/tribunal-avalia-servico-digital-de-seguro-desemprego-para-trabalhadores-formais) |
| F3 | Possíveis pagamentos indevidos (indícios de R$ 147 mi e de cerca de R$ 544 mil) | MTE; Dataprev | [TCU 135/2024](https://portal.tcu.gov.br/imprensa/noticias/inconsistencias-no-seguro-desemprego-causaram-prejuizo-a-administracao-publica) |
| F4 | Recursos repetitivos em instância única | MTE | TCU 135/2024; Res. 957, art. 28 |
| F5 | Sem base de conhecimento única | MTE (e a Caixa, por extensão [INFERÊNCIA]) | TCU 1621/2026 |
| F6 | Acesso do controle ao eSocial prejudicado por problemas operacionais | MTE; Dataprev | [TCU 1114/2025](https://portal.tcu.gov.br/imprensa/noticias/fragilidades-na-transparencia-do-esocial-aumentam-risco-de-pagamentos-indevidos) |
| F7 | Devolução ao FAT após 67 dias; canal de reemissão do formal não documentado | Caixa; MTE | Res. 957, art. 21 |
| F8 | Horários diferentes entre a URA Caixa (humano até 21h) e o 158 (até 19h); 158 gratuito só de fixo | Caixa; MTE | [Caixa](https://www.caixa.gov.br/atendimento/Paginas/default.aspx); [MTE 158](https://www.gov.br/trabalho-e-emprego/pt-br/assuntos/inspecao-do-trabalho/acesso-a-informacao/central-alo-trabalho-158) |
| F9 | Carta de Serviços desatualizada: a página de recurso cita a Res. 467/2005, revogada | MTE | [gov.br Recurso](https://www.gov.br/pt-br/servicos/cadastrar-recurso-relativo-ao-seguro-desemprego) |
| F10 | 158 listado como canal de requerimento sem previsão na Res. 957 | MTE/CODEFAT | [gov.br](https://www.gov.br/pt-br/servicos/solicitar-o-seguro-desemprego) |
| F11 | Defeso com regime duplo: INSS para os antigos, MTE para os novos, com biometria e prazos alterados várias vezes (Res. 1.035, 1.045 e 1.046) | MTE, INSS, MPA, CODEFAT | [Portal FAT](https://portalfat.mte.gov.br/resolucoes-2/resolucoes-por-assunto/seguro-desemprego/) |

### 5. Lacunas, incertezas e inferências

- **[LACUNA]** Menu atual da URA; tecnologia de voz; vencedor da CECOT 121/2026; operador do 158; íntegra dos acórdãos; composição atual do Comitê Gestor do eSocial; canal de reemissão do formal.
- **[NÃO CONFIRMADO]** O 158 como canal efetivo de protocolo; escopo do WhatsApp Caixa para o seguro-desemprego; numeração dos artigos da Res. 1.027 após as alterações de 2026.
- **[INFERÊNCIA]**
  - cruzamento com benefícios previdenciários;
  - Justiça do Trabalho como emissora do documento judicial;
  - Justiça Federal como foro das ações;
  - papéis na LGPD (MTE controlador, Dataprev operadora) e papel da ANPD;
  - SGD/MGI como gestora do gov.br;
  - fluxo do lote de pagamento Dataprev → Caixa.

### 6. Lista de fontes consultadas

1. https://www.caixa.gov.br/beneficios-trabalhador/seguro-desemprego/Paginas/default.aspx
2. https://www.caixa.gov.br/beneficios-trabalhador/seguro-desemprego/perguntas-frequentes/Paginas/default.aspx
3. https://www.caixa.gov.br/atendimento/Paginas/default.aspx
4. https://www.caixa.gov.br/atendimento/canais-digitais/whatsapp/Paginas/default.aspx
5. https://pncp.gov.br/api/consulta/v1/orgaos/00360305000104/compras/2026/315
6. https://www.gov.br/pt-br/servicos/solicitar-o-seguro-desemprego
7. https://www.gov.br/pt-br/servicos/cadastrar-recurso-relativo-ao-seguro-desemprego
8. https://www.gov.br/pt-br/servicos/reemitir-parcelas-seguro-defeso
9. https://www.gov.br/trabalho-e-emprego/pt-br/assuntos/inspecao-do-trabalho/acesso-a-informacao/central-alo-trabalho-158
10. https://www.gov.br/trabalho-e-emprego/pt-br/noticias-e-conteudo/2025/novembro/seguro-defeso-passa-a-ser-administrado-pelo-ministerio-do-trabalho-e-emprego
11. https://www.gov.br/trabalho-e-emprego/pt-br/acesso-a-informacao/tratamento-de-dados-pessoais/PORTARIAMTEN1.889DE7DENOVEMBRODE2025.pdf
12. https://www.gov.br/esocial/pt-br/centrais-de-conteudo/legislacao/empresas/portaria-300_textoconsolidado.pdf
13. https://www.gov.br/governodigital/pt-br/acessibilidade-e-usuario/atendimento-gov.br/atendimento-presencial/espaco-do-atendente-balcao-gov.br/nivel-da-conta
14. https://www.gov.br/gestao/pt-br/assuntos/noticias/2025/maio/mais-de-100-milhoes-de-contas-gov-br-ja-sao-prata-ou-ouro
15. https://www.consumidor.gov.br/pages/conteudo/sobre-servico
16. https://www.in.gov.br/web/dou/-/resolucao-codefat-n-957-de-21-de-setembro-de-2022-431328890
17. https://portalfat.mte.gov.br/resolucoes-2/resolucoes-por-assunto/seguro-desemprego/
18. https://portalfat.trabalho.gov.br/wp-content/uploads/2026/11/Resolucao-no-1027-de-10.11.2025-SDPA.docx
19. https://portalfat.trabalho.gov.br/wp-content/uploads/2026/01/Resolucao-no-1031-de-16.12.2025-SD_Altera-a-957-Trabalhador-Resgatado.docx
20. https://portalfat.trabalho.gov.br/wp-content/uploads/2026/09/Resolucao-Codefat-MTE-no-1043-de-26-de-agosto-de-2026-Altera-a-957-SD.pdf
21. https://www.planalto.gov.br/ccivil_03/leis/l7998.htm
22. https://www.planalto.gov.br/ccivil_03/_ato2015-2018/2015/lei/l13134.htm
23. https://www.planalto.gov.br/ccivil_03/leis/lcp/lcp150.htm
24. https://www.planalto.gov.br/ccivil_03/_ato2015-2018/2017/lei/l13460.htm
25. https://www.planalto.gov.br/ccivil_03/_ato2015-2018/2018/lei/l13667.htm
26. https://www.planalto.gov.br/ccivil_03/_ato2019-2022/2020/lei/L14075.htm
27. https://www.planalto.gov.br/ccivil_03/leis/l8213cons.htm
28. https://www.planalto.gov.br/ccivil_03/leis/2003/l10.779.htm
29. https://www.planalto.gov.br/ccivil_03/_ato2023-2026/2025/mpv/mpv1323.htm
30. https://www.planalto.gov.br/ccivil_03/_ato2023-2026/2025/lei/l15265.htm
31. https://www.planalto.gov.br/ccivil_03/_ato2023-2026/2026/lei/l15399.htm
32. https://www.planalto.gov.br/ccivil_03/_ato2023-2026/2026/lei/l15455.htm
33. https://portal.tcu.gov.br/imprensa/noticias/inconsistencias-no-seguro-desemprego-causaram-prejuizo-a-administracao-publica
34. https://portal.tcu.gov.br/imprensa/noticias/fragilidades-na-transparencia-do-esocial-aumentam-risco-de-pagamentos-indevidos
35. https://portal.tcu.gov.br/imprensa/noticias/tribunal-avalia-servico-digital-de-seguro-desemprego-para-trabalhadores-formais
36. https://portal.tcu.gov.br/publicacoes-institucionais/sumarios-executivos/auditoria-seguro-desemprego-emprega-brasil
37. https://agenciagov.ebc.com.br/noticias/202512/facilita-brasil-governo-federal-lanca-novo-canal-digital-para-simplificar-servicos-a-trabalhadores-e-empresas
38. https://agenciagov.ebc.com.br/noticias/202607/saiba-como-acessar-os-canais-de-atendimento-do-ministerio-do-trabalho-e-emprego
39. https://jornalcontabil.com.br/noticia/seguro-desemprego-fgts-e-pis-tem-novas-datas-de-pagamento/ (secundária, 2018)

### 7. Questões em aberto para a sessão de mapeamento

1. **Escopo:** o mapa cobre só o trabalhador formal ou inclui doméstico, pescador e resgatado? O pescador tem cadeia própria (MPA, Fundacentro, biometria, INSS legado).
2. **URA como ator de IA:** sem evidência de reconhecimento de voz, a URA entra como "sistema automatizado (DTMF)" ou como "IA a confirmar"? Uma ligação de teste resolve.
3. **Fronteira da jornada telefônica:** o 158 do MTE é parte da jornada "URA da Caixa" (transbordo) ou uma jornada paralela? E os sistemas de retaguarda (motor de habilitação, CNIS, eSocial)?
4. **Fornecedor do call center:** ele entra como ator "R" (executa) mesmo sem identidade confirmada, ou só a Caixa como "A"?
5. **RACI de falhas compartilhadas:** quem é "A" quando a URA não resolve uma dúvida de concessão — a Caixa (canal) ou o MTE (conteúdo e Carta de Serviços)?
6. **Atores de controle e defesa (TCU, CGU, Senacon, Justiça):** entram no mapa como "I" ou ficam fora, numa camada de governança?
7. **Granularidade institucional:** MTE como bloco único ou desdobrado em Secretaria de Trabalho, Inspeção do Trabalho e central 158?
8. **Corte temporal:** o mapa representa novembro de 2026 ou mostra as transições de 2025–2026 (defeso, resgatado, Facilita)?
