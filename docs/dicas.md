## Como limpar memória local do navegador (cache do browser) 

Acesse, no navegador, o ícone que fica no canto superior direito que contém três tracinhos horizontais 
Selecione Preferências 
Selecione o painel Privacidade e Segurança. 
Na seção "Histórico", tem um botão "Limpar histórico" 
Acione o botão e selecione a opção "tudo" com a marcação "cache", em seguida confirmando a limpeza. 
Atualize a página do PJe. 
Segue o sítio que contém essas orientações que passei sobre a limpeza do histórico: 
https://support.mozilla.org/pt-BR/kb/como-limpar-cache-firefox 

## Distribuição de processos em caixas de procuradores 

O PJe do primeiro grau tem uma funcionalidade que, ao ser protocolado novo processo, os filtros cadastrados nas caixas de advogados e procuradores são automaticamente acionados de forma a preencher as caixas com os processos respectivos. O acionamento se dá no protocolo de novos processos e na construção de atos de comunicação e na redistribuição. 

 

Em versões anteriores à 2.1.2.6.17, quando o processo é remetido a outra zona, se não há mudança de UF, o número do processo permanece o mesmo. Para o sistema, o que ocorreu não foi um novo protocolo. Os filtros não são acionados automaticamente nesses casos. Para eles, o procurador gestor deve utilizar a distribuição disponível por meio do ícone de seu painel, uma varinha, como se fosse de mágica, que coloca cada processo na caixa respectiva. 

 

O painel do procurador tem jurisdições, onde ele pode protocolar processos e acompanhar processos onde é parte/foi intimado, e pode ter caixas ou não. Em geral, as caixas que já existem hoje são caixas cujos nomes são os nomes das zonas, mas o procurador gestor pode ter apagado essas caixas, mudado de nome... Só há como ter certeza se consultar pelo log. Não se cria caixa dentro de caixa. Sendo assim, se ele foi criar uma outra caixa, serão exibidas todas as caixas para o gestor. A caixa não fica dentro de uma zona, mas o nome das caixas iniciais que criamos coincide com o nome da zona. 

 

O procurador gestor é responsável pela gestão de suas caixas. Se ele vir que alguém tem que ter acesso a apenas um processo, ele mesmo pode criar uma caixa nova e colocar esse outro promotor nessa caixa nova e ele mesmo pode mover o processo da caixa geral para essa caixa nova. Ele também pode criar filtros de forma a tentar distribuir os processos em caixas e apagar a caixa que criamos para cada zona. As caixas que criamos é uma sugestão de organização, apenas. Mas a gestão é toda do procurador gestor. 

## Documentos não lidos 

O PJe tem um controle bem antigo para sinalizar ao servidor que documentos novos foram incluídos pelo usuário externo. A possibilidade de se iniciar fluxo de petição avulsa nem sempre existiu e o controle era feito anteriormente por essa opção. 

Esse controle é só um aviso, ele não impede o usuário de ver o documento. 

Para que o aviso não seja mais exibido, o usuário sinaliza que já viu o documento, mas não significa que ele efetivamente foi visto. Pode-se marcar que o documento foi lido sem nem ter aberto o documento. A marcação significa que o usuário quer que o aviso desapareça. Se o usuário abrir o documento, mas não marcar que já viu, o sistema vai continuar exibindo que há documentos não lidos. 

Esse aviso era exibido apenas por meio de um agrupador, que não utilizamos muito na justiça eleitoral, já que são muito onerosos para a performance. Todos os agrupadores são muito onerosos. 

Outros tribunais utilizam bastante e queriam que o aviso aparecesse nos autos do processo. 

Por isso apareceu essa novidade, a partir da versão 2.1.2.6. 

Quando entrou em produção, como nunca utilizamos, todos os processos com documentos protocolados pelo usuário externo exibirão nos autos o aviso de documentos não lidos.  

Mais informações sobre o comportamento da opção: 

http://www.pje.jus.br/wiki/index.php/Funcionalidades#Processos_com_documentos_n.C3.A3o_lidos  

## Publicar em sessão

Sobre publicação do acórdão em sessão, no mesmo lugar ele pode publicar o acórdão ou a certidão de julgamento. Os documentos só aparecerão se estiverem devidamente vinculados à sessão e se estiverem assinados. 

Como assessor de plenário, ele tem que ir no menu "Publicação de decisões em sessão" 

Ao entrar ne tela, ele deve selecionar uma data de sessão e mandar pesquisar. As sessões que tiverem acórdão ou certidão de julgamento associados retornarão na pesquisa 

Depois ele vai preencher, na linha do(s) processo(s) correspondentes que ele quer publicar as opções da publicação: data, tipo do prazo, o prazo em si. Se tiverem dois documentos, ou seja, o acórdão e a certidão, na coluna Documento ele precisa marcar qual que ele quer. Geralmente a certidão já vem marcada. Os processos que serão publicados devem estar selecionados por meio da caixa de seleção da primeira coluna. 

Depois de tudo pronto, ele deve selecionar o botão salvar e depois ele seleciona o publicar 

Por meio dessa mesma tela, o usuário poderia publicar em sessão decisões monocráticas. Seria o mesmo procedimento, mas para que as decisões aparecessem na consulta, o gabinete teria que ter usado uma tarefa específica sinalizando que a decisão monocrática seria publicada 

Depois de finalizado tudo, o PJe gera uma intimação para as partes envolvidas de acordo com o que foi preenchido. De acordo com parâmetros configurados, o Ministério Público pode não ser intimado. No caso do TSE, eles não são. 

Há um defeito conhecido quando a pesquisa retorna muitos processos e o usuário seleciona para publicação processos de páginas posteriores à primeira no resultado da pesquisa. A solução de contorno é restringir a pesquisa de forma que o resultado não venha paginado para evitar o erro na publicação.

## Como funciona minuta em lote no PJe 

