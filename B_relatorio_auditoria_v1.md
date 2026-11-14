# B — Auditoria da v1 pelo assistente 2

> **Assistente 2:** Grok (xAI) — modelo distinto do assistente 1 (Claude).
> **Data:** 14/11/2026 · **Objeto:** `B_relatorio_assistente_v1.md` · **Prompt:** o de auditoria do tutorial (item B.2).
> Resposta colada na íntegra, sem edição.

## Auditoria v1

Encontrei 27 falhas na auditoria da pesquisa sobre a URA da Caixa. Na forma atual, ela não serve como mapa confiável da jornada em 2026. A maior parte das fontes oficiais existe e confere. Os erros graves estão em quatro pontos:

* trata o pescador como caso do INSS, mas a gestão passou ao MTE em 1º/11/2025;
* se apoia numa resolução do CODEFAT já revogada;
* lê errado alguns dados do TCU;
* deixa de fora atores e variantes relevantes.

F1. Erro factual (alta). "O requerimento é recebido e processado pelo INSS, não pelo MTE", e a tabela repete o "INSS | Processa o seguro-defeso".

* Isso valeu com a Lei 13.134/2015.
* A MP 1.323/2025, convertida na Lei 15.399/2026, passou a gestão ao MTE a partir de 1º/11/2025. Ao INSS ficaram só os defesos até 31/10/2025.
* Por isso, a inferência de transbordo ao INSS está errada.
* Fontes: [MTE, nov./2025](https://www.gov.br/trabalho-e-emprego/pt-br/noticias-e-conteudo/2025/novembro/seguro-defeso-passa-a-ser-administrado-pelo-ministerio-do-trabalho-e-emprego) e [Lei 15.399/2026](https://www.planalto.gov.br/ccivil_03/_ato2023-2026/2026/lei/l15399.htm).

F2. Fonte revogada (alta). "A Resolução CODEFAT 467/2005 é citada pelo gov.br como base do recurso", e a 957/2022 aparece como "[NÃO CONFIRMADO]".

* A Res. 957/2022 revogou a 467/2005 (art. 68, XLVII) e está em vigor desde 3/10/2022.
* É a norma geral do benefício, não só da habilitação automática. A própria página [gov.br Solicitar](https://www.gov.br/pt-br/servicos/solicitar-o-seguro-desemprego) a lista como legislação ([texto na LegisWeb](https://www.legisweb.com.br/legislacao/?id=436595)).

F3. Atribuição normativa errada (média). "Do 7º ao 120º dia [...] (Lei 7.998, art. 6º)". O art. 6º só diz "a partir do sétimo dia". O prazo de 120 dias vem de resolução do CODEFAT ([Lei 7.998](https://www.planalto.gov.br/ccivil_03/leis/l7998.htm)).

F4. Leitura errada do TCU (média). "Cerca de 4 mil recursos por ano". Segundo o [TCU 135/2024](https://portal.tcu.gov.br/imprensa/noticias/inconsistencias-no-seguro-desemprego-causaram-prejuizo-a-administracao-publica), são cerca de 4 mil por ano só nos casos que já tinham dois recursos indeferidos para o mesmo requerimento. Não é o total de recursos, e isso muda a escala do problema.

F5. Regra legal imprecisa (média). "6 meses a partir do 3º". A lei exige salário em cada um dos 6 meses imediatamente anteriores à dispensa. São meses seguidos, não seis meses quaisquer ([Lei 13.134](https://www.planalto.gov.br/ccivil_03/_ato2015-2018/2015/lei/l13134.htm)).

F6. Atribuição incorreta (média). "eSocial (gerido pelo Serpro)".

* Quem governa é um Comitê Gestor formado por RFB, área do Trabalho e INSS. Serpro e Dataprev dão apoio técnico ([Decreto 8.373/2014](https://www.planalto.gov.br/ccivil_03/_ato2011-2014/2014/decreto/d8373.htm) e [Portaria 300/2019](https://www.gov.br/esocial/pt-br/centrais-de-conteudo/legislacao/empresas/portaria-300_textoconsolidado.pdf)).
* A RFB, como ator, ficou de fora.

F7. Fonte fraca e inferência (média). "Lei 14.075/2020 autoriza [...] inclusive o seguro-desemprego [...] CAIXA Tem", com a FAQ da Caixa como fonte.

* A lei não cita seguro-desemprego, Caixa nem CAIXA Tem. O benefício só entra por inferência, via art. 3º, V.
* A lei veio da MP 982/2020 e remete ao CMN e ao Banco Central. A fonte certa é a [própria lei](https://www.planalto.gov.br/ccivil_03/_ato2019-2022/2020/lei/L14075.htm).

F8. Atribuição normativa (baixa). "A Caixa só paga como agente pagador (Lei 7.998, art. 15)". O art. 15 fala em "Bancos Oficiais Federais" e não nomeia a Caixa. O papel dela vem de norma do CODEFAT e de contrato. CONFERIR NA FONTE.

F9. Âncora normativa errada (média). O texto usa a Portaria MTE 1.889/2025 como base do papel LGPD de MTE e Dataprev.

* A portaria só autoriza a Dataprev a repassar à Telebrás dados de pescadores de certos municípios.
* Ela não serve para o seguro-desemprego formal. A Telebrás, aliás, seria um ator da variante pescador ([Portaria](https://www.gov.br/trabalho-e-emprego/pt-br/acesso-a-informacao/tratamento-de-dados-pessoais/PORTARIAMTEN1.889DE7DENOVEMBRODE2025.pdf)).

F10. Canais imprecisos (baixa). "Portal de Serviços da Dataprev [...] presencialmente em SRTE ou Sine, com agendamento".

* Não há fonte para dizer que o portal é "da Dataprev". O TCU fala em Portal Emprega Brasil, do MTE.
* O presencial é subsidiário e é agendado pela Facilita.
* O Sine é rede estadual e municipal.

F11. Fonte atribuída errado (baixa). O texto atribui o Fala.BR à página gov.br Solicitar, mas ela não o menciona. Quem menciona é a [Agência Gov de julho de 2026](https://agenciagov.ebc.com.br/noticias/202607/saiba-como-acessar-os-canais-de-atendimento-do-ministerio-do-trabalho-e-emprego).

F12. Leitura forçada do TCU (baixa). "Determina a integração ao eSocial em 180 dias". O TCU determinou que, em 180 dias, o MTE "tome medidas para integrar". É prazo para agir, não para concluir ([TCU 1621/2026](https://portal.tcu.gov.br/imprensa/noticias/tribunal-avalia-servico-digital-de-seguro-desemprego-para-trabalhadores-formais)).

F13. Leitura forçada do TCU (baixa). "A Dataprev não forneceu dados completos". O TCU fala em problemas operacionais que impediram o acesso e mandou dar acesso ao DataLake em 10 dias. A frase sugere uma recusa que a fonte não sustenta ([TCU 1114/2025](https://portal.tcu.gov.br/imprensa/noticias/fragilidades-na-transparencia-do-esocial-aumentam-risco-de-pagamentos-indevidos)).

F14. Generalização (baixa). O texto fala em "pagamentos indevidos (> 300 mil solicitações...)". Na fonte, são "possíveis" pagamentos indevidos e "indícios" de R$ 147 mi. O texto omite os R$ 544 mil de fraudes presumidas e o exame dos pagamentos por ordem judicial.

F15. Variante incompleta (média). No doméstico faltam o limite de 3 parcelas e o prazo próprio, do 7º ao 90º dia. A [LC 150](https://www.planalto.gov.br/ccivil_03/leis/lcp/lcp150.htm) (arts. 26 e 29) nem é citada.

F16. Variantes omitidas (média).

* O trabalhador resgatado (art. 2º-C) recebe 3 parcelas de 1 salário mínimo, e a Auditoria-Fiscal do Trabalho entra como ator.
* A bolsa qualificação (arts. 2º-A e 3º-A) também ficou de fora.
* As duas têm regras próprias na Res. 957.

F17. Ator omitido (média). O próprio TCU 135/2024 trata de pagamentos por ordem judicial. A via judicial, com Justiça Federal, AGU e DPU, é uma saída real da jornada e não aparece na tabela.

F18. Ator omitido e inferência fraca (média). "O cruzamento com o CNIS é presumido". O art. 3º, V exige que o trabalhador não receba benefício previdenciário. O TCU declarou ilegal a acumulação com pensão por morte e com auxílio-reclusão. Então o INSS e as bases de benefícios são atores da jornada formal, não uma hipótese.

F19. Ator omitido (baixa). O texto cita "login gov.br Prata/Ouro", mas o provedor de identidade (gov.br, da SGD/MGI) não está na tabela. A Lei 15.399, art. 7º, ainda traz uma transição de autenticação para os pescadores.

F20. Atores regulatórios omitidos (baixa).

* Banco Central e CMN, que regulam a Poupança Social Digital e as regras de SAC e ouvidoria (CONFERIR NA FONTE).
* Senacon, dona do consumidor.gov.br.
* ANPD, por causa da LGPD.
* As entidades de pesca, na variante pescador (Lei 15.399, § 12).

F21. Classificação sem base (baixa). "URA eletrônica | IA-sistema". A própria pesquisa admite que não sabe se a URA usa reconhecimento de fala ou só teclas. O mesmo problema vale para os apps e para o motor de regras.

F22. Afirmação sem leitura da fonte (baixa).

* A "opção 9 seguida de 1" entrou no texto sem que a fonte fosse lida.
* O [Jornal Contábil de 2018](https://jornalcontabil.com.br/noticia/seguro-desemprego-fgts-e-pis-tem-novas-datas-de-pagamento/) confirma a opção 5, o NIS e a identificação positiva. Mas ele reproduz um comunicado da Caixa, que é a fonte primária a buscar.
* A consulta da conta de crédito só vale para crédito em conta Caixa.

F23. Horários sem base sólida (baixa). No [Portal Cidadão da Caixa](https://cidadao.caixa.gov.br/frontpage), os horários de 8h às 21h e de 10h às 16h aparecem no bloco da Central 111. Só sites secundários os ligam ao 0800 726 0207. Não há fonte para o WhatsApp "24h", e um site secundário fala em 8h às 18h. CONFERIR NA FONTE.

F24. Risco superestimado (baixa). O prazo de 67 dias confere. Mas a parcela pode ser reemitida pelo app ou pelo 158 (Res. 957), e quem cuida da reemissão é o MTE, não a Caixa.

F25. Datas mal situadas (baixa).

* A Facilita já tinha 238 mil atendimentos "em dois meses" em 18/12/2025. Então essa data foi o lançamento oficial, não o início do serviço.
* A Celeste já aparece em dez./2025.
* No trecho que li da matéria de julho, as SRTE não aparecem.

F26. Incerteza que dava para resolver (baixa). O art. 15 vigente é o original, porque a redação da MP 905 caducou. O art. 23 vigente vem da Lei 14.261/2021, e o Planalto grafa "10.261" por erro.

F27. Imprecisão normativa (baixa). A Lei 13.460 não "cria" ouvidorias, ela disciplina as atribuições delas. E ela também se aplica à Caixa, como empresa pública, não só ao MTE. CONFERIR NA FONTE os artigos.

O que não consegui verificar (CONFERIR NA FONTE):

* As páginas da Caixa (FAQ, Atendimento e WhatsApp). Elas redirecionaram ou estouraram o tempo, então esses pontos ficaram só com corroboração secundária.
* Os artigos exatos da Res. 957 sobre os 120 dias, os 67 dias e a ordem de pagamento.
* A íntegra dos três acórdãos do TCU.
* O fim da matéria da Agência Gov de julho de 2026.
* A composição atual do Comitê Gestor do eSocial.
