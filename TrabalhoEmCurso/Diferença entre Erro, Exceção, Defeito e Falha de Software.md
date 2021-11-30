![Controle de versão de Softwares utilizando o GitHub](https://i0.wp.com/dfilitto.com.br/wp-content/uploads/2019/07/Controle-de-vers%C3%A3o-de-Softwares-utilizando-o-GitHub.jpg?fit=990%2C557&ssl=1)

![img](https://secure.gravatar.com/avatar/96b0cf816922260d5cefaf274a072e27?s=80&d=mm&r=g)[Danilo Filitto](https://dfilitto.com.br/author/danilo-filitto/)

197 Views

Share This!



Softwares podem apresentar diversos tipos de anomalias mais conhecidas como *bugs*. E a palavra *bug* é usada para generalizar um “erro”, “defeito” ou até mesmo “falha” de software sendo que cada uma dessas palavras tem um significado diferente e são designadas cuidadosamente a situações específicas.

## Diferença entre Erro, Exceção, Defeito e Falha de Software

## Erro (Error)

O Instituto de Engenheiros Eletricistas e Eletrônicos (IEEE) tem realizado vários esforços para padronizar a terminologia dentro do contexto de software. O padrão IEEE nº 610.12-1990 traz quatro definições sobre erro:

> **Definição 1**: a diferença entre um valor ou condição computada, observada ou medida e o valor ou condição verdadeira, especificada ou teoricamente correta.

> **Definição 2**: uma etapa, processo ou definição de dados incorreto.

> **Definição 3**: um resultado incorreto.

> **Definição 4**: uma ação humana que produz um resultado incorreto.

Das definições mencionadas, de forma comum a **definição 1** é atribuída à palavra “erro”. Um erro é a causa de um defeito (*fault* — as vezes traduzido também como “falta”, **definição 2**) e é causado por um engano (*mistake*, **definição 4**). Em palavras mais simples, um erro pode ser entendido como a diferença entre o resultado obtido e o resultado esperado, cuja causa tem por origem uma ação humana (engano).
Exemplo em código:

```
def soma(a, b):
    return a * b

print( soma(1, 2) )
```

Por engano do programador, o código acima produz uma saída incorreta que é diferente do resultado esperado. Ao executar a função soma(1, 2), o resultado é 2, em vez de 3. Esse erro gera um defeito no funcionamento do programa, causando uma falha. Caso fosse chamado soma(2, 2), o resultado seria 4 e o defeito não causaria uma falha. Note que um erro denota uma anomalia **interna** de um artefato de software.

- Engano: o programador trocou o símbolo **+** por *****
- Erro: o programa executará **a \* b** em vez de **a + b**
- Defeito: o programa multiplica as entradas em vez de somá-las
- Falha: o programa não conseguiu somar as duas entradas


“*Mistake*” também pode ser traduzida como erro, mas apenas pessoas cometem *mistake*. Máquinas cometem *error*.

O ato de identificar e corrigir erros em código é conhecido como **depuração**. Essa ação pode ser requerida, caso um **defeito** seja observado no universo do usuário. Testa-se um software para descobrir defeitos, mas depura-se para encontrar e corrigir erros.

## Defeito (Defect, Fault)

Com base no documento IEEE Std 1044-2009 (revisão do IEEE Std 1044-1993, do mesmo órgão responsável pelo estabelecimento de formatos e padrões importantes para a computação, engenharia elétrica e eletrônica):

> **Defeito (\*defect\*)**: uma imperfeição ou deficiência em um produto de trabalho em que o produto de trabalho não atende a seus requisitos ou especificações e precisa ser consertado ou substituído.

Em um sentido mais específico, um defeito (*fault*) é a manifestação de um erro em um software. Também é uma etapa, processo ou definição de dados incorreto que pode gerar uma falha.

![img](https://i0.wp.com/2.bp.blogspot.com/-Pb-w9gOiUzA/XNuFhFojzPI/AAAAAAAADNA/vTnFR5TpzEYd1SESLZKyNyfjH_oQ_KzIgCLcBGAs/s640/Autoci%25C3%25AAncia%2B-%2BDiferen%25C3%25A7a%2Bentre%2BErro%2BFalha%2Be%2BDefeito.png?w=1320&ssl=1)Padrão de Classificação IEEE para Anomalias de Software em Diagrama de Classe (Fonte: adaptação de IEEE Std 1044-2009)

Em uma passagem rápida sobre o diagrama, com recapitulação do que foi explicado sobre erro: um engano humano pode introduzir um erro no software. Erro é a diferença entre o resultado obtido e aquilo que se espera. A manifestação de um erro é conhecida como defeito. Um defeito pode gerar uma, muitas ou nenhuma falha. Falhas podem ou não acarretar problemas, mas problemas não fazem parte do escopo IEEE 1044.

Diferentemente do erro, um defeito denota a **percepção externa** de que um artefato de software não está trabalhando como deveria.

![img](https://i0.wp.com/4.bp.blogspot.com/-s48vbb77jDs/XNuY7dKGktI/AAAAAAAADNM/hEOAI-5c2KoL7E-wqFgyCtqWr7ZLFPaKACLcBGAs/s640/Autoci%25C3%25AAncia%2B-%2BCiclo%2Bde%2BVida%2Bdo%2BDefeito.png?w=1320&ssl=1)Ciclo de vida do defeito como Diagrama de Estado em UML
(Fonte: adaptação de IEEE Std 1044-2009)

A tratativa para defeitos se dá por meio de uma SCR (*Software Change Request* — Solicitação de Mudança de Software) para que o software volte a operar normalmente. Softwares que são capazes de operar propriamente mesmo com defeitos são chamados de “*Fault-tolerant*“, que em português é traduzido como “Tolerante a Falhas”. Mas em inglês não existe o termo “*Failure-tolerance*“, porque o que acontece é que *fault* pode ser traduzido também como falha, conforme o dicionário de Cambridge, WordReference e também o Google tradutor. Embora exista essa tradução, um software deve ser tolerante a defeitos e jamais a falhas.

## Falha (Failure)

A **definição 3** de erro se aplica à falha. É um resultado incorreto. O IEEE Std 1044-2009 traz também duas definições a respeito:

> **Definição A**: rescisão da capacidade de um produto executar uma função exigida ou sua incapacidade de executar dentro dos limites especificados anteriormente (adaptado da ISO/IEC 25000:2005).

> **Definição B**: um evento no qual um sistema ou componente do sistema não executa uma função necessária dentro dos limites especificados (adaptado da ISO/IEC 24765:2009).

Em outras palavras, um software falha quando não cumpre seu propósito.

**Exemplo 1**: um profissional de recursos humanos não consegue carregar os relatórios através do botão “Carregar Relatórios” do sistema, pois, nenhum dos relatórios é trazido.

**Exemplo 2**: o gerente do departamento de compras, ao buscar pelos documentos de compra do dia 14 de março, recebe os documentos de compra do dia 14 de fevereiro.
**Exemplo 3**:

```
def get_config(file_name):
    with open(file_name, 'r') as config:
        return config.readlines()

# O arquivo buscado foi renomeado por alguém para local.cfg
get_config('local_config.cfg')
```

Note que uma falha denota a **percepção externa** de uma anomalia que ocorreu no artefato de software. O **exemplo 1** ilustra muito bem a definição A ou B demonstrando que o software não foi capaz de atingir seu objetivo. O **exemplo 2** é semelhante, mas em vez do sistema não trazer um resultado, ele traz, porém, incorreto assim como descrito na definição 3 de erro. Por fim, no exemplo 3, o programa não consegue ler o arquivo de configuração exigido e falha em carregar as configurações esperadas. Relembre o diagrama de classes apresentado onde uma falha pode ter como causa zero ou um defeito. Este é um caso em que há zero defeitos no código, o arquivo apenas não existe, por isso foi gerado uma **exceção** (diferentemente do exemplo de erro em soma(a, b), onde não houve exceções) e o software falhou.

## Exceção (Exception)

Para finalizar, uma exceção é um evento que causa a suspensão da execução normal de um programa. Segundo o IEEE Std 610.12-1990, isso inclui exceção de endereçamento, exceção de dados, exceção de operação, exceção de overflow, exceção de proteção e exceção de underflow. É importante salientar que a ocorrência de uma exceção não implica diretamente em uma falha. Se a leitura do exemplo 3 fosse envolvida em um bloco de tratamento de exceções, seria possível obrigar o programa a ler um outro arquivo cópia que tivesse as mesmas configurações.

## Conclusão

Vimos como a Engenharia de Software é cuidadosa ao dar nomes. As definições aqui apresentadas foram com base nos documentos supracitados do IEEE. Em resumo, podemos dizer que:

- Um **engano** (*mistake*) é uma ação humana que produz um resultado incorreto, introduzindo um erro.
- Um **erro** (*error*) é a diferença entre um resultado obtido e um resultado esperado, podendo gerar um **defeito** (*fault*).
- Um **defeito** (*fault*) é a manifestação de um erro e pode acarretar uma falha.
- Uma **falha** (*failure*) é quando um software não cumpre seu objetivo, com ou sem exceção.
- Uma **exceção** (*exception*) é um evento que causa a suspensão da execução normal de um programa.

Ter essa diferenciação em mente é importante, porque auxilia na tarefa de teste, identificação e também documentação. Há padrões de classificação e documentação para falhas e defeitos. Para mais informações, consulte o material da bibliografia.
**Referência Bibliográfica**

IEEE Std 1044-2009, **IEEE Standard Classification of Software Anomalies**.

IEEE Std 610.12-1990, **IEEE Standard Glossary of Software Engineering**.

CAMBRIDGE DICTIONARY. **Dicionário Cambridge**: **tradução de inglês para português**. Disponível em <https://dictionary.cambridge.org/pt/dicionario/ingles-portugues/>. Acesso em 15 mai. 2019.

LEITE, J. C. S. P. **Erro, Defeito: Falta, Falha** -> **cuidado ao dar nomes!!**. Disponível em <https://jcspl.net/2006/08/20/erro-defeito-falta-falha-error-fault-failure/>. Acesso em 15 mai. 2019.

GOOGLE TRADUTOR. **Google Tradutor**. Disponível em <https://translate.google.com/>. Acesso em 15 mai. 2019.

WORDREFERENCE. **Dicionário Inglês-Português (Brasil)**. Disponível em <https://www.wordreference.com/enpt/>. Acesso em 15 mai. 2019.

**Fonte:** autociencia.blogspot.com