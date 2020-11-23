# Variáveis

|  Descrição  | Código |
|:-------|:----------|
| Número do Processo |  #{processoTrfHome.instance.numeroProcesso} |
| Assuntos do Processo| #{processoTrfHome.instance.assuntoTrfListStr} |
| Partes formatadas|#{processoJudicialAction.recuperarParteFormatada(true, true, 'A', 'P', 'T')} onde
    • primeiro item dentro dos parênteses informa se a resposta virá dentro de uma tabela (true) ou fora (false);
    • segundo item informa se, quando houver advogados, deve ser exibida a oab (true) ou não (false);
    • Terceiro item "A" informa que devem ser retornadas as partes do polo ativo;
    • Quarto item "P" informa que devem ser retornadas as partes do polo passivo;
    • "Quinto item "T" informa que devem ser retornadas os terceiros cadastrados no processo.|
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
| Usuário Logado|#{usuarioLogado.nome}|
| Papel usuário logado|#{usuarioLogadoLocalizacaoAtual.papel}|
| Login Usuário Logado|#{usuarioLogado.login}|
| Nome do Usuário Logado|#{usuarioLogado.nome}


