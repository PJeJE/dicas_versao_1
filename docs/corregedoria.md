# Procedimentos da corregedoria

O objetivo dessa documentação é deixar registrado as possibilidades de atuação em processos por meio de tarefas de fluxo quando eles estão nas unidades da corregedoria. 

Um processo de uma classe padrão (não corregedoria) entra no PJe por meio do Fluxo Originárias na tarefa Verificar e Certificar dados do processo

## Verificar e Certificar dados do processo

O processo, seguindo o fluxo padrão, cairá na tarefa Remeter Processo

## Remeter Processo

A partir dessa tarefa, há a possibilidade de iniciar o cumprimento na corregedoria por meio da transição Remeter à Unidade de Fiscalização e Cadastro Corregedoria

### Remeter à Unidade de Fiscalização e Cadastro Corregedoria

Aqui o processo irá para o fluxo principal de corregedoria. Com essa transição, o fluxo originárias será encerrado e o único fluxo do processo será o da corregedoria.

## Verificar Pendências

A partir da tarefa Verificar Pendências, também há a possibilidade de se acionar a corregedoria. As possibilidades são:


### Remeter à Unidade de Assuntos Judiciários - Corregedoria

Lança movimento 60044 e remete o processo para o fluxo Fluxo - Processar Atividades no Processo - Corregedoria

Ao retornar, testa de houve encaminhar gab corregedoria e encaminha. Se não houve, testa se houve encaminhamento pro arquivo e vai pra realiza baixa. Caso contrário, testa encaminhar SJD e volta pro verificar pendências ou então vai pro término. 


### Remeter ao Gabinete do Corregedor

Faz com que o fluxo de gabinetes seja iniciado no gabinete da corregedoria, sem redistribuir o processo


### Remeter à Unidade de Fiscalização e Cadastro Corregedoria (já descrita mais acima)

## Fluxo principal corregedoria

Estabelece o campo pessoa relator

	Corregedoria Unidade de Fiscalização e Cadastro	Chefe de Seção
Corregedoria Unidade de Fiscalização e Cadastro	Servidor
Corregedoria Unidade de Fiscalização e Cadastro	Colaborador
Corregedoria Unidade de Fiscalização e Cadastro	Coordenador
Administração PJe	Administrador

### Verificar dados - Processo Corregedoria

Remeter à SJD - encerra fluxo da corregedoria e inicia fluxo originárias, lançando movimento (60005)

Remeter ao cumprimento de determinações - inicia fluxo de cumprimento determinações corregedoria. Finalizado, retorna ao verificar pendências - processo corregedoria

Elaborar decisão colegiada - inicia fluxo de decisão colegiada

Elaborar Decisão Monocrática - inicia fluxo de preparação de ato judicial

Remeter ao Certificar e alterar dados

### Verificar pendências - Processo Corregedoria

Remeter ao TSE desde que a aplicação seja de segundo grau

Devolver Processo Corregedoria a Origem

Arquivar processo - lança movimento e envia processo para  Manter Processos Arquivados - Processo Corregedoria
