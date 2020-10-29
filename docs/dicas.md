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

-  Processo não aparecer para ser incluído em mesa mesmo após sessão anterior ser finalizada em geral, é porque o processo está em outra sessão. Se não tem outra sessão em andamento, é porque o cara deixou o processo em uma sessão antiga e inativou a sessão (isso era possível antes da versão 2.0.0.0.64). Para pesquisar em que sessões o processo está, utilizem o menu Audiência e sessões - Processos pautados em sessão 