As tarefas de construção de documentos (minutar ato, elaborar documentos) podem ser executadas em lote (mais de um processo por vez) ou individualmente. Para construir documentos em lote, deve-se selecionar os processos de alguma tarefa onde a minuta em lote esteja habilitada por meio do campo de seleção disponível ao lado do cabeçalho do processo. 

Pode-se também selecionar todos os processos daquela página por meio do campo de seleção que fica logo abaixo dos agrupadores de PROCESSOS / ETIQUETAS. Selecionando essa opção, todos os processos daquela página serão incluídos no lote. Lembramos que o limite de processos por página é 30. 

## Atuação de juiz substituto em processo sigiloso  na zona 

Exemplo de situação: O juiz de uma zona especializada (002ZE) se declarou suspeito. 

Foi designado para atuar no processo o juiz titular da outra especializada (003ZE).  

No sistema, para que cada ze concorra em igualdade de condições, e tbm, por óbvio, pq n existe dois juízes ativos concomitantemente no mesmo juízo eleitoral, a distribuição foi configurada apenas com o cargo de juiz titular respondendo “Sim” para “recebe distribuição”. 

Logo, esse processo em que ele se declarou suspeito foi distribuído para o cargo de juiz eleitoral titular. 

O que pode ser feito para que o juiz designado não visualize os demais processos sigilosos (inclusive com nível 5) e enxergue apenas o feito para o qual ele foi indicado? 

Resposta: Configurar a visibilidade do juiz substituto só pro cargo dele e adiciona ele como visualizador do processo. Ele terá acesso ao processo porque é visualizador e terá acesso às tarefas porque é juiz. 

Resumo: se cadastrar um juiz no cargo Juiz Eleitoral Designado, limitar a visibilidade dele apenas a esse cargo e acrescentar seu cpf como visualizador do processo sigiloso, ele vai visualizar o processo na tarefa minutar ato, assim como o Juiz titular, mesmo que o processo seja nível 5. 

 

##   Intimação de pauta na publicação da lista e no fechamento da pauta 

A publicação de pauta (última aba na Relação de julgamento) no diário utiliza a pessoa Destinatário para ciência pública. A intimação não é gerada para pessoas individuais, já que aquele é um aviso geral da sessão que acontecerá. 

 

As intimações individuais são geradas no fechamento mesmo (primeira aba da Relação de julgamento), ou se você quiser fazer via fluxo do Preparar ato de comunicação. Para inibir as intimações gerais, tem que usar a configuração do Órgão julgador colegiado, onde há um campo lá falando sobre intimação automática da pauta. 

    Campos na intimação de pauta 

  

No documento de intimação de pauta só funcionam as variáveis listadas na regra abaixo: 

 http://www.cnj.jus.br/wiki/index.php/Regras_de_neg%C3%B3cio#RN618 

  

Se tentar colocar outra informação, vai dar problema. Vou copiar aqui a regra: 

  

A publicação da pauta utiliza os processos selecionados pelo usuário na aba Aptos para publicação e monta um documento de acordo com os seguintes parâmetros:  

 

-   Pessoa que será utilizada para registrar ciência quando a publicação ocorrer no DJ conforme configuração do parâmetro pje:fluxo:publicacao:idDestinacaoPessoaCienciaPublica  

-    Tipo de processo documento conforme configuração do parâmetro idTipoProcessoDocumentoIntimacaoPauta  

-    Modelo de documento conforme configuração do parâmetro idModeloIntimacaoPauta  (deve ser usado tanto para o fechamento da pauta quanto para sua publicação) 

 

Para cada processo selecionado, o sistema construirá um documento de acordo com o modelo referenciado, e o utilizará para registrar o ato de comunicação eletronicamente via diário sem prazo para resposta. O movimento de código 60 conforme tabela unificada de movimentos do SGT no CNJ com complemento código 4 com elemento do tipo domínio de código 80 é lançado no processo associado ao documento gerado. Essas configurações de movimento dizem respeito ao registro final no processo "Expedição de outros documentos".  

No modelo de documento utilizado nessa funcionalidade, as seguintes variáveis, e apenas elas, estão disponíveis para uso:  

    processoJudicial, contendo o número do processo;  

    classeJudicial;  

    orgaoJulgador;  

    poloAtivo, contendo a lista de partes do polo ativo com seus respectivos tipos e a lista de advogados que representam partes do polo ativo com seus respectivos números de OAB;  

    poloPassivo, contendo a lista de partes do polo passivo com seus respectivos tipos e a lista de advogados que representam partes do polo passivo com seus respectivos números de OAB;  

    localSessao;  

    dataSessao;  

    horaSessao;  

    tipoSessao  

Para processos da justiça eleitoral:  

    estado;  

    municipio 

 

##  Sobre prazo em horas 

Prazo em em horas dá problema nas suspensões de prazo no PJe. A recomendação é que se converta em dias.  

Sobre a determinação da regulamentação e do magistrado, além de pedido para que o registro do AR abra opção de inseriri o horário, Bruney ressaltou: 

Temos aqui dois pontos: uma é a questão de poder registrar o horário quando da devolução do A.R. (isso seria uma melhoria, quando desenvolvido o sistema essa funcionalidade não foi pensada); outra é a questão da suspensão de prazo em horas (aqui é um defeito). 

 

Nos dois casos precisaríamos evoluir, entretanto, ao mesmo tempo, precisamos priorizar as demandas, de forma a atender, em primeiro lugar, as que impactam no processo eleitoral. 

 

Sem que isso impacte diretamente na questão e na necessidade de evolução do sistema, a jurisprudência do TSE é bem farta no que se refere à conversão de prazos em horas para prazos em dias: Ac. de 23.11.2010 no AgR-AI nº 85876, rel. Min. Aldir Passarinho Junior; Ac. de 6.8.2013 no AgR-REspe nº 664, rel. Min. Dias Toffoli.  

 

Nenhum dos exemplos se adequa aos casos concretos que estamos tratando aqui, mas a ideia me parece a mesma (meu juízo aqui é apenas opinativo e não vinculativo, hehehehe). 

##  Como ficam os processos após remessa 

Primeiro grau: Ao utilizar tarefa “Remeter processo para o TRE”, o processo fica em “Aguardando apreciacão do TRE” bloqueado para novas petições ou edições. Caso seja  retornado do TRE, deve ir automaticamente para o “Analisar processo – ZE" ou “Analisar determinações - ZE”, retirando o bloqueio de edições/novas petições. 

O “Retornar processo” não tem nada a ver com remessa, ele só retorna o processo de volta pro analisar determinações ou analisar processo, verificando os movimentos lançados para encaminhar para um ou outro. No ambiente de zona, para remeter a outra instância, só existe hoje a possibilidade de utilizar o Remeter processo para o TRE, mesmo quando for devolução. De toda maneira, o sistema sempre consulta o processo na instância de origem ao fazer a remessa. Encontrando o processo lá, ele vai automaticamente fazer uma devolução, e não uma nova remessa. 

Segundo grau: 

A partir do verificar pendências, existe a transição “Remessa para outra instância” e existe a “Devolver processo à origem”. 

Ao usar o “Remessa para outra instância”, o objetivo é enviar um processo que tenha iniciado no TRE para TSE ou primeiro grau. A tarefa permite que se protocole um “novo processo” no destino, com classes e assuntos específicos e também com novas configurações de partes. As classes exibidas são as classes passíveis de serem recebidas como recurso configuradas no destino. Caso a classe selecionada esteja configurada no destino com a marcação “exige numeração própria”, um novo número de processo será gerado.  

Após a confirmação, o sistema lançará o movimento de remessa conforme o destino selecionado (TSE ou Zona eleitoral) e manterá o processo em “Aguardando apreciação de outra instância” bloqueado para novas petições ou edições. 

Em Devolver processo à origem, se existir fluxo de acórdão em execução, o processo retornará automaticamente para o Verificar pendências. Caso contrário, o processo irá para a tarefa “Expedir processo – Retorno à origem”, que apresenta um aviso pedindo que o usuário, antes de devolver o processo, verifique se não há expedientes abertos ou tarefas em andamento, de modo a evitar que o processo seja encaminhado sem o devido cumprimento. A tela da tarefa permite a seleção do motivo da devolução e o acionamento do botão “Retorno do processo à origem”. O usuário pode também desistir da tarefa, retornando ao Verificar pendências, ou encaminhar para novos cumprimentos, por meio da transição “Necessita atos de ofício”. Se selecionar o botão de retorno do processo à origem, o sistema verificará se há documentos não assinados para que o usuário possa desistir da execução da tarefa, se for o caso. Na confirmação da execução, o sistema retornará o processo para a última instância de origem (se veio do TSE, retornará para o TSE, se veio do primeiro grau, retornará para o primeiro grau). O sistema lancará o movimento de baixa e deixará o processo bloqueado na tarefa “Manter processos expedidos”. 

 

As tarefas onde os processos permanecem após remessa e devolução são diferentes para que se saiba com mais facilidade qual o caminho que o processo percorreu. 

 

## Como ficam os processos após remessa a outra jurisdição 

O processo, após remetido a outra jurisdição, não deve ficar nessa mesma tarefa. Se gera novo número, é para ficar o número originário em processo arquivado e o novo em analisar novo processo. Se não gera novo número, fica um processo apenas também no analisar novo processo. Pode ser que fique na mesma tarefa se há problema no nosso balanceamento. É que as máquinas do PJe funcionam direcionando requisições para uma ou outra máquina de acordo com a carga maior de um e de outro. Ocorre que quando um usuário estabelece uma sessão em uma máquina, o balanceador deve continuar sempre enviando suas requisições daquela sessão para o mesmo servidor. A requisição para mudar o processo de tarefa foi enviada para outra máquina, o que ocasiona o erro de o processo não tramitar. 

 

## Problemas com sessão na 2.0 

 

 -  Fluxo com órgão julgador deslocado temporariamente (substituição por recesso, por exemplo, ou Recurso Extraordinário no TSE) : O órgão julgador responsável não consegue salvar o voto, dá um erro e fica gerando um monte de cópia do voto. Pode-se verificar as cópias no item Documentos dos autos.  

O que acontece é que o sistema salva o voto no nome do órgão julgador relator, mas na hora que a tela recarrega, ele tenta recuperar um voto vinculado ao órgão julgador autenticado (que é o deslocado), e não tem.  

A solução é alterar o órgão julgador que fará a decisão colegiada antes que seja iniciada a construção dos documentos. Ao final da sessão, depois de assinado o acórdão, o processo pode retornar para o relator original. Foi feita alteração de fluxo para permitir que isso aconteça no TSE.

Se já tiver sido iniciada a construção dos documentos, tem que alterar no banco o órgão julgador do voto que foi salvo pra ser do órgão deslocado e aí os documentos são recuperados. 

Na sessão de julgamento, o relator do processo precisará votar como vogal e novamente terá problemas. Para resolver, tem que alterar o órgão julgador responsável pelo processo no banco, deixar o vogal votar, e depois alterar de volta o órgão.  

Pode ser que ocorra problemas se for necessário retificar voto de relator deslocado ou desse vogal relator depois do julgamento. A solução é mexer na relatoria por meio do banco novamente, alterando de volta depois. 

 - Ao desvincular documento no selecionar documentos para acórdão, em algumas vezes o sistema está apagando o registro do documento na sessão 

 - Ao excluir processo de pauta não fechada, incluir processo em outra pauta e fechar a pauta, o sistema não está vinculando os documentos - resolve com o selecionar documentos para acórdão 

 - No selecionar documentos para acórdão, ao vincular documentos de voto vogal ao acórdão, o sistema não está obedecendo 

 - Ao excluir processo com pauta fechada, pode dar um erro vermelho. Deve-se configurar o parâmetro idProcessoRetiradoPauta  para 273 e tentar novamente 

 

