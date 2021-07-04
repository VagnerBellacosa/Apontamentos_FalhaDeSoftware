IBM OS/VS - Mensagens comuns de erro de sistema e códigos de ABEND



| Brasília (DF), Sábado, 29 de Janeiro de 2022. Bom Dia! 11:20:26 |
| [![clique aqui para imprimir esta página](http://www.cadcobol.com.br/impri_01.gif)](javascript: window.print();) | 
|![Volta a página anterior](http://www.cadcobol.com.br/botao_02.gif) |
| [![Volta ao Menu Principal](http://www.cadcobol.com.br/botao_03.gif)](http://www.cadcobol.com.br/menuprin.htm) |
| ------------------------------------------------------------ |
| ------------------------------------------------------------ |
| ------------------------------------------------------------ | 
| ------------------------------------------------------------ |
|                                                              |                                                              |                                                              |                                                              |



Desenvolvido por DORNELLES Carlos Alberto - Analista de Sistemas - Brasília DF. - cad_cobol@hotmail.com





**Mensagens comuns de erro de sistema e códigos de ABEND** [Introdução](http://www.cadcobol.com.br/abend_01.htm#intro) [Identificando o código de erro](http://www.cadcobol.com.br/abend_01.htm#identerrorcode) 



**Códigos de ABEND mais comuns** 
[<br>        ABEND CODE         013](http://www.cadcobol.com.br/abend_01.htm#013)
[<br>        ABEND CODE         0C1](http://www.cadcobol.com.br/abend_01.htm#0C1)
[<br>        ABEND CODE         0C4](http://www.cadcobol.com.br/abend_01.htm#0C4)
[<br>        ABEND CODE         0C5](http://www.cadcobol.com.br/abend_01.htm#0C5)
[<br>        ABEND CODE         0C7](http://www.cadcobol.com.br/abend_01.htm#0C7)
[<br>        ABEND CODE         106](http://www.cadcobol.com.br/abend_01.htm#106)
[<br>        ABEND CODE         213](http://www.cadcobol.com.br/abend_01.htm#213)
[<br>        ABEND CODE         222](http://www.cadcobol.com.br/abend_01.htm#222)
[<br>        ABEND CODE         2F3](http://www.cadcobol.com.br/abend_01.htm#2F3)
[<br>        ABEND CODE         322](http://www.cadcobol.com.br/abend_01.htm#322)
[<br>        ABEND CODE         613](http://www.cadcobol.com.br/abend_01.htm#613)
[<br>        ABEND CODE         722](http://www.cadcobol.com.br/abend_01.htm#722)
[<br>        ABEND CODE         804](http://www.cadcobol.com.br/abend_01.htm#804)
[<br>        ABEND CODE         806](http://www.cadcobol.com.br/abend_01.htm#806)
[<br>        ABEND CODE         80A](http://www.cadcobol.com.br/abend_01.htm#80A)
[<br>        ABEND CODE         813](http://www.cadcobol.com.br/abend_01.htm#813)
[<br>        ABEND CODE         913](http://www.cadcobol.com.br/abend_01.htm#913)
[<br>        ABEND CODE         A13](http://www.cadcobol.com.br/abend_01.htm#A13)
[<br>        ABEND CODE         B37](http://www.cadcobol.com.br/abend_01.htm#B37)
[<br>        ABEND CODE         D37](http://www.cadcobol.com.br/abend_01.htm#D37)
[<br>        ABEND CODE         E37](http://www.cadcobol.com.br/abend_01.htm#E37) 



**Introdução**

A interpretação do sistema operacional da IBM a respeito de codigos de erros e mensagens podem ser tediosas e frustrantes. 
Muitas vezes os manuais apropriados não estão prontamente disponíveis para o acesso do usuário. 
Se os manuais estiverem disponíveis, a descrição do erro e o procedimento de correção são, freqüentemente, de dificil interpretação. 
Uma lista dos erros comumente encontrada no CIS, Departamento de Apoio Técnico, com uma breve descrição compreensível do significado deles/delas e um procedimento sugerido por corrigir o erro é determinada abaixo. 











------







**Introdução** 

A interpretação do sistema operacional da IBM a respeito de codigos de erros e mensagens podem ser tediosas e frustrantes. Muitas vezes os manuais apropriados não estão prontamente disponíveis para o acesso do usuário. Se os manuais estiverem disponíveis, a descrição do erro e o procedimento de correção são, freqüentemente, de dificil interpretação. Uma lista dos erros comumente encontrada no CIS, Departamento de Apoio Técnico, com uma breve descrição compreensível do significado deles/delas e um procedimento sugerido por corrigir o erro é determinada abaixo. 



**Identificando o código de erro**

 Identificar o código de erro é o primeiro passo no processo. 

A primeira página ou páginas geradas como output por um job é um log JES3 ou um dataset de JESMSG. 

Este é uma listagem cronológica que especifica JES3 e mensagens do sistema operacional usadas durante o processamento do job. 

Se seu abended (término anormal), uma mensagem no fim do JESMSG aparecerá, e se assemelhar a:hh.mm.ss SYS2 R=IEF450I jobname procname stepname-ABEND Snnn Ummmm           TIME=hh.mm.ssOs carácteres "IEF450I " são um identificadores de mensagem que pode serem vistas na " IBM OS/VS Mensagem Biblioteca: VS2 Mensagens do Sistema " manual que tem uma descrição da mensagem. 

O jobname atual, nome de procedimento, e stepname para seu job aparecerão nos locais indicados na mensagem. O " Snnn " e " Ummmm " identificam as partes mais úteis da mensagem. O " Snnn " é um código que denota um abend do SISTEMA. Estes códigos podem ser achados na " IBM OS/VS Mensagem Biblioteca: VS2 Sistema Códigos ". 

O " Ummmm " é um código que denota um abend de USUÁRIO. Estes códigos podem ter variasões de um programa para outro, então estes não serão discutidos.Seguindo o joblog do JES3 deve ser um arquivo de impressão referenciado para um JESJCL.

Esta é uma lista que especifica JCL e qualquer declaração de controle de trabalho adicional de procedimentos incluídosA próxima seção de saída é referecniada para o dataset de SYSMSG. Dentro deste arquivo serão impressas todas as mensagens do sistema que incluirá uma mensagem mais descritiva associada com a mensagem de erro que se aparece em JESMSG. 

Bastante comumente, um código de erro tem vários significados, enquanto fazendo a informação extra assim nesta seção muito útil identificando o problema.  Por exemplo:IEC150I 913-38,IFG0194C,jobname,procname,ddname,35D,UGS004,dsname IEF472I jobname procname stepname - COMPLETION CODE - SYSTEM=913 USER=0000Os carácteres "IEC150I " são outros códigos de mensagens que podem serem vistos no manual de mensagens do sistema. 

À direita deste código é o código do abend do sistema. Neste exemplo é " 913 ". Os " -38 " são um número de código adicional ocasionalmente distinguia entre erros diferentes debaixo do mesmo código de abend do sistema.Os códigos de abend do sistemas abaixo, são os mais comuns.Códigos de ABEND mais comuns

<br>       

ABEND CODE         0131.

-  Identificação do erro:  IEC141I
2. Descrição:  O sistema não pode ABRIR um de seu datasets corretamente, geralmente por causa de um parâmetro incorreto de DCB (BLKSIZE), ou não pôde achar o membro especificado de um dataset particionado. 
3. Procedimento corretivo:Confira o BLKSIZE no parâmetro de DCB para assegurar que mesmo é o BLKSIZE do dataset. Verifique a ortografia e existência do membro do dataset particionado. 

<br>       

ABEND CODE         0C11. 

-  Identificação do erro:  Nenhuma 
2. Descrição:  O computador tentou executar uma instrução de máquina inválida e uma exceção de operação aconteceu. 
3. Procedimento corretivo:Confira a parte do overlaying de seu programa. Acidentalmente parte do overlaying de seu programa com dados está fora da área de alcance (subscript out of range) ou perdas de endereços produziram este erro.

ABEND CODE         0C41. <br>      

-  Identificação do erro:  Nenhuma 
2. Descrição:  Esta geralmente é uma violação de proteção de armazenamento causada por seu programa tentando armazenar dados em memória que não é alocada para seu uso. 
3. Procedimento corretivo:Tenha certeza de que qualquer subscrição (subscripts) usada não excede o limite especificado. Corrija todos os maus endereços de uma declaração store-type. <br>        

ABEND CODE         0C51.

-  Identificação do erro:  Nenhuma 
2. Descrição:  O computador tentou ENVIAR uma área para uma parte de memória não existente.
3. Procedimento corretivo:Confira para subscrições impróprias (subscripts) e para listas incompatíveis para sub-programas. <br>        

ABEND CODE         0C71. 

-  Identificação do erro:  nenhuma 
2. Descrição::  Este é um erro de exceção de nos dados apurados. O sistema tentou executar uma instrução que trabalha com números decimais e encontrou dados formatados incorretamente. 
Este erro acontece comumente em programas PL/I e COBOL ao trabalhar com dados que foram convertidos incorretamente depois de uma entrada de cartões ou algum outro arquivo ou quando campos numéricos declarados para conter dados decimais não são inicializado antes de uso.
DATA EXCEPTION. Normalmente e causado por erro na especificacao dos dados.
Basicamente ocorre quando as posicoes de sinal de um item decimal compactado ou as posicoes de digitos estao invalidas. Pode ser causado ainda por operacoes de atribuicao,comparacao, edicao com campos decimais lidos incorretamente ou pesquisa fora dos limites de tabela de valores decimais.  
* - Para evitar este erro, sempre teste a validade dos dados de entrada e atribua valor inicial aos campos da 'WORKING STORAGE'. Dados nao numericos em um campo numerico.Campo numerico na 'WORKING STORAGE' sem valor inicial.
Tentativa de mover um campo numerico invalido para campo de edicao.Tentativa de comparar um campo numérico inválido.Soma de campo sinalizado sobre um campo nao sinalizado ou mover dados 'DISPLAY', ou mover zeros para grupo ou item descrito como 'COMP' ou 'COMP-3'.
Indexador com valor menor do que (1).Estouro de indexador ultrapassando o limite maximo especificado na clausula.Tentativa de ter acesso ao 'BUFFER' antes de abrir o arquivo.Definicao incorreta da 'LINKAGE SECTION':9.1 - Passagem de parametros em ordem errada.9.2 - Omissao ou inclusao de parametro.9.3 - Nao inicializacao da clausula 'USAGE', se necessaria.9.4 - Não definição do tamanho exato.Omissao da palavra 'LINE(S)' na clausula 'PAGE LIMIT' dentro do 'REPORT WRITER' de cobol.Quando utilizar o 'PARM' a partir do comando 'EXEC' deve se ter o cuidado de usar o 'LINKAGE EDITOR (COBUCLG)' ao inves do 'LOADER(COBUCG)'. Neste caso o 'PARM' deve ser usado no primeiro comando da 'PROCEDURE DIVISION'; Caso contrario o endereco do 'PARM' sera alterado causando o processamento de dados nao determinados.3. Procedimento corretivo:Entre com os dados correto ou faça a conversão internamente no programa <br>        

ABEND CODE         1061. <br>     
 
-  Identificação do erro:  nenhuma 
2. Descrição::  Ocorreu um erro com um software do sistema ou problema de disco durante a execução de instrução LINK ou LOAD. 
3. Procedimento corretivo:Assegure que o pedido de carga no problema foi especificado corretamente e não foi modificado incorretamente, então resubmit o trabalho. <br>        

ABEND CODE         2131. <br>      

-  Identificação do erro:  IEC143I 
2. Descrição::  O sistema tentou abrir um data set DASD fixados e encontrou dificuldades. Este ABEND acontece quando o nome do dataset especificado no parâmetro do DSNAME não exista. 3. Procedimento corretivo:Se o dataset é catalogado, verifique se o nome do mesmo está correto. Se o dataset não é catalogado, assegura que o próprio volume foi especificado no parâmetro de VOL=SER. <br>        

ABEND CODE         2221. <br>      

-  Identificação do erro:  IEF301I 
2. Descrição::  O operador cancelou o job. 
3. Procedimento corretivo:Se nenhuma mensagem for determinada em JESMSG, contate o operador para uma explicação. <br>        

ABEND CODE         2F31. <br>      

-  Identificação do erro:  Nenhuma 
2. Descrição::  O job estava sendo executado quando ocorreu uma falha no sistema. 3. Procedimento corretivo:Resubmit o job, caso seu resultado for insatisfatorio, contate com a area de suporte um estudo mais apropriado. <br>        

ABEND CODE         3221. <br>      

-  Identificação do erro:  Nenhuma 
2. Descrição::  A execução de um job, job step ou um step de procedure catalogada levou mais tempo que o especificado (timeout). Se nenhum tempo foi especificado no parâmetro TIME do seu jobcard, o mesmo será determinado pelo valor default da instalação. 3. Procedimento corretivo:Confira os erros do programa, como loops infinitos. Corrija qualquer erro e execute o job novamente. Se nenhum erro foi achado, aumenta o tempo para a execução do mesmo e execute o job novamente. <br>        

ABEND CODE         6131. <br>      

-  Identificação do erro:  IEC147I 
2. Descrição::  Um erro de input/output (I/O) aconteceu durante execução de uma instrução OPEN para um dataset em fita magnética. O resultado do erro está entre uma leitura ou gravação de fita magnética , ou o mau posicionando da mesma. Este erro acontece tipicamente em processo de arquivos em fita magnéticas de multi-arquivos. 3. Procedimento corretivo:Execute o job novamente depois de verificar que o equipamento foi devidamente consertado. 

<br>        

ABEND CODE         7221. <br>      

-  Identificação do erro:  Nenhuma 
2. Descrição::  O sistema cancelou o seu job porque o limite de linhas para ser impressa foi excedido (SYSOUT). 3. Procedimento corretivo:Assumindo que o programa está correto, aumente a especificação apropriada por uso. Se fossem excedidas linhas (default=5000), o parâmetro de LINHAS (em milhares) deverá ser aumentado adequadamente. <br>  

ABEND CODE         8041. <br>      

-  Identificação do erro:  Nenhuma 
2.  Descrição::  Seu job requer mais armazenamento virtual (memória) do que esta disponível no momento. 
3.  Procedimento corretivo:Aumente o parâmetro REGION no cartão de EXEC do step que abendou. Se nenhum parâmetro de REGION foi especificado, o valor default para o procedimento que é executado foi assumido.

ABEND CODE         8061. <br>      

-  Identificação do erro:  Nenhuma 
2. Descrição::  Este erro aconteceu durante execução de um LINK ou instrução de LOAD. O sistema não pôde localizar um módulo de carga. 
3. Procedimento corretivo:Tenha certeza de que o nome do módulo de carga ou o nome do programa esteja correto ou que o STEPLIB apropriado ou JOBLIB no cartão de DD, que define qual biblioteca reside o módulo de carga, esteja incluído no seu JCL. <br>        

ABEND CODE         80A1. <br>      

-  Identificação do erro:  Nenhuma 
2. Descrição::  Este erro é complemento do código de abend 804, discutido acima. 
3. Procedimento corretivo:Os mesmos procedimentos devem ser exercitados para este erro 

ABEND CODE         8131. <br>      

-  Identificação do erro:  IEC149I 
2. Descrição::  Durante a execução de uma instrução OPEN para um dataset em fita magnética, o nome do mesmo no header da fita não é igual ao informado no cartão de DD. 
3. Procedimento corretivo:Assegure que a declaração DD especifica o DSNAME correto, número de série do volume e etiqueta para a fita acessada. 

ABEND CODE         9131. <br>      

-  Identificação do erro:  IEC150I 
2. Descrição::  Uma instrução OPEN foi usada para um dataset RACF protegido em um volume de DASD que seu userid não foi autorizado para ter acesso. RACF só lhe permite ter acesso a datasets com um alto nivel de qualificação igual a seu userid ou o qual você foi explicitamente determinada permissão de  acesso pelo dono do dataset. 
3. Procedimento corretivo:Tenha certeza você tem a autoridade de acesso precisada ao dataset. Deveria ser prestada atenção à publicação " RACF, A Component of the IBM Operating System of The University of Georgia ". Este é um manual de informação geral breve especificamente publicado para usuários de IBM na Universidade. Pode ser obtido ao Departamento de Apoio Técnico.

ABEND CODE         A131. <br>      

-  Identificação do erro:  IEC151I 
2. Descrição::  O sistema tentou um OPEN em um dataset não existente em fita magnética. O sistema encontrou a marca de fim de volume para o arquivo você especificou no parâmetro de LABEL no cartão DD. 
3. Procedimento corretivo: Confira o número sequencial do arquivo e número de série do volume do job que criou o dataset.

ABEND CODE         B371. <br>      

-  Identificação do erro:  IEC030I 
2. Descrição::  Este erro resulta se qualquer uma da situações acontecer. Primeiramente, se o volume de DASD para o qual o sistema nomeou um do datasets de produção do programa não tem espaço bastante disponível para permitir fazer as distribuições secundárias necessárias. Secundariamente, este
ABEND pode ocorrer se o dataset de produção usar todas as 16 extensões de distribuições secundárias mas ainda requereram mais espaço. 
3. Procedimento corretivo:Calcule o espaço requerido para o dataset de produção antes de re-executar seu programa. 
Se possível, diminua a quantia de espaço pedida ou se mais espaço é necessario incrementar a primeira e/ou segunda alocação. 

ABEND CODE         D371. <br>      
-  Identificação do erro:  IEC031I 
2. Descrição::  Um dataset de saida usou todo o espaço primário alocado e nenhum espaço secundário foi pedido. 
3. Procedimento corretivo:Aumente a area primária ou acrescente uma area secundária ao parâmetro especial para aquele dataset de saida.

ABEND CODE         E371. <br>     
-  Identificação do erro:  IEC032I 
2. Descrição::  Se criando um dataset em fita, todo o espaço disponível no volume especificado sera usado e o sistema tentou gravar outro registro. Se criando um dataset dividido em acesso direto, 16 extensões de espaço secundário serão usados quando o programa tentou gravar outro registro. 3. Procedimento corretivo:Especifique mais um volume de fita pelo menos ou especifique espaço mais primário criando-se um dataset dividido. 

|      | ![Volta a página anterior](http://www.cadcobol.com.br/botao_02.gif) | [![Volta ao Menu Principal](http://www.cadcobol.com.br/botao_03.gif)](http://www.cadcobol.com.br/menuprin.htm) |
| ---- | ------------------------------------------------------------ | ------------------------------------------------------------ |
|      |                                                              |                                                              |