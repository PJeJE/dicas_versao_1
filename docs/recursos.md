# Recursos internos

Quando interpostos os recursos agravo regimental, embargos de declaração e recurso extraordinário, impugnação ao registro e notícia de inelegibilidade não há alteração na numeração do processo. Não obstante, o processamento desses recursos é realizado de forma diversa, com partes de tipos diversos, decisões e julgamentos exclusivos do recurso. Além disso, é primordial para análise dos recursos identificar qual a origem do recurso, ou seja, se a parte está recorrendo de uma decisão do processo ou de uma decisão relacionada a outro recurso. 

Descreveremos aqui o mecanismo utilizado no PJe para que esse registro seja realizado de forma a permitir o tratamento diferenciado que a interposição requer. 

## Classes

Os recursos internos, apesar de serem interpostos por meio de documentos, são mapeados diretamente em classes processuais disponíveis nacionalmente no [Sistema de Gestão de Tabelas Processuais Unificadas](https://www.cnj.jus.br/sgt/consulta_publica_classes.php)

Sendo assim, ao serem registrados os recursos internos, o sistema fará a identificação por meio de uma nova capa processual vinculada ao mesmo número de processo com a classe vinculada ao recurso correspondente. Vejamos um exemplo na consulta processual de uma Ação Cautelar com um recurso interno vinculado:

![Consulta](img/recurso1.png)

Com a devida permissão, o usuário pode pesquisar outras capas vinculadas ao processo. Essa opção vem desmarcada por padrão, mas no caso de querer visualizar separadamente a capa do recurso, o usuário pode selecionar a opção "Incluir recursos internos" na pesquisa.

![Consulta recursos internos](img/recurso2.png)

Veja o resultado da consulta:

![Resultado da consulta](img/recurso3.png)

Ao selecionar qualquer das opções, o sistema exibirá todo o conteúdo do processo, mas a "capa", ou seja, o cabeçalho superior dos autos será exibido de acordo com a seleção. Veja os autos com a capa original do processo:

![Capa processo](img/recurso5.png)

Veja agora os autos com a capa processual gerada para o recurso:


![Capa recurso](img/recurso4.png)

Sendo assim, o PJe precisa estar com a configuração da classe Embargos de declaração como recurso interno para que seja possível registrar o recurso correspondente. Essa configuração já está feita por padrão. Colocamos aqui a informação para que o usuário saiba qual o impacto em alterar. A configuração da classe correspondente por meio do menu Configuração - Tabelas Judiciais - Classe Judicial - Classe Judicial deve estar assim:

![Configuração da classe](img/recurso6.png)

Perceba que as informações importantes para o registro do recurso estão destacadas. Ou seja, a classe tem que ter o como Natureza como "RECURSO INTERNO", deve estar marcada como recursal e deve ter o tipo de documento inicial correspondente vinculado.

## Como é iniciado um recurso interno

Via de regra, o recurso é interposto quando o usuário externo (advogado, procurador, parte) inclui um novo documento expondo seu pleito. O documento, se classificado corretamente pelo usuário na interposição, terá o tipo correspondente à classe recursal interna. Ou seja, se o advogado, por exemplo, quer recorrer por meio de Embargos de Declaração em uma Ação Cautelar, ele deve selecionar, na tela correspondente, o tipo de documento Embargos de Declaração. Veja a tela de inclusão de documentos que o advogado tem acesso:

![Inclusão de documento](img/recurso7.png)

Ele deve selecionar a opção Embargos de Declaração para interpor o recurso correspondente. Ao finalizar a inclusão do documento, é iniciada uma tarefa "Registrar recurso" para que o servidor faça o registro.

![Registrar recurso](img/recurso8.png)

Veja que a tarefa ser iniciada é resultado de uma configuração no tipo de documento. Conforme pode-se verificar abaixo, o tipo de documento Embargos de declaração tem um "Fluxo associado". É o fluxo que contém a tarefa registrar recurso. O sistema entende, desse forma, que ao ser inserido um documento desse tipo, será iniciada uma tarefa.

![Tipo de documento](img/recurso9.png)

E o que fazer quando o advogado protocola um documento que não iniciou a tarefa de recurso?

Ao analisar os autos do processo, o servidor percebe que o documento de petição inserido pelo advogado é na verdade um recurso interposto. 

![Autos petição](img/recurso10.png)

O servidor deve, então, iniciar a tarefa de registro de recurso.

Essa possibilidade se dá a partir da tarefa "Analisar determinação"

![Transição registrar recurso](img/recurso11.png)

A tarefa de registro de recurso é criada:

![Recurso com petição](img/recurso12.png)

## Registrando um recurso

### Classificar recurso

O primeiro passo no registro do recurso é a classificação. Na classificação, o servidor pode selecionar qual o documento principal do registro e também se o recurso foi interposto para o processo originário ou para um outro recurso, caso já tenham sido registrados recursos para esse processo anteriormente.

A lista de recursos já registrados exibe todos os recursos já registrados pelo servidor. Cada item corresponde a uma capa processual a mais já gerada para o processo originário.

A lista de recursos não registrados exibe todos os documentos vinculados a classes recursais classificadas como "RECURSO INTERNO" e que não estão ainda vinculados a uma capa processual recursal. Em outras palavras, o advogado protocolou um documento de embargos, mas o servidor ainda não registrou o recurso.

Mas o advogado protocolou uma petição contendo um registro de embargos e não é exibida na lista de recursos não registrados. Por quê?

Porque o servidor precisa reclassificar esse documento. A reclassificação acontece na mesma tela. O servidor deve fazer essa reclassificação por meio do ícone de lápis disponível na coluna Ações do documento de petição correspondente:

![Recurso com petição](img/recurso13.png)

Ao selecionar salvar, veja que o sistema moverá o documento, que estava na lista "Outros documentos do processo" para a lista "Recursos não registrados":

![Recurso com petição](img/recurso14.png)

Para o registro do recurso, é obrigatório que um item da lista "Recursos não registrados" esteja selecionado. Se o usuário tentar prosseguir sem a seleção, o sistema não permitirá, notificando que a seleção deve ser realizada:

![Recurso com petição](img/recurso15.png)

### Confirmar cadeia / órgão julgador

Em construção
