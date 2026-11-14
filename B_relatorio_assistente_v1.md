# B — Relatório do assistente 1 (v1)

> Assistente 1: Claude (Anthropic, Claude Opus 5.5) com busca web · gerado em 13/11/2026 a partir do prompt do Apêndice de A_meta_prompt.md

## v1

### 1. Sumário executivo

- A jornada "Seguro-Desemprego pela URA da Caixa" é, na verdade, uma jornada **bifurcada**: o MTE habilita e concede o benefício (com sistemas operados pela Dataprev), e a Caixa só **paga** como agente pagador, com recursos do FAT ([Caixa – Seguro-Desemprego](https://www.caixa.gov.br/beneficios-trabalhador/seguro-desemprego/Paginas/default.aspx); [Lei 7.998/1990, art. 15](https://www.planalto.gov.br/ccivil_03/leis/l7998.htm)).
- O 0800 726 0207 ("Atendimento CAIXA Cidadão") atende PIS, Benefícios Sociais, FGTS e Cartão Social. Tem URA eletrônica 24h e atendimento humano de segunda a sexta, das 8h às 21h, e aos sábados, das 10h às 16h ([Caixa – Atendimento](https://www.caixa.gov.br/atendimento/Paginas/default.aspx)).
- A própria Caixa remete dúvidas sobre **concessão e valor** aos canais do MTE (app Carteira de Trabalho Digital, gov.br, central 158) ([FAQ Caixa](https://www.caixa.gov.br/beneficios-trabalhador/seguro-desemprego/perguntas-frequentes/Paginas/default.aspx)). Por isso, a URA resolve sobretudo dúvidas de **pagamento** e transborda o resto.
- O TCU apontou falhas estruturais nos Acórdãos 135/2024, 1114/2025 e 1621/2026 (seção 4).
- Não encontrei fonte primária sobre os menus atuais da URA, o fornecedor de URA ou de reconhecimento de fala, nem o operador do 158 (seção 5).

### 2. Linha do tempo da jornada

**2.1 Marcos normativos e institucionais (2015–2026)**

| Data | Marco | Fonte |
|---|---|---|
| 2015 | Lei 13.134/2015 altera a Lei 7.998/1990. A carência passa a ser escalonada: 12 meses nos últimos 18 no 1º pedido, 9 meses nos últimos 12 no 2º e 6 meses a partir do 3º. As parcelas vão de 3 a 5, o CODEFAT pode prolongar o benefício e o pedido do pescador passa a ser processado pelo INSS. | [planalto – L13134](https://www.planalto.gov.br/ccivil_03/_ato2015-2018/2015/lei/l13134.htm) |
| 2017 | Lei 13.460/2017 (Código de Defesa do Usuário de Serviços Públicos) cria ouvidorias, Carta de Serviços e conselhos de usuários (arts. 7º, 13 a 22). | [planalto – L13460](https://www.planalto.gov.br/ccivil_03/_ato2015-2018/2017/lei/l13460.htm) |
| 2020 | Lei 14.075/2020 autoriza o pagamento de benefícios sociais, inclusive o seguro-desemprego, em Poupança Social Digital movimentada pelo app CAIXA Tem. | [FAQ Caixa](https://www.caixa.gov.br/beneficios-trabalhador/seguro-desemprego/perguntas-frequentes/Paginas/default.aspx) |
| 31/01/2024 | Acórdão 135/2024-Plenário (TC 006.464/2022-0) aponta inconsistências em mais de 300 mil solicitações (2018 a jun./2022), falhas de governança na relação entre a Secretaria do Trabalho e a Dataprev e cerca de 4 mil recursos por ano. | [TCU – notícia](https://portal.tcu.gov.br/imprensa/noticias/inconsistencias-no-seguro-desemprego-causaram-prejuizo-a-administracao-publica) |
| 21/05/2025 | Acórdão 1114/2025-Plenário (TC 008.443/2024-6) trata da integridade dos dados do eSocial usados no seguro-desemprego e no abono. A Dataprev converte o eSocial numa base intermediária ("eSocial Negócio"). | [TCU – notícia](https://portal.tcu.gov.br/imprensa/noticias/fragilidades-na-transparencia-do-esocial-aumentam-risco-de-pagamentos-indevidos) |
| 18/12/2025 | O MTE lança a Plataforma Facilita (Facilita Brasil), desenvolvida pela Dataprev, que reúne seguro-desemprego, abono, CTPS Digital e outros serviços. | [Agência Gov](https://agenciagov.ebc.com.br/noticias/202512/facilita-brasil-governo-federal-lanca-novo-canal-digital-para-simplificar-servicos-a-trabalhadores-e-empresas) |
| 24/06/2026 | Acórdão 1621/2026-Plenário (TC 015.553/2025-6) avalia o serviço digital. Aponta sistemas paralelos (Empregador Web × eSocial), falhas de atendimento, recursos lentos e ausência de base de conhecimento única. Determina a integração ao eSocial em 180 dias. | [TCU – notícia](https://portal.tcu.gov.br/imprensa/noticias/tribunal-avalia-servico-digital-de-seguro-desemprego-para-trabalhadores-formais); [TCU – sumário](https://portal.tcu.gov.br/publicacoes-institucionais/sumarios-executivos/auditoria-seguro-desemprego-emprega-brasil) |
| jul./2026 | O MTE divulga seus canais: 158, Facilita, a assistente virtual "Celeste" e as SRTE. | [Agência Gov](https://agenciagov.ebc.com.br/noticias/202607/saiba-como-acessar-os-canais-de-atendimento-do-ministerio-do-trabalho-e-emprego) |

**2.2 Jornada do cidadão (trabalhador formal)**

1. **Dispensa.** O empregador entrega o Requerimento do Seguro-Desemprego e informa o desligamento pelo eSocial ou pelo Empregador Web ([gov.br – Solicitar](https://www.gov.br/pt-br/servicos/solicitar-o-seguro-desemprego); [TCU 1621/2026](https://portal.tcu.gov.br/imprensa/noticias/tribunal-avalia-servico-digital-de-seguro-desemprego-para-trabalhadores-formais)).
2. **Requerimento**, do 7º ao 120º dia após a dispensa. Pode ser feito pelo gov.br ou pelo Portal de Serviços da Dataprev, pelo app Carteira de Trabalho Digital, pelo 158 ou presencialmente em SRTE ou Sine, com agendamento ([gov.br – Solicitar](https://www.gov.br/pt-br/servicos/solicitar-o-seguro-desemprego); [Lei 7.998, art. 6º](https://www.planalto.gov.br/ccivil_03/leis/l7998.htm)). **A URA da Caixa não recebe requerimentos** [INFERÊNCIA a partir da lista oficial de canais de requerimento, que não inclui a Caixa — [FAQ Caixa](https://www.caixa.gov.br/beneficios-trabalhador/seguro-desemprego/perguntas-frequentes/Paginas/default.aspx)].
3. **Habilitação.** O sistema do MTE, operado pela Dataprev, verifica automaticamente os critérios com base nos dados do empregador e de outras bases. Havendo impedimento, o trabalhador é notificado e pode recorrer em 120 dias ([gov.br – Recurso](https://www.gov.br/pt-br/servicos/cadastrar-recurso-relativo-ao-seguro-desemprego)). A habilitação automática estaria prevista na Resolução CODEFAT 957/2022 [NÃO CONFIRMADO — li só a descrição em resultado de busca; o texto integral não estava acessível].
4. **Liberação e pagamento.** A 1ª parcela sai cerca de 30 dias após o requerimento, e as demais a cada 30 dias. O pagamento segue esta ordem: (a) conta indicada; (b) poupança CAIXA; (c) Poupança Social Digital (CAIXA Tem); (d) terminais, lotéricas e correspondentes, com Cartão Social e senha ou biometria; (e) agência, com documento ([gov.br – Solicitar](https://www.gov.br/pt-br/servicos/solicitar-o-seguro-desemprego); [FAQ Caixa](https://www.caixa.gov.br/beneficios-trabalhador/seguro-desemprego/perguntas-frequentes/Paginas/default.aspx)). A parcela não sacada em **67 dias volta ao FAT** (FAQ Caixa).
5. **Chamada à URA (0800 726 0207).**
   - (a) **Entrada:** URA eletrônica 24h, sobre PIS, Benefícios Sociais, FGTS e Cartão Social ([Caixa – Atendimento](https://www.caixa.gov.br/atendimento/Paginas/default.aspx)).
   - (b) **Menu:** a "opção 5" para seguro-desemprego foi relatada em 2018 ([Jornal Contábil, 2018](https://jornalcontabil.com.br/noticia/seguro-desemprego-fgts-e-pis-tem-novas-datas-de-pagamento/)) [NÃO CONFIRMADO para 2026]. Guias de terceiros descrevem a opção 5 para Cartão Social e senha e a opção 9 seguida de 1 para atendente [NÃO CONFIRMADO; a fonte de terceiros não pôde ser lida, apenas o resumo da busca].
   - (c) **Autenticação:** NIS e "identificação positiva" com dados cadastrais ([Jornal Contábil, 2018](https://jornalcontabil.com.br/noticia/seguro-desemprego-fgts-e-pis-tem-novas-datas-de-pagamento/)) [NÃO CONFIRMADO para 2026].
   - (d) **Consulta:** se a parcela foi liberada, agendada ou paga, a data da próxima parcela e a conta de crédito (mesma fonte) [NÃO CONFIRMADO para 2026].
   - (e) **Transbordo:** para um atendente humano, no horário de atendimento humano; ou para fora da Caixa, quando a dúvida é de concessão ou valor, que vai ao MTE (FAQ Caixa).
   - (f) **Encerramento:** resposta, ou encaminhamento a app Caixa, agência, 158/gov.br ou SRTE/Sine. Pesquisa de satisfação: [NÃO CONFIRMADO].
6. **Pós-atendimento.** Reclamação no SAC Caixa (0800 726 0101), na Ouvidoria Caixa (0800 725 7474) ou no consumidor.gov.br, para o lado bancário ([Caixa – Atendimento](https://www.caixa.gov.br/atendimento/Paginas/default.aspx)); ou no Fala.BR/CGU, para o lado do MTE ([gov.br – Solicitar](https://www.gov.br/pt-br/servicos/solicitar-o-seguro-desemprego)). Recurso administrativo ao MTE em 120 dias ([gov.br – Recurso](https://www.gov.br/pt-br/servicos/cadastrar-recurso-relativo-ao-seguro-desemprego)).

**Variações que mudam a jornada telefônica:**

- **Doméstico:** usa o mesmo fluxo de recurso (modalidade "Doméstico") e recebe valor de 1 salário mínimo ([gov.br – Recurso](https://www.gov.br/pt-br/servicos/cadastrar-recurso-relativo-ao-seguro-desemprego); [FAQ Caixa](https://www.caixa.gov.br/beneficios-trabalhador/seguro-desemprego/perguntas-frequentes/Paginas/default.aspx)). Os canais próprios de requerimento não foram confirmados: a página gov.br específica retornou 404.
- **Pescador artesanal (defeso):** o requerimento é recebido e processado pelo **INSS**, não pelo MTE ([L13134](https://www.planalto.gov.br/ccivil_03/_ato2015-2018/2015/lei/l13134.htm)). Assim, a dúvida de concessão é transbordada ao INSS, e não ao 158 [INFERÊNCIA].

### 3. Tabela de atores

| Ator | Tipo (humano / IA-sistema / institucional) | Papel | Entra na jornada | Sai da jornada | Fonte (URL) |
|---|---|---|---|---|---|
| Trabalhador formal requerente | humano | Requer, consulta, saca e recorre | Na dispensa | No saque da última parcela ou no indeferimento/recurso | https://www.gov.br/pt-br/servicos/solicitar-o-seguro-desemprego |
| Empregador | humano/institucional | Entrega o requerimento e informa o desligamento (eSocial/Empregador Web) | Na dispensa | Após o envio dos dados (volta se houver divergência) | https://portal.tcu.gov.br/imprensa/noticias/tribunal-avalia-servico-digital-de-seguro-desemprego-para-trabalhadores-formais |
| Ministério do Trabalho e Emprego (MTE) | institucional | Responsável pelo serviço; habilita, concede, define o valor e analisa recursos; fiscaliza o programa (art. 23) | No requerimento | Na concessão/indeferimento ou na decisão do recurso | https://www.gov.br/pt-br/servicos/solicitar-o-seguro-desemprego ; https://www.planalto.gov.br/ccivil_03/leis/l7998.htm |
| Caixa Econômica Federal | institucional | Agente pagador com recursos do FAT; opera a URA 0800 726 0207, os apps e a rede de pagamento | Na liberação da parcela / ligação | No pagamento ou no transbordo ao MTE | https://www.caixa.gov.br/beneficios-trabalhador/seguro-desemprego/Paginas/default.aspx |
| Atendente humano da Caixa (CAIXA Cidadão) | humano | Atende o transbordo da URA (seg.–sex. 8h–21h; sáb. 10h–16h) | No transbordo da URA | Ao encerrar ou encaminhar | https://www.caixa.gov.br/atendimento/Paginas/default.aspx |
| URA eletrônica 0800 726 0207 | IA-sistema | Autoatendimento 24h: menus, identificação, consulta de parcela | Na ligação | No encerramento ou transbordo | https://www.caixa.gov.br/atendimento/Paginas/default.aspx |
| Assistente virtual WhatsApp Caixa (0800 104 0104) | IA-sistema | Chatbot 24h para produtos e serviços (escopo para seguro-desemprego: [NÃO CONFIRMADO]) | Canal alternativo | Ao responder ou encaminhar | https://www.caixa.gov.br/atendimento/canais-digitais/whatsapp/Paginas/default.aspx |
| Apps CAIXA Tem / Benefícios Sociais CAIXA | IA-sistema | Consulta da parcela e movimentação da Poupança Social Digital | Após a liberação | No saque/transferência | https://www.caixa.gov.br/beneficios-trabalhador/seguro-desemprego/perguntas-frequentes/Paginas/default.aspx |
| Rede de lotéricas, correspondentes CAIXA Aqui e terminais (com biometria) | humano + sistema | Saque com Cartão Social e senha ou biometria | No saque | Após o saque | https://www.caixa.gov.br/beneficios-trabalhador/seguro-desemprego/perguntas-frequentes/Paginas/default.aspx |
| Dataprev | institucional | Contratada do MTE; opera os sistemas do seguro-desemprego, o Portal de Serviços e a base "eSocial Negócio"; desenvolveu a Facilita | No requerimento (processamento) | Na emissão do lote de pagamento [INFERÊNCIA] | https://portal.tcu.gov.br/imprensa/noticias/inconsistencias-no-seguro-desemprego-causaram-prejuizo-a-administracao-publica ; https://portal.tcu.gov.br/imprensa/noticias/fragilidades-na-transparencia-do-esocial-aumentam-risco-de-pagamentos-indevidos |
| Motor de regras de habilitação (sistema do Seguro-Desemprego) | IA-sistema | Verificação automática de requisitos e geração de notificações/impedimentos | Após o requerimento | Na habilitação ou notificação | https://www.gov.br/pt-br/servicos/cadastrar-recurso-relativo-ao-seguro-desemprego (verificação automática: [NÃO CONFIRMADO] via Res. CODEFAT 957/2022) |
| eSocial (gerido pelo Serpro) / base "eSocial Negócio" | IA-sistema | Fonte dos vínculos e salários usados na habilitação | Na dispensa | Na habilitação | https://portal.tcu.gov.br/imprensa/noticias/fragilidades-na-transparencia-do-esocial-aumentam-risco-de-pagamentos-indevidos |
| Empregador Web | IA-sistema | Sistema paralelo de envio do requerimento pelo empregador (duplica o eSocial) | Na dispensa | Na habilitação | https://portal.tcu.gov.br/imprensa/noticias/tribunal-avalia-servico-digital-de-seguro-desemprego-para-trabalhadores-formais |
| App Carteira de Trabalho Digital / gov.br | IA-sistema | Requerimento, acompanhamento e recurso; login gov.br Prata/Ouro para recurso | No requerimento | No acompanhamento final | https://www.gov.br/pt-br/servicos/cadastrar-recurso-relativo-ao-seguro-desemprego |
| Central Alô Trabalho 158 (MTE) | humano + sistema | Orientação, requerimento por telefone e agendamento presencial | No transbordo da Caixa | Ao orientar ou agendar | https://www.gov.br/pt-br/servicos/solicitar-o-seguro-desemprego |
| Assistente virtual "Celeste" (MTE) | IA-sistema | Orientações sobre serviços do MTE (uso de IA: [NÃO CONFIRMADO]) | Canal alternativo | Ao orientar | https://agenciagov.ebc.com.br/noticias/202607/saiba-como-acessar-os-canais-de-atendimento-do-ministerio-do-trabalho-e-emprego |
| Plataforma Facilita (MTE/Dataprev) | IA-sistema | Atendimento remoto: documentos, agendamento e pendências | Em pendência ou divergência | Na resolução | https://agenciagov.ebc.com.br/noticias/202512/facilita-brasil-governo-federal-lanca-novo-canal-digital-para-simplificar-servicos-a-trabalhadores-e-empresas |
| SRTE e atendentes do Sine | humano/institucional | Atendimento presencial, requerimento e recurso; uso dos sistemas internos | Por agendamento | Ao concluir o atendimento | https://www.gov.br/pt-br/servicos/cadastrar-recurso-relativo-ao-seguro-desemprego |
| CODEFAT / FAT | institucional | Gere o FAT; define e prorroga parcelas; regulamenta (Res. 467/2005 citada pelo gov.br) | Fora do fluxo (normatiza e financia) | — | https://www.planalto.gov.br/ccivil_03/leis/l7998.htm |
| INSS | institucional | Processa o seguro-defeso do pescador artesanal | Só na variante pescador | — | https://www.planalto.gov.br/ccivil_03/_ato2015-2018/2015/lei/l13134.htm |
| TCU | institucional | Controle externo e auditorias (Acórdãos 135/2024, 1114/2025 e 1621/2026) | Fora do fluxo | — | https://portal.tcu.gov.br/imprensa/noticias/tribunal-avalia-servico-digital-de-seguro-desemprego-para-trabalhadores-formais |
| CGU / Fala.BR | institucional | Recebe manifestações sobre o serviço do MTE | Após falha | Na resposta | https://www.gov.br/pt-br/servicos/solicitar-o-seguro-desemprego |
| SAC e Ouvidoria Caixa; consumidor.gov.br | institucional | Reclamações sobre o lado bancário e o atendimento Caixa | Após falha | Na resposta | https://www.caixa.gov.br/atendimento/Paginas/default.aspx |
| Intérprete de Libras (parceiro Caixa) | humano | Atendimento acessível | Sob demanda | Ao fim | https://www.caixa.gov.br/atendimento/Paginas/default.aspx |

### 4. Pontos de falha e responsáveis

| # | Falha | Evidência | Quem responde |
|---|---|---|---|
| F1 | **Pergunta errada no canal errado.** O cidadão liga para a Caixa com dúvida de concessão ou valor, mas a Caixa só informa pagamento. | FAQ Caixa remete ao MTE ([link](https://www.caixa.gov.br/beneficios-trabalhador/seguro-desemprego/perguntas-frequentes/Paginas/default.aspx)) | MTE (Carta de Serviços, art. 7º da Lei 13.460/2017) e Caixa (script de transbordo). Ausência de "transferência quente" entre 0800 e 158: [INFERÊNCIA] |
| F2 | **Duplicidade de dados** do empregador (Empregador Web × eSocial), que gera bloqueios, indeferimentos e recursos | [TCU 1621/2026](https://portal.tcu.gov.br/imprensa/noticias/tribunal-avalia-servico-digital-de-seguro-desemprego-para-trabalhadores-formais) | MTE (prazo de 180 dias para integrar ao eSocial); empregador (qualidade do dado) |
| F3 | **Base de dados inconsistente** e pagamentos indevidos (> 300 mil solicitações; indícios de R$ 147 mi a servidores de entes subnacionais) | [TCU 135/2024](https://portal.tcu.gov.br/imprensa/noticias/inconsistencias-no-seguro-desemprego-causaram-prejuizo-a-administracao-publica) | MTE (governança contratual) e Dataprev (execução) |
| F4 | **Recursos lentos e repetitivos**: cerca de 4 mil por ano, um requerimento analisado 15 vezes, sem 2ª instância | TCU 135/2024; TCU 1621/2026 | MTE |
| F5 | **Falta de base de conhecimento única**: respostas diferentes e encaminhamentos sucessivos, inclusive no Sine | TCU 1621/2026 | MTE (e, por extensão, atendentes Caixa sem acesso à base do MTE [INFERÊNCIA]) |
| F6 | **Opacidade do eSocial para o controle**: a Dataprev não forneceu dados completos ao TCU | [TCU 1114/2025](https://portal.tcu.gov.br/imprensa/noticias/fragilidades-na-transparencia-do-esocial-aumentam-risco-de-pagamentos-indevidos) | MTE e Dataprev |
| F7 | **Parcela não sacada em 67 dias volta ao FAT**: risco para quem não consegue o cartão, a senha ou a biometria | FAQ Caixa | Caixa (meios de pagamento); MTE/CODEFAT (regra) |
| F8 | **Horário humano limitado; menus descritos por terceiros desatualizados** | Caixa – Atendimento; Jornal Contábil (2018) | Caixa |
| F9 | **Golpes por mensagem** (Caixa avisa que não pede senhas) | WhatsApp Caixa | Caixa; cidadão |

### 5. Lacunas, incertezas e inferências

- **[LACUNA]** Não encontrei fonte primária com a **árvore de menus vigente** da URA 0800 726 0207. A descrição da seção 2.2 vem de matéria de 2018 [NÃO CONFIRMADO para 2026]. Recomenda-se uma ligação de teste documentada (observação direta).
- **[LACUNA]** Não identifiquei se a URA usa **reconhecimento de fala (ASR/NLU)** ou só DTMF, nem o **fornecedor ou operador** do call center Caixa (contratos não pesquisados nesta v1).
- **[LACUNA]** O operador da central 158 (próprio ou terceirizado) não foi identificado.
- **[NÃO CONFIRMADO]** A Resolução CODEFAT 957/2022 como base da habilitação automática: o texto integral retornou 403. A Resolução CODEFAT 467/2005 é citada pelo gov.br como base do recurso.
- **[NÃO CONFIRMADO]** O conteúdo da Portaria MTE 1.889/2025 (tratamento de dados pela Dataprev): o PDF não foi legível. Por isso, o papel formal de controlador (MTE) e operador (Dataprev) segundo a LGPD é **[INFERÊNCIA]**.
- **[INFERÊNCIA]** O cruzamento com o **CNIS** e bases previdenciárias (necessário pelo art. 3º da Lei 7.998) é presumido. A acumulação ilegal apontada pelo TCU 135/2024 sugere cruzamento falho, mas não achei documento primário com as bases consultadas.
- **[INFERÊNCIA]** A Caixa recebe da Dataprev/MTE um lote de parcelas liberadas. O fluxo técnico Dataprev→Caixa não foi documentado em fonte lida.
- **[INCERTEZA]** O papel do WhatsApp Caixa e da "Celeste" no seguro-desemprego e o uso de IA generativa nesses canais não estão descritos nas páginas oficiais lidas.
- **[INCERTEZA]** A Lei 7.998 compilada exibe várias redações dos arts. 15 e 23.
- **[LACUNA]** Não verifiquei Banco Central, Procons, DPU ou MPF. Não li a íntegra dos acórdãos, só as notícias e o sumário do TCU.

### 6. Lista de fontes consultadas

1. Caixa – Seguro-Desemprego (agente pagador/FAT): https://www.caixa.gov.br/beneficios-trabalhador/seguro-desemprego/Paginas/default.aspx
2. Caixa – Perguntas frequentes do Seguro-Desemprego: https://www.caixa.gov.br/beneficios-trabalhador/seguro-desemprego/perguntas-frequentes/Paginas/default.aspx
3. Caixa – Atendimento (0800 726 0207, SAC, Ouvidoria, Libras): https://www.caixa.gov.br/atendimento/Paginas/default.aspx
4. Caixa – WhatsApp: https://www.caixa.gov.br/atendimento/canais-digitais/whatsapp/Paginas/default.aspx
5. gov.br – Solicitar o Seguro-Desemprego: https://www.gov.br/pt-br/servicos/solicitar-o-seguro-desemprego
6. gov.br – Cadastrar recurso relativo ao Seguro-Desemprego: https://www.gov.br/pt-br/servicos/cadastrar-recurso-relativo-ao-seguro-desemprego
7. Lei 7.998/1990: https://www.planalto.gov.br/ccivil_03/leis/l7998.htm
8. Lei 13.134/2015: https://www.planalto.gov.br/ccivil_03/_ato2015-2018/2015/lei/l13134.htm
9. Lei 13.460/2017: https://www.planalto.gov.br/ccivil_03/_ato2015-2018/2017/lei/l13460.htm
10. TCU – Acórdão 135/2024 (notícia): https://portal.tcu.gov.br/imprensa/noticias/inconsistencias-no-seguro-desemprego-causaram-prejuizo-a-administracao-publica
11. TCU – Acórdão 1114/2025 (notícia): https://portal.tcu.gov.br/imprensa/noticias/fragilidades-na-transparencia-do-esocial-aumentam-risco-de-pagamentos-indevidos
12. TCU – Acórdão 1621/2026 (notícia): https://portal.tcu.gov.br/imprensa/noticias/tribunal-avalia-servico-digital-de-seguro-desemprego-para-trabalhadores-formais
13. TCU – Sumário executivo, auditoria Seguro-Desemprego/Emprega Brasil: https://portal.tcu.gov.br/publicacoes-institucionais/sumarios-executivos/auditoria-seguro-desemprego-emprega-brasil
14. Agência Gov – Facilita Brasil (dez./2025): https://agenciagov.ebc.com.br/noticias/202512/facilita-brasil-governo-federal-lanca-novo-canal-digital-para-simplificar-servicos-a-trabalhadores-e-empresas
15. Agência Gov – Canais de atendimento do MTE (jul./2026): https://agenciagov.ebc.com.br/noticias/202607/saiba-como-acessar-os-canais-de-atendimento-do-ministerio-do-trabalho-e-emprego
16. Jornal Contábil (secundária, 2018) – menu do 0800 726 0207: https://jornalcontabil.com.br/noticia/seguro-desemprego-fgts-e-pis-tem-novas-datas-de-pagamento/

*Sem acesso (não usadas): Res. CODEFAT 957/2022, Portaria MTE 1.889/2025, página gov.br do doméstico e guia Tecnoblog.*
