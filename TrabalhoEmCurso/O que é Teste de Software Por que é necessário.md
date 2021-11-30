# O que é Teste de Software? Por que é necessário?

19/10/2020 • 4 min. de leitura

![Avatar de Guilherme Wergutz Muller](https://secure.gravatar.com/avatar/54f3d7aa2f416fa58c88a043e69a3f41?s=300&d=mm&r=g)

Guilherme Wergutz MullerAutor

------

Nem sempre o que é “óbvio” para um, é “óbvio” para outro, não é mesmo?!

Neste sentido, escrevo esta publicação com um objetivo simples: apresentar de forma consistente, resumida e estruturada em tópicos, pontos relevantes sobre “O que é teste de software e por que ele é necessário dentro do ciclo de desenvolvimento de sistemas, seja ele ágil ou não”.

Este conteúdo direciona-se a todos os profissionais experientes (ou não) das áreas relacionadas ao desenvolvimento e teste de software, que desejam reciclar seus conhecimentos sobre testes e, também, a todos aqueles que desejam conhecer mais sobre este mundo. A base desta escrita é o manual de estudos para certificação CTFL de teste de software do ISTQB (2018br) — International Software Testing Qualifications Board.

![Image for post](https://miro.medium.com/max/402/1*uuS5Kz8p7IoQe46lk0108w.png)Foto: https://blog.onedaytesting.com.br/teste-de-software/

## O que é teste de software?

- O teste de software é uma maneira de avaliar a qualidade da aplicação e reduzir o risco de falha em operação.
- Testar não consiste apenas em executar testes (executar o software e verificar os resultados). **Executar** testes é apenas umas das atividades.
- Planejamento, análise, modelagem e implementação dos testes, relatórios de progresso, resultado e avaliação da qualidade, também são partes de um **processo de testes**.

*Testar software não é somente* **verificar** *se os requisitos foram atendidos ou se as estórias de usuário (User Stories), bem como demais especificações, foram contempladas. Atribui-se ao teste de software também a* **validação***, ou seja, verificar se o sistema atenderá às necessidades do usuário e de outras partes interessadas em seu(s) ambiente(s) operacional(is).*

### Podemos dividir os testes em duas categorias: dinâmico e estático.

O teste **dinâmico** refere-se à execução de um componente ou sistema. Já os demais, que não envolvem a execução do componente ou sistema, são conhecidos como testes **estáticos**. Para cada uma destas categorias existem inúmeros tipos de processos, mas neste momento não irei entrar neste assunto. Lembrando que estou seguindo a linha apresentada pelo Syllabus.

#### São vários os objetivos de se testar um software, independente do projeto. O Syllabus destaca os seguintes:

- Avaliar os produtos de trabalho (requisitos, estórias de usuário, modelagem e código);
- Verificar se todos os requisitos especificados foram atendidos;
- Validar se o objeto de teste está completo e funciona como os usuários e outras partes interessadas esperam;
- Criar confiança no nível de qualidade do objeto de teste;
- Evitar defeitos;
- Encontrar falhas e defeitos;
- Fornecer informações suficientes às partes interessadas para permitir que elas tomem decisões, especialmente em relação ao nível de qualidade do objeto de teste;
- Reduzir o nível de risco de qualidade de software inadequada (ex.:, falhas não detectadas anteriormente que ocorrem em produção);
- Cumprir com requisitos ou normas contratuais, legais ou regulamentares, e/ou verificar o cumprimento do objeto de teste com tais requisitos ou normas.

## Testar software não é depurá-lo.

As atividades não são sinônimas. O que ocorre é que em alguns casos, os testadores são responsáveis pelo teste inicial e pelo teste de confirmação final, enquanto os desenvolvedores fazem a depuração e o teste do componente associado. Há ainda os contextos ágeis, onde os testadores podem ser envolvidos na depuração e no teste de componente. Em resumo, há uma diferenciação para **TESTE** e **DEPURAÇÃO**:

***Teste →\*** *A execução dos testes pode mostrar falhas causadas por defeitos no software.**
**
****Depuração →\*** *Atividade de desenvolvimento que localiza, analisa e corrige esses defeitos.*

## Por que o teste é necessário?

- Para reduzir o risco de falhas durante a operação. Isso se dá a partir de testes rigorosos de componentes e sistemas, além do uso de documentação adequada;
- Para contribuir com a qualidade dos componentes ou sistemas. Isso se dá a partir da detecção e correção de defeitos;
- Para atender aos requisitos contratuais/legais ou aos padrões específicos do setor a que se destinam;

## Contribuições para o sucesso

Envolver o papel do testador durante todo o ciclo de desenvolvimento do software pode aumentar as chances de sucesso nos projetos. Sabendo disso, o Syllabus exemplifica alguns cenários, os quais separo em **ETAPA** – momento do ciclo onde sugere-se o envolvimento do teste, **BENEFÍCIO** – contribuições do teste na referida etapa e **JUSTIFICATIVA** – ganhos ao inserir o teste na etapa.

![img](https://lh3.googleusercontent.com/UVp90rU3OPoGdHWGK6H0aJZ7Cz2axrrHRotQaUi6JbwFMoyg17vO-jr9OPGcU80es9NWGr0CWgJJITgr-NrgUqc14i-RI1xf6yxgtTdPbsGCbDuOZMZeLBp1s0w2VWViPhcu5TO5)

### BUG, DEFEITO e FALHA


Uma pessoa pode cometer um erro (engano), que pode levar à introdução de um defeito no código do software ou em algum outro produto de trabalho relacionado.

- Um erro que leva à introdução de um defeito em um produto de trabalho pode acionar outro erro que leva à introdução de um defeito em um outro produto de trabalho relacionado.

***Exemplo:\*** *uma* ***pessoa\*** *levanta um requisito de forma incompleta, ambígua, incorreta. Caracteriza-se um erro. O* ***projeto\*** *de software daquele requisito é realizado de forma incorreta. Caracteriza-se um* ***defeito\****. O* ***desenvolvedor\*** *cria um código incorreto a partir de um projeto incorreto/errado. Caracteriza-se um* ***erro\****. O* ***software\*** *gerado apresentará* ***defeito\*** *devido ao código incorreto.*

- A execução de um código defeituoso, pode causar uma falha, mas não necessariamente em todas as circunstâncias.

***Exemplo:\*** *bug do milênio, que ocorreu em uma circunstância específica.*

- Nem todos os resultados de testes inesperados são falhas. Podem ocorrer **falsos positivos** (relatos de defeitos que não são defeitos) ou também **falsos negativos** (testes que não detectam defeitos que deveriam ser detectados).
- **Falsos positivos** podem ocorrer devido a erros na forma como os testes foram executados ou devido a defeito nos dados, no ambiente ou em outro tesware (produtos de teste) ou por outros motivos.

![http://www.galitezi.com.br/2012/02/conceito-erro-defeito-e-falha.html](https://miro.medium.com/max/443/1*icF-0Anwg2rgQeRTXEnq-A.jpeg)Foto: http://www.galitezi.com.br/2012/02/conceito-erro-defeito-e-falha.html

C*omo coloquei no início desta publicação, acredito muito que não exista o óbvio, principalmente quando falamos de saberes. Nem tudo que é óbvio para mim, é óbvio para você. Em outras palavras, mesmo que para profissionais da área alguns dos conceitos apresentados anteriormente pareçam ser básicos, para outros pode ser novidade, ou então, já tinham lido a respeito mas não lembravam e buscam uma reciclagem para recapitular pontos importantes. De qualquer forma, a disseminação de conhecimento sempre é válida, do básico ao avançado, ele deve ser repassado.*

**[CTFL Foundation](https://www.bstqb.org.br/node/197)**