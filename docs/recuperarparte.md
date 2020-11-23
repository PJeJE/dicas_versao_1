#Variável recuperarParteFormatada

Uso: #{processoJudicialAction.recuperarParteFormatada(true, true, 'A', 'P', 'T')} 

- Essa variável permite que se recupere os nomes das partes do processo e seus tipos (recorrente,recorrido...) juntamente com seus advogados alinhados. Pode-se recuperar os advogados com o número da OAB ou não. Pode-se recuperar em formato de tabela (alinhado) ou não (alinhamento pode ter alguma variação, mas não causará problemas na publicação do Diário antigo) Pode-se recuperar todos os polos ou especificar polos específicos.

A variável retorna o nome social, caso tenha sido cadastrado. Se o parte for sigilosa, retorna "Em segredo de justiça" em lugar do nome da parte.

Ao utilizar a expressão acima em modelos de documentos, o documento resultante será contruído exibindo, no lugar da expressão, as partes do processo junto com representantes advogados em linhas separadas e com colunas alinhadas, de forma que sejam exibidos os nomes dos tipos de parte respectivos junto com os nomes das partes. Para o caso de advogados, a alinhamento é feito de forma que o advogado fique vinculado à parte que ele representa.

Utilizando diferentes parâmetros entre os parênteses, pode-se alterar o que será retornado.

- primeiro item dentro dos parênteses informa que a resposta virá dentro de uma tabela (true) ou fora (false);
- segundo item informa se, quando houver advogados, deve ser exibida a oab (true) ou não (false);
- Terceiro item "A" informa que devem ser retornadas as partes do polo ativo;
- Quarto item "P" informa que devem ser retornadas as partes do polo passivo;
- Quinto item "T" informa que devem ser retornadas os terceiros cadastrados no processo.


A variável pode ser utilizada em modelos de documentos utilizados em tarefas e também no juntar documentos dos autos digitais.


O usuário pode configurar a variável no modelo de documento de várias formas:


processoJudicialAction.recuperarParte(true, false,'A')

ou

processoJudicialAction.recuperarParte(true, true,'A', 'P')

ou

processoJudicialAction.recuperarParte(false, true,'T')


ou seja, que as partes possam ser recuperadas quando estiverem no polo ativo, passivo ou terceiros conjuntamente ou separadamente, de acordo com o desejo do configurador, que sejam exibidas em formato de tabela caso o primeiro parâmetro seja true, e que a OAB seja também recuperada caso o segundo parâmetro da variável seja true