- Editor de tarefa antes da versão 2.0.0.0.64 não exibe conteúdo porque dá problema com caracteres ' (denominado "aspas simples" ou "apóstrofo"), ' ("acento agudo" sem vinculação a uma letra), ` ("acento grave" sem vinculação a uma letra) e \ (denominado "contrabarra" ou "barra inversa"). Para documentos de sessão, a solução é ir no selecionar documentos para acórdão, não selecionar o documento que está com problema e enviar o processo para a unidade que produziu o documento originalmente. Lá, o servidor poderá acessar o conteúdo do documento por meio dos autos digitais, copiar em um editor externo, retirar as aspas, copiar o documento sem as aspas de volta no editor, que está em branco, salvar, e mandar de novo para a COARE. O documento novo criado sem as aspas deve aparecer na tarefa de acórdão da COARE. 

 - Processo cujo julgamento foi encerrado individualmente não aparece para ser incluído em outra sessão, só depois que a sessão é finalizada. Para contornar, o assessor de plenário tem acionado a ASPJe para que o processo seja retirado da sessão via banco e possa incluir na sessão seguinte 

-  Processo não aparecer para ser incluído em mesa mesmo após sessão anterior ser finalizada em geral, é porque o processo está em outra sessão. Se não tem outra sessão em andamento, é porque o cara deixou o processo em uma sessão antiga e inativou a sessão (isso era possível antes da versão 2.0.0.0.64). Para pesquisar em que sessões o processo está, utilizem o menu Audiência e sessões - Processos pautados em sessão. 

## Artigo 260 no PJe 

Há uma especificidade da JE referente à distribuição de processos que afetam a eleição. Art. 260 do Código Eleitoral (CE) - Lei 4737/65: 

Art. 260. A distribuição do primeiro recurso que chegar ao Tribunal Regional ou Tribunal Superior, prevenirá a competência do relator para todos os demais casos do mesmo município ou Estado. 

Perceba que o art. 260 é aplicável, apenas, aos recursos, não sendo aplicado às ações originárias. 

Até as Eleições de 2020 a maioria dos Tribunais Regionais vinham optando, em sua maioria, por não utilizar o art. 260 do CE como critério de Distribuição. 

Ocorre que a Resolução TSE n.º 23.609 passou a prever, expressamente, a distribuição pelo art. 260: 

Art. 64. Recebidos os autos no tribunal, a distribuição do recurso se fará:I por prevenção: a) ao relator do recurso do mesmo município que primeiro tiver chegado ao TRE ou ao TSE, quando se tratar de RRC, RRCI ou DRAP relativo ao cargo de prefeito ou vice-prefeito (Código Eleitoral, art. 260);b) ao relator do recurso do mesmo estado que primeiro tiver chegado ao TSE, quando se tratar de RRC, RRCI ou DRAP relativo ao cargo de governador ou vice-governador (Código Eleitoral, art. 260). 

A Resolução TSE n.º 23.608, por sua vez, fez previsão de distribuição com base no art. 260 do Código Eleitoral para os recursos interpostos em algumas espécies de representações: 

Art. 53. Ao aportarem nos tribunais regionais eleitorais ou no Tribunal Superior Eleitoral, os recursos interpostos nos autos das representações que versem sobre as hipóteses previstas nos arts. 30-A, 41-A, 45, VI, 73, 74, 75 e 77 da Lei n° 9.50411997 serão distribuídos com observância do art. 260 do Código Eleitoral. 

O artigo 260 diz que a escolha pelo usuário de qualquer dos assuntos abaixo listados na autuação de um processo fará com que novos processos daquele assunto naquele ano de eleição e naquele município de origem sejam distribuídos para o mesmo relator, com exceção das classes do item 2: 

 

    Assuntos para o 260: 

i. Abuso – Código CNJ 11717 

ii. Abuso de poder econômico – Código CNJ 11718 

iii. Abuso de poder político/autoridade – Código CNJ 11719 

iv. Abuso – uso indevido de meio de comunicação social – Código CNJ 11720 

v. Captação ilícita de sufrágio – Código CNJ 11721 

vi. Propaganda política – propaganda institucional – Código CNJ 11723 

vii. Conduta vedada a agente público – Código CNJ 11558 

viii. Captação ou gasto ilícito de recursos financeiros de campanha eleitoral – Código CNJ 11685 

ix. Corrupção ou fraude – Código CNJ 11722 

x. Eleições – eleição suplementar – Código CNJ 11647 

xi. Transgressões eleitorais – Código CNJ 11716 

xii. Recursos financeiros de campanha eleitoral – Código CNJ 11684 

xiv. Eleições - Eleição Majoritária - Código CNJ 11645. 

 

DICA: No que se refere a recursos em registros de candidaturas, somente os processos de eleições majoritária são distribuídos com base no art. 260 do CE. Assim, como os assuntos de “registro” são comuns aos cargos proporcionais e majoritários, o assunto “Eleição Majoritária” foi criado para identificar os casos de distribuição pelo art. 260. 

 

2 Classes que excluem a aplicação do art. 260 do Código Eleitoral. 

i. AÇÃO DE IMPUGNAÇÃO DE MANDATO ELETIVO – Código CNJ 11526 

Motivo: inexistência de previsão legal para distribuição pela prevenção do art. 260 do CE nas ações originárias. 

ii. AÇÃO DE INVESTIGAÇÃO JUDICIAL ELEITORAL – Código CNJ 11527 

Motivo: inexistência de previsão legal para distribuição pela prevenção do art. 260 do CE nas ações originárias. 

iii. AÇÃO RESCISÓRIA – Código CNJ .  

Motivo: nos termos dos arts. 76 e 77 do RISTF, aplicáveis a este Tribunal por força do art. 94 do RITSE, a ação rescisória será distribuída automaticamente, excluindo-se o Relator do processo cuja decisão se pretende rescindir. 

iv. RECURSO CONTRA EXPEDIÇÃO DE DIPLOMA – Código CNJ 11533 e REPRESENTAÇÃO – Código CNJ 11541 contra cargo de Presidente da República e Vice (no caso do TSE) E contra cargo de Governador, Vice-Governador, Deputado Federal e Deputado Estadual ou Distrital (no caso dos TREs) 

Os assuntos abaixo não geram a prevenção do art. 260 do CE, uma vez que referem-se a processos originários para o TSE.   

11634 - DIREITO ELEITORAL|Eleições|Cargos|Cargo - Presidente da República 

11641 - DIREITO ELEITORAL|Eleições|Cargos|Cargo - Vice-Presidente da República 

No caso dos Tribunais Regionais Eleitorais, deve-se aplicar a mesma regra para os assuntos inerentes aos cargos de Governador, Vice-Governador, Senador, Deputado Estadual e Deputado Distrital: 

11632 - DIREITO ELEITORAL|Eleições|Cargos|Cargo – Governador 

11639 - DIREITO ELEITORAL|Eleições|Cargos|Cargo – Vice-Governador 

11637 - DIREITO ELEITORAL|Eleições|Cargos|Cargo – Senador 

11630 - DIREITO ELEITORAL|Eleições|Cargos|Cargo – Deputado Estadual 

11631 - DIREITO ELEITORAL|Eleições|Cargos|Cargo – Deputado Federal 

 

3. Como configurar o PJe para que o sistema entenda essas determinações: 

 

Foram criados três agrupamentos de classes e assuntos (Menu Configuração - Tabelas judiciais - Agrupamento de classes ou assuntos) para contemplar as subdivisões de classes e assuntos mencionadas acima. Por mais que um tribunal opte por não utilizar a prevenção do art. 260, via de regra os agrupamentos já estão configurados, podendo sofrer alterações de acordo com a concepção local.  

 

PE1 - Agrupamento que habilita a prevenção do art 260 CE (apenas assuntos específicos) 

PE2 - Agrupamento que desqualifica processo a pertencer a uma cadeia (apenas classes específicas) 

PE3 - Agrupamento que desqualifica processo a pertencer a uma cadeia (classes E assuntos) 

 

Foi criado um parâmetro com uma expressão lógica (utiliza operadores que são comuns na área de TI) para relacionar as regras e os agrupamentos. Por mais que um tribunal opte por não utilizar a prevenção do art. 260, o parâmetro já está configurado, mas com a propriedade "Situação" igual a "inativo".  

 

listaAgrupamentosPrevencao260JE = ou+PE1,ou-PE2,ou-PE3 

 

Sendo assim, para habilitar a prevenção do 260, deve-se alterar esse parâmetro para que a "Situação" seja "ativo". 

OBS: a lista de classes e assuntos que se enquadram ou que são exceções está de acordo com o que foi especificado inicialmente na época que a pendência foi codificada. Nada impede que seja alterada. 

4. Como incluir assuntos em PE1 e PE3 ou classes em PE2? 

 

 

Para incluir novos assuntos em PE1 ou PE3 o configurador deve seguir os seguintes passos: 

a) Menu; 

b) Configuração; 

c) Tabelas Judiciais; 

d) Agrupamento de classes ou assuntos; 

e) Selecionar o botão de editar em PE1 ou PE3; 

f) Escolher a opção “Assuntos Vinculados ao Agrupamento” 

g) Descer a barra de rolagem até o fim para verificar os assuntos já adicionados; 

h) Subir a barra de rolagem, pesquisar o assunto e, em seguida incluir por meio do botão do lado direito ao respectivo assunto encontrado. 

Para incluir novos classes em PE2 o configurador deve seguir os mesmos passos acima, com exceção do item “f”, em que deverá optar por “classes judiciais vinculadas ao agrupamento”. 

Eventuais dúvidas sobre a configuração devem ser enviadas ao email aspje@tse.jus.br 

## Definir revisor 

Um processo, ao ser protocolado, vai incluir o nome do revisor automaticamente se a classe tiver marcada como exige revisor. Nesse caso, na configuração do órgão julgador colegiado, temos que colocar quem é o revisor padrão de cada gabinete. 

 
Se for facultativo, ele pode ter ou não o revisor. 

 
Após o protocolo de processos, dependendo da atualização do fluxo, existe uma tarefa depois do analisar determinação, que permite a determinação do revisor para processos cujas classes tenha revisão marcada como facultativa. Se assim estiver, a tarefa permite que se marque ou desmarque que o processo exige revisão e também permite que o revisor seja alterado. 
 

Você poderá verificar o nome do revisor pelos autos digitais, na opção de exibir mais detalhes do cabeçalho 

Quando um processo está no fluxo de colegiadas, na tarefa “Conferir relatório, voto e ementa”, o sistema verifica se o processo exige revisor, e isso foi selecionado no protocolo, ou se o processo tem uma classe que a revisão é facultativa. Se uma dessas condições for satisfeita, aparece uma transição para que o usuário envie o processo para o revisor, que será o que aparece nos autos. 

Quando a classe exige revisão, o processo só poderá ser pautado se o revisor tiver incluído o voto.  

Para corrigir um revisor no processo utilizando a tarefa, coloca o revisor correto na configuração do colegiado, depois marca a classe com "exige revisor" facultativo, depois coloca o processo, a partir do analisar determinação, na tarefa de definir o revisor. Na tarefa, altere as marcações (exige revisor e nome do revisor) e, por fim, deixe selecionado o revisor correto, retornando depois o processo para analisar determinação. FAÇA ALTERAÇÕES gerais na tela para garantir que o sistema atualizará a definição de acordo com o valor selecionado, já que a tarefa não tem o botão salvar e a alteração será refletida após tramitação quando o sistema detecta que houve mudança. 

Há também a situação em que o processo tem uma classe que exige revisão, mas o julgamento será do recurso. O procedimento correto é marca o facultativo para exige revisão na classe e pautar o processo após o procedimento. Nesse caso, quem envia o processo para a pauta é o relator, não o revisor. Depois, pode-se alterar a classe de volta. Se o processo já tiver sido pautado, pode-se fazer o seguinte: 

·         Tirar da sessão: Para processo com pauta fechada, o sistema gerará a certidão de cancelamento de pauta; 

·         Marcar facultativa a classe para “Exigir Revisor”: Feito. 

·         Ir na tarefa “Analisar determinação”: Pode-se cancelar a decisão colegiada e remeter o processo para SJD. Os documentos construídos de voto, relatório e ementa não serão perdidos. 

·         Tirar o revisor pela tarefa. 

·         Coloca na sessão novamente: Adicionar por mesa na sessão de julgamento. 

 Dessa forma, pode-se alterar a ordem de votação do processo, já que com o revisor, o sistema não permite. 
 
## Votos antes da sessão, Visualização de votos pelo painel do procurador na sessão, painel do membro da OAB na sessão, painel do púlpito, Internet sem usuário e senha 

O relatório, ementa e voto são construídos no PJe da JE por meio da tarefa “Minutar relatório voto e ementa” pelo relator do processo. Se o usuário autenticado estiver em um órgão julgador diferente do relator do processo, é gerada uma inconsistência só resolvida via banco de dados (verificar item 10.1). Por voto, entenda-se que é o conjunto da indicação do voto e o próprio documento de voto. A visualização desses itens/documentos não assinados só é possível se as respectivas marcações “Liberar voto”, “Liberar relatório” e “Liberar ementa” forem realizadas. 

 

Os pontos do sistema onde poderão ser visualizadas são: painel do secretário da sessão, painel do magistrado na sessão, painel do membro da OAB na sessão/painel do membro do ministério público na sessão, púlpito de sustentação oral, Internet - opção Pautas de julgamento (http://www.tse.jus.br/servicos-judiciais/sessoes-de-julgamento/pautas-de-julgamento/pje) e tarefas de vogais. 

 

Depois que inicia a sessão, quando o Assessor de plenário colocar em julgamento, vai aparecer na Internet, sem usuário e senha, o "tipo de voto", ou seja, concedo, nego, mas não aparece o documento.  Na Internet, sem login e senha, só aparece o documento depois de assinado. Já no painel  do membro da OAB,  basta iniciar a sessão.  Em todos os casos, é sempre necessário liberar por meio da tarefa do gabinete 

    Painel do secretário da sessão 

Se o parâmetro “pje:sessao:ocultarVotosAntecipadosNaoMagistrado” estiver marcado como false e o magistrado tiver liberado seu documento para visualização por meio da opção respectiva na tarefa, voto/documentos serão exibidos para o “Assessor de plenário”. 

O “Assessor de plenário” pode liberar os processos para que sejam visualizados na Internet - opção “Pautas de julgamento”, quando inicia a sessão não contínua. Para sessões contínuas, os processos são apresentados após o início da sessão, que é automática, de acordo com o horário planejado. 

O “Assessor de plenário” pode liberar o voto/documentos para que sejam visualizados na Internet - opção “Pautas de julgamento”, quando finaliza a sessão. Se o magistrado tiver liberado seu documento para visualização por meio da opção respectiva na tarefa, os votos serão exibidos na opção “Pautas de julgamento” desde que: 

1. parâmetro “pje:sessao:plenarioVirtual:documentoAssinado" tem deve estar configurado como false 

2. o gabinete tem que ter construído e liberado o voto 

3. o processo foi julgado 

4. a sessão esteja encerrada  

Se o parâmetro  “pje:sessao:plenarioVirtual:documentoAssinado" estiver com o valor “true”, o documento só aparecerá em “Pautas de julgamento” após assinatura do acórdão. 

Os processos são colocados em julgamento automaticamente em sessões contínuas após o início da sessão. 

Os processos e votos/documentos serão visualizados no menu “Painel do membro da OAB na sessão” em sessões contínuas quando iniciada a sessão. Se o parâmetro “pje:sessao:ocultarVotosAntecipadosNaoMagistrado” estiver marcado como false e o magistrado tiver liberado seu documento para visualização por meio da opção respectiva na tarefa, voto/documentos serão exibidos no “Painel do membro da OAB na sessão”. 

Os processos e votos/documentos serão visualizados no menu “Painel do membro do ministério público na sessão” em sessões contínuas quando iniciada a sessão. Se o parâmetro “pje:sessao:ocultarVotosAntecipadosNaoMagistrado” estiver marcado como false e o magistrado tiver liberado seu documento para visualização por meio da opção respectiva na tarefa, voto/documentos serão exibidos no “Painel do membro do ministério público na sessão”. 

O “Assessor de plenário” pode liberar os processos e votos/documentos para que sejam visualizados no menu “Painel do membro do ministério público na sessão” do procurador que está cadastrado naquela sessão em sessões não contínuas quando inicia a sessão. Se o parâmetro “pje:sessao:ocultarVotosAntecipadosNaoMagistrado” estiver marcado como false e o magistrado tiver liberado seu documento para visualização por meio da opção respectiva na tarefa, voto/documentos serão exibidos no “Painel do membro do ministério público na sessão”. 

O “Assessor de plenário” pode liberar o processo para ser visualizado no menu “Púlpito de sustentação oral” em julgamentos de sessões não contínuas quando colocar o processo “Em julgamento” (ícone balancinha sendo exibido). 

O “Assessor de plenário” pode liberar o voto/documentos para que sejam visualizados por meio do menu “Púlpito de sustentação oral” em julgamentos de sessões não contínuas quando clicar no ícone de olho disponível nos processos que estão “Em julgamento” (ícone balancinha sendo exibido). Se o magistrado tiver liberado seu documento para visualização por meio da opção respectiva na tarefa, voto/documentos serão exibidos no “Púlpito de sustentação oral” 

 

Orientação passada para o TSE quando foram disponilizados os paineis: 

  

De ordem da assessora-chefe da Assessoria do PJe , informamos que a versão disponibilizada hoje no TSE, 18 de maio de 2020, contempla um painel aos advogados e ao ministério público para acompanhamento das sessões virtuais e por videoconferência. 

 Para as sessões iniciadas, virtuais ou não, o painel da OAB e do MP exibe documentos de relatório, voto e ementa produzidos pelos gabinetes, desde que liberados para visualização. 

 Conforme já ocorria antes dessa melhoria, a liberação de visualização dos documentos é realizada pelo gabinete, a partir das opções já existentes "Liberar relatório", "Liberar ementa" e Liberar voto", disponíveis nas tarefas de conferência dos documentos. 

 A liberação pode ocorrer por documento, ou seja, o gabinete pode escolher liberar apenas o relatório, assim como pode escolher não liberar documento algum. 

   

 Orientação passada para os TREs quando foram disponilizados os paineis: 

A versão 2.0.0.0.49.3 do PJe nos regionais e no TSE traz uma melhoria solicitada pela OAB e pelo ministério público para que advogados e MP possam enxergar os documentos de voto, relatório e ementa, desde que liberados pelo gabinete, a partir das opções já existentes "Liberar relatório", "Liberar ementa" e Liberar voto", disponíveis nas tarefas de "Aguarda sessão de julgamento" inclusive para julgamento virtual. Caso liberados os documentos, os processos que estejam em sessão aberta terão a opção do placar, que exibe os votos dos magistrados. 

 As permissões para esse painel podem ser encontradas no menu Configuração - Controle de acesso - Funcionalidades, pesquisando pelo identificador "/pages/Painel/ProcuradorMP/sessaoAbertaProcuradorMP.seam". Às permissões que já existem, pode ser acrescentada a permissão para o perfil de advogado. Ou ainda, se for o desejo, retirar permissões. 

   

Além da melhoria nessa funcionalidade, foi disponibilizada uma nova, que só permite acesso aos documentos liberados pelo gabinete de processos em julgamento de sessões abertas não contínuas e que tenham visualização liberada pelo Assessor de plenário. A liberação ocorre por meio de um novo ícone em forma de olho no painel do secretário da sessão que aparece para cada processo. Ao clicar nesse ícone, a visualização dos documentos está liberada para esse novo painel. Além disso, a permissão para o painel deve ser também configurada por meio do controle de acesso - funcionalidades, identificador "/pages/Painel/painel_usuario/painelPulpito.seam" juntamente com a associação do papel "pje:papel:pulpitoSustentacaoOral" ao perfil ao qual vc deseja dar acesso ao novo painel. 

SOBRE ESSAS DUAS FUNCIONALIDADES, A LIBERAÇÃO do ASSESSOR DE PLENÁRIO SÓ É NECESSÁRIA QUANDO SE USA O PAINEL DO PÚLPITO. 

Cada tribunal deve decidir qual painel se aplica a qual situação sua e configurar conforme desejar. 

## Problema de processo migrado que os documentos não aparecem a aba para selecionar documentos para acórdão

Ajustar o nr_instancia do client.tb_processo_trf para o mesmo ds_instancia do core.tb_processo_documento. A migração tem que ser também ajustada para preencher esse campo e o problema deixar de ocorrer.

## Situação do advogado na autuação 

Sobre aparecer "Advogado (não validado)", tanto no cadastro como na retificação da autuação, ocorre o seguinte: 

O Pje, ao acessar a OAB, guarda os dados da validação realizada 

Por vezes, o advogado estava com algum problema por lá, mas foi feito o cadastro mesmo assim por parte do servidor. O sistema deixa, o servidor assume que a pessoa é um advogado e que a situação está ativa. 

Após realizar novas validações, o sistema não apaga a antiga. 

Aí, na hora de exibir o advogado, o sistema pega a primeira validação das que vierem, e aí pode ser que venha aquela de quando ele estava com o cadastro irregular. 

Se vc, como servidor, sabe que aquele advogado é válido, não há problema, isso é só um alerta. Esse alerta só aparece para servidores 

Isso ocorre no cadastro do processo e na retificação 

## Situação de partes: Inativo, baixado, suspenso 

A suspensão é mais para execução criminal, já que um réu pode ser suspenso se estiver cumprindo medidas restritivas e observando-as. Se tinha que comparecer de tempos em tempos e sumiu, volta a estar ativo 

A inativação (situação da parte marcada como "I") e baixa (situação da parte marcada como "B") de parte no processo contempla o mesmo significado, ou seja, a parte cuja relação processual tenha sido extinta por qualquer motivo. A diferença é que partes baixadas ainda podem ser utilizadas como parâmetro nas consultas processuais, assim como são retornadas no detalhamento do processo. Ao realizar consultas processuais utilizando partes inativas como parâmetro, os processos respectivos não serão retornados. 

## Intimação de pessoa representada por defensoria 

Não há restrições para se intimar via sistema uma pessoa física vinculada a uma defensoria, desde que pelo menos um defensor tenha feito o login direitinho. Se a pessoa física tiver o cadastrado validado, o sistema também permitirá o envio eletrônico. **A intimação eletrônica de partes vinculadas a defensoria é permitida sim. Então não há restrições para se intimar via sistema uma pessoa física vinculada a uma defensoria, desde que pelo menos um defensor tenha feito o login direitinho.** 

## Campo máscara no preenchimento de configuração da classe 

O campo de máscara na configuração da classe judicial é para quando é marcada a opção anterior de processo referência. Significa que ao digitar o número do processo referência, o sistema vai colocar máscara, fazendo com que pontinhos e tracinhos apareçam no lugar certo 

## Sobre distribuição e pesos

https://www.cnj.jus.br/wiki/index.php/Distribui%C3%A7%C3%A3o 

Regras de cálculo dos pesos estão no item 4 de: 

https://www.cnj.jus.br/wiki/index.php/Distribui%C3%A7%C3%A3o#Procedimento_de_distribui.C3.A7.C3.A3o 

 

Tenho um magistrado que vai começar a atuar e não quero que ele entre recebendo tudo quanto é processo. Na versão 2.0, fazer o seguinte: 

Ao criar um novo cargo judicial em um órgão julgador, o sistema pergunta se ele deve ser inicializado com os valores dos outros cargos existentes. Sendo assim, o sistema faz cria o novo cargo já com os pesos acumulados dos outros que já existem e estão recebendo distribuição. Orientamos, então, a criar um novo cargo judicial dentro do órgão com as seguintes características: 


Descrição: Podem fornecer a que melhor lhes convier 

 Sigla: Podem fornecer a que melhor lhes convier 

 Cargo: Ministro 

 Recebe distribuição: Sim 

 Cargo Auxiliar: Não 

 Divisor do peso do proceso: 1.0 

 Ativo: Sim 


Ao selecionar a opção "Incluir", o sistema exibirá a seguinte mensagem: 


"Deseja que o acumulador de cargos seja atualizado para não haver compensação na distribuição?" 
 

A resposta deve ser "Sim". 


Após finalizado essa etapa, você deve vincular o magistrado como titular do órgão vinculado a esse novo cargo judicial.

## Audiências

Começando do zero, primeiro você deve apertar em designar audiência, para poder marcar uma. Aí depois de marcada, você pode cancelar, realizar ou remarcar apertando em verificar existência. 

Quando o usuário aperta em Verificar existência de audiência, o sistema verifica se existe audiência agendada para hoje ou para dias seguintes. Se tiver, ele encaminha para a tarefa de fazer o registro da audiência. Caso contrário, ele retorna para o Gerenciar audiências. 

## Unificação de pessoas  

A unificação de pessoas existe para que partes cadastradas repetidas vezes possam ser unificadas no mesmo cadastro. Dessa forma, fica valendo o cadastro principal e os outros que o usuário vincular serão enxergados como a mesma pessoa. Pode-se fazer isso com pessoa físicas, jurídicas ou entes. Os processos onde as pessoas unificadas estiverem cadastradas como partes serão todos refletidos de forma a prevalecer o cadastro principal. A unificação tem volta, ou seja, se você unificou um cadastro e percebeu que não era isso que você queria fazer, pode desunificar. No entanto, se em um processo há uma parte cadastrada com a pessoa principal e a pessoa sendo unificadas, a desunificação não será possível para esse caso não será possível. 

O botão "Unificar" presente no cadastro dos tipos de pessoa citados permitirá que se faça uma pesquisa e recupere que outras pessoas serão vinculadas àquele cadastro. Ao final da pesquisa, o usuário poderá finalizar a unificação. 

O "Desunificar" fica no menu Atividades 

## Publicações no DJe – Como o sigilo é verificado?  

A única propriedade que é levada em consideração para marcar uma publicação como sigilosa ou não é se o processo é sigiloso. 

A dúvida surgiu porque na tarefa “Preparar ato de comunicação”, no 2o passo, existe a opção “sigiloso” ao lado do nome da parte Marcar essa opção não tem efeito na publicação do DJe. Ou seja, caso o processo não seja sigiloso, os dados da parte aparecerão mesmo que esta opção esteja selecionada. 

Então qual a finalidade da opção “Sigiloso” na tarefa “Preparar ato de comunicação?” 

Marcar essa opção, deveria refletir no documento que será criado/selecionado em “Instrumento de comunicação” após clicar no “lápis”. E diz respeito ao sigilo do documento ao ser listado nos autos digitais. No entanto, a recomendação é NÃO utilizar essa marcação. Ela não se comporta como o esperado e precisará de correção. 

## Carta Precatória - Visualização promotor deprecado. 

Por meio do Ofício nº 022/2020 – GABCRE/TRE-AM, o Vice-Presidente e Corregedor Regional Eleitoral do Amazonas, Des. Jorge Manoel Lopes Lins, apresentou sugestão para a implementação de funcionalidade que permita a inclusão do membro do Ministério Público Eleitoral do juízo deprecado nos processos do PJe autuados na classe Carta Precatória. 

O procedimento foi encaminhado a essa Assessoria para manifestação. 

Após realização de testes no ambiente de homologação, seguem as considerações: 

Quando a Carta Precatória é distribuída pelo deprecante diretamente na zona deprecada, observa-se manutenção da numeração única do processo (da zona deprecada) e  que os autos ficam vinculados a caixa do Procurador deprecado. 

Na hipótese de os autos serem autuados na zona deprecante e remetidos à zona deprecada, observam-se duas situações: 

a)  Quando a remessa é para outra zona do mesmo Estado, a  numeração permanece e, a princípio, o processo ainda fica vinculado na caixa do Promotor deprecante. Entretanto, no primeiro ato de comunicação, o processo migra para caixa correta, ou seja, na primeira intimação ao Ministério Público, o promotor do juízo deprecado é comunicado, de forma a ser viabilizada a atuação; 

b) A remessa entre zonas de Estados distintos não é praxe, entretanto, tecnicamente, quando a remessa é para zona de outro Estado o número do processo é alterado (art. 5º da Resolução CNJ n.º 65/2008), mas as partes permanecem as mesmas, ou seja, não atualiza para o Ministério Público do Estado deprecado. Neste caso, é necessário que o Cartório Eleitoral deprecado atualize os dados do processo, de forma a inserir o Ministério Público deprecado na autuação.

Verifica-se, assim, que a funcionalidade solicitada já consta do sistema. 

