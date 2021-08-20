Instruções sobre audiências

# Procedimento atual no primeiro grau (até 31/08/2021)

## Quero marcar uma audiência:

Pelo "Analisar Determinação" / "Analisar Processos", selecione "Gerenciar Audiência"

Estando na tarefa "Gerenciar Audiência - ZE", você terá as opções: "Designar Audiência", "Verificar existência de audiência" e "Cancelar". Pelo "Cancelar", você retornará à tarefa anterior. Pelo "Designar Audiência", você poderá agendar audiência ou realizar audiências já agendadas.

A tela será exibida com algumas opções, conforme descrito em http://www.pje.jus.br/wiki/index.php/Funcionalidades#Tarefas_de_audi.C3.AAncia, mas deve-se ir até o final da tela, no agrupador "Audiência". Vc poderá agendar uma nova audiência. Ao clicar em "Reservar sala", o sistema agendará a audiência gerando a movimentação de designação nos autos. 

** Configurações necessárias para o correto funcionamento:

- Configurar salas pra cada órgão julgador

- Configurar tempo de audiência para cada tipo de audiência e cada órgão julgador


Se já houver audiência marcada anteriormente não realizada, o usuário só conseguirá agendar novas se a variável de fluxo correta estiver setada na tarefa. A expressão a ser utilizada é a seguinte:

 #{tramitacaoProcessualService.gravaVariavelTarefa('pje:fluxo:audiencia:permitirDesignarMultiplas', true)}

Deve ser configurada essa expressão em uma ação do evento entrar no nó.

## Opções para audiências já designadas

Após agendada, as audiências marcadas aparecerão no agrupador "Últimas audiências do processo". Na coluna "Ações" da tabela de audiências desse agrupador estarão disponíveis as seguintes opções:

- Redesignar
- Cancelamento
- Converter em Diligência

Pela tarefa atual, o usuário tem a opção de "Retornar ao Gerenciar Audiência".

** Configurações necessária para o correto funcionamento

Parâmetro "pje:audiencia:realizacaoEmFluxo" esteja marcado como "true"


## Quero realizar uma audiência já marcada:

A partir da tarefa "Gerenciar Audiência - ZE", o usuário deve selecionar "Verificar existência de audiência". Se houver audiência pendente de realização, o sistema encaminhará o usuário para a tarefa "Informar Dados da Audiência - ZE". A tarefa permitirá que o usuário registre a realização da primeira audiência pendente de realização. O usuário poderá informar se a audiência foi realizada e, em caso afirmativo, os nomes do realizador e conciliador, assim como dados do acordo.

Nota: quando o usuário aperta em "Verificar existência de audiência", o sistema verifica se existe audiência agendada para hoje ou para dias seguintes. Se tiver, ele encaminha para a tarefa de fazer o registro da audiência. Caso contrário, ele retorna para o Gerenciar audiências. 

Ao finalizar, a audiência ficará marcada como finalizada. As seguintes opções estarão disponíveis: "Minutar ata de audiência" e "Retornar ao Gerenciar Audiência". O usuário deverá selecionar a opção "Minutar ata de audiência". O sistema apresentará a tela com o editor de texto para a produção da ata. A ata poderá ser construída e assinada nessa mesma tarefa, o que fará com que a movimentação de realização seja gerada, juntamente com a ata. O usuário também poderá selecionar a opção "Remeter para o Juiz Eleitoral assinar". Após a assinatura do juiz, o movimento e o documento assinado serão exibidos nos autos. 

** Configurações necessária para o correto funcionamento

Parâmetro "pje:audiencia:realizacaoEmFluxo" esteja marcado como "true"


------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# Novo procedimento (até 31/08/2021)

## Quero marcar uma audiência:

Pelo "Analisar Determinação" / "Analisar Processos", selecione "Audiências"

Estando na tarefa "Audiências", pelo "Cancelar", você retornará à tarefa anterior. As opções da tela atual estão descritas em http://www.pje.jus.br/wiki/index.php/Funcionalidades#Tarefas_de_audi.C3.AAncia.

Para marcar uma nova audiência, deve-se ir até o final da tela, no agrupador "Audiência". Serão exibidas as opções de designação sugerida e designação manual. Selecione designação sugerida, o tipo de audiência e selecione "Procurar horário". O sistema exibirá o próximo horário disponível. Ao clicar em "Reservar sala", o sistema agendará a audiência gerando a movimentação de designação nos autos. 

Se já houver audiência marcada anteriormente não realizada, o usuário deve seelecionar o opção "Designar nova audiência" e prosseguir com a marcação.

** Configurações necessárias para o correto funcionamento:

- Configurar salas pra cada órgão julgador

- Configurar tempo de audiência para cada tipo de audiência e cada órgão julgador

Se já houver audiência marcada anteriormente não realizada, o usuário só conseguirá agendar novas se a variável de fluxo correta estiver setada na tarefa. A expressão a ser utilizada é a seguinte:

 #{tramitacaoProcessualService.gravaVariavelTarefa('pje:fluxo:audiencia:permitirDesignarMultiplas', true)}

Deve ser configurada essa expressão em uma ação do evento entrar no nó.

## Opções para audiências já designadas

Após agendada, as audiências marcadas aparecerão no agrupador "Últimas audiências do processo". Na coluna "Ações" da tabela de audiências desse agrupador estarão disponíveis as seguintes opções:

- Realização
- Redesignar
- Cancelamento
- Converter em Diligência

## Quero realizar uma audiência já marcada:

 O usuário deverá clicar em "Realização".

O sistema apresentará no final da tela um quadro denominado "REALIZAR AUDIÊNCIA" para registrar as informações, onde o usuário poderá informar se a audiência foi realizada e, em caso afirmativo, os nomes do realizador e conciliador, assim como dados do acordo. O usuário clica em "Próximo", e a audiência ficará marcada como finalizada. A aba "Anexar documento a audiência" passa a ser apresentada. O usuário preenche os documento da ata pelo editor de texto disponível na aba, seleciona "Salvar" e o botão "Assinar documento(s)" será disponibilizado. Ao assinar o documento, o usuário deve selecionar o botão "Concluir". O movimento de realização e o documento assinado serão exibidos nos autos.  

** Configurações

Caso o parâmetro "pje:audiencia:realizacaoEmFluxo" esteja marcado como "false".


## "Finalizei a audiência, mas não houve movimento de realização".  

O movimento de realização será lançado após o botão "Concluir" ser acionado. Caso o botão não seja acionado, o documento eventualmente produzido aparece nos autos, mas sem movimento associado. Nesse caso, na tarefa "Audiências" será apresentada a opção "Ata de audiência". A opção exibirá, no final da tela, os dados da realização e permitirá ao usuário clicar em "Proximo". A tela para construção do documento será exibida, mas o usuário deve clicar em "Concluir". O movimento será lançado nos autos vinculado ao documento já gerado.


## "Finalizei a audiência, mas não fiz a ata"

O documento da audiência será produzido quando a aba "Anexar documento a audiência". Caso o usuário não finalize a ata, mas já tiver informado os dados de realização, na tarefa "Audiências" será apresentada a opção "Ata de audiência". A opção exibirá, no final da tela, os dados da realização e permitirá ao usuário clicar em "Proximo" para construir o documento. Para finalizar, após assinatura, o usuário deve clicar em "Concluir".



## Quero verificar informações sobre todas as audiências do processo

Para verificar audiências do processo e seu estado atual, o usuário deverá abrir os autos digitais e, no menu de opções (ícone de três barrinhas horizontais no canto superior direito dos autos) selecionar a opção Audiência. O sistema apresentará uma listagem com as audiências já marcadas com os respectivos estados atuais.



