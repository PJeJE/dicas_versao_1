# Variáveis

|  Descrição  | Código |
|:-------|:----------|
| Número do Processo |  #{processoTrfHome.instance.numeroProcesso} |
| Número do processo referência (o número do drap estará nessa variável) |  #{processoTrfHome.instance.processoReferencia} |
| Assuntos do Processo| #{processoTrfHome.instance.assuntoTrfListStr} |
| Nome Autor Processo|#{processoTrfHome.instance.tipoNomeAutorProcesso}|
| Nome Réu Processo|#{processoTrfHome.instance.nomeReuProcesso}|
| Partes Polo Passivo|#{processoTrfHome.processoPartePoloPassivoSemAdvogadoStr}|
| Nome Autor Ativo Processo|#{processoTrfHome.instance.nomeAutorAtivoProcesso}|
| Nome Outros Interessados|#{processoParteHome.processoParteTerceiroSemVinculacaoList}|
| Lista Nome Autor|#{processoTrfHome.nomeCpfAutorList}|
| Partes polo Ativo|#{processoTrfHome.processoPartePoloAtivoSemAdvogadoStr}|
| Endereço Partes Polo Ativo|#{processoTrfHome.processoParteEnderecoPoloAtivoStr}|
| Endereço Partes Polo Passivo|#{processoTrfHome.processoParteEnderecoPoloPassivoStr}
| Lista Tipo Nome Advogado Autor|#{processoTrfHome.instance.tipoNomeAdvogadoAutorList}|
| Lista Tipo Nome Advogado Réu|#{processoTrfHome.instance.tipoNomeAdvogadoReuList}|
| Tipo Nome Réu Processo|#{processoTrfHome.instance.tipoNomeReuProcesso}|
| Endereço Advogado Polo Ativo|#{processoTrfHome.advogadoEnderecoPoloAtivoStr}|
| Endereço Advogado Polo Passivo|#{processoTrfHome.advogadoEnderecoPoloPassivoStr}|
| Classe do Processo|#{processoTrfHome.instance.classeJudicial}|
| Data da Distribuição|#{processoTrfHome.dataDistribuicao}|
| Data da Audiência|#{processoTrfHome.dataAudiencia}|
| Tipo de Audiência|#{processoTrfHome.tipoAudiencia}|
| Endereço da Sala de Audiência|#{processoTrfHome.enderecoSalaAudiencia}|
| Sala de Audiência|#{processoTrfHome.salaAudiencia}|
| Data Atual|#{currentDate}|
| Data Atual Abreviada|#{dataAtualAbreviada}|
| Data Atual Extenso|#{dataAtual}|
| Data atual Formatada|#{dataAtual}|
| Data e Hora Atual|#{currentDatetime}
| Hora Atual|#{currentTime}|
| Data Semana Hoje Extenso|#{dataAtualExtenso}|
| Órgão Julgador Processo|#{processoTrfHome.instance.orgaoJulgador}|
| Cidade Órgão Julgador Processo|#{processoTrfHome.instance.orgaoJulgador.localizacao.endereco.cep.municipio}|
| UF Órgão Julgador|#{processoTrfHome.instance.orgaoJulgador.localizacao.endereco.cep.municipio.estado.codEstado}|
| Juiz Órgão Julgador|#{processoTrfHome.instance.nomeJuizOrgaoJulgador}|
| Endereço Órgão Julgador|#{processoTrfHome.instance.orgaoJulgador.localizacao.endereco.enderecoCompleto}|
| Objeto do processo|#{processoTrfHome.instance.objeto}|
| Cargo do órgão julgador do processo|#{processoTrfHome.instance.orgaoJulgadorCargo}|
| Usuário Logado|#{usuarioLogado.nome}|
| Papel usuário logado|#{usuarioLogadoLocalizacaoAtual.papel}|
| Login Usuário Logado|#{usuarioLogado.login}|
| Nome do Usuário Logado|#{usuarioLogado.nome}|
| Partes formatadas| [#{processoJudicialAction.recuperarParteFormatada(true, true, 'A', 'P', 'T')}](recuperarparte.md)
| Presidente da sessão| #{sessaoComposicaoOrdemManager.obterPresidenteSessao(sessaoPautaProcessoTrfManager.getSessaoPautaProcessoTrfJulgado(tramitacaoProcessualService.recuperaProcesso()).sessao, true)} |
| Procurador da sessão| #{pessoaProcuradorManager.getTituloProcurador(sessaoPautaProcessoTrfManager.getSessaoPsautaProcessoTrfJulgado(tramitacaoProcessualService.recuperaProcesso()).sessao)} |
| Revisor| #{pessoaMagistradoManager.getMagistradoTitular(orgaoJulgadorColegiadoOrgaoJulgadorManager.recuperarOrgaoJulgadorRevisorPadrao(tramitacaoProcessualService.recuperaProcesso()).orgaoJulgadorRevisor.orgaoJulgador).getNome().toUpperCase()} |
| Partes dentro da certidão de julgamento | #{processoJudicialManager.recuperarParteFormatada(sessaoProcessoDocumentoHome.sessaoPautaProcessoTrf.processoTrf, false,true,false,'A','P','T')} |
| Cabeçalho do processo com cadeia recursal em siglas dentro da sessão| #{sessaoProcessoDocumentoHome.sessaoPautaProcessoTrf.processoTrf} |
| Cabeçalho do processo com cadeia recursal em siglas | #{processoTrfHome.instance} |
| Cabeçalho do processo com cadeia recursal por extenso, exceto classe do principal | #{processoTrfHome.instance.extensoClasse != null ? processoTrfHome.instance.extensoClasse : processoTrfHome.instance.classeJudicial} |
| Cabeçalho do processo com cadeia recursal por extenso, exceto classe do principal dentro da sessão | #{sessaoProcessoDocumentoHome.sessaoPautaProcessoTrf.processoTrf.extensoClasse != null ? sessaoProcessoDocumentoHome.sessaoPautaProcessoTrf.processoTrf.extensoClasse : sessaoProcessoDocumentoHome.sessaoPautaProcessoTrf.processoTrf.classeJudicial} |
| Escreve título Juiz ou Juíza de acordo com a informação sexo do cadastro do magistrado relator | #{processoTrfHome.getRelator(processoTrfHome.instance) != null and processoTrfHome.getRelator(processoTrfHome.instance).sexo == 'F'? 'Juíza': 'Juiz'} |
| Número do processo para uso em modelos de oficial de justiça | #{processoExpedienteCentralMandadoHome.instance.processoExpediente.processoTrf.processo.numeroProcesso} |
| Classe do processo para uso em modelos de oficial de justiça | #{processoExpedienteCentralMandadoHome.instance.processoExpediente.processoTrf.classeJudicial} |
ocesso} |
| Partes do processo para uso em modelos de oficial de justiça | #{processoJudicialManager.recuperarParteFormatada(processoExpedienteCentralMandadoHome.instance.processoExpediente.processoTrf, false,true,false,'A','P','T')} |
| Recupera conteúdo dos documentos relatório, voto relator e ementa | #{sessaoProcessoDocumentoManager.getEmenta()}, #{sessaoProcessoDocumentoManager.getRelatorio(null)}, #{sessaoProcessoDocumentoManager.getVoto(null)} |
| Recupera data da última sessão de julgamento | #{sessaoProcessoDocumentoManager.getDataUltimaSessaoJulgamento(null)} |
