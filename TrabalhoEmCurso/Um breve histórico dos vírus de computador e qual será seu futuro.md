# Um breve histórico dos vírus de computador e qual será seu futuro

![content/pt-br/images/repository/isc/2017-images/virus-img-10.jpg](https://www.kaspersky.com.br/content/pt-br/images/repository/isc/2017-images/virus-img-10.jpg)

Quando o assunto é cibersegurança, alguns termos são mais reconhecidos do que "vírus de computador". Apesar da predominância dessas ameaças e de seu amplo impacto, muitos usuários não conhecem a natureza básica dos vírus. Veja a seguir um breve histórico dos vírus de computador e qual será o futuro dessa ameaça cibernética tão difundida.

## A teoria dos autômatos que se autorreplicam

O que é vírus de computador? Essa ideia foi abordada pela primeira vez em uma série de palestras do matemático John von Neumann, no final dos anos de 1940, e em um artigo publicado em 1966, [Theory of Self-Reproducing Automata](http://cba.mit.edu/events/03.11.ASE/docs/VonNeumann.pdf), ou A teoria dos autômatos que se autorreproduzem. O artigo, na verdade, foi uma experiência teórica sobre a possibilidade de um organismo "mecânico", como um código de computador, danificar máquinas, se copiar e infectar novos hospedeiros da mesma forma que um vírus biológico.

## O programa Creeper

Conforme observado pela [Discovery](http://news.discovery.com/tech/first-computer-virus-creeper-was-no-bug-110316.htm), o programa Creeper, em muitos casos considerado o primeiro vírus, foi criado em 1971 por Bob Thomas da BBN. O Creeper foi, na verdade, criado como um teste de segurança para conferir se um programa era capaz de se replicar. E era — mais ou menos. Em cada novo disco rígido infectado, o Creeper tentava se remover do host anterior. O Creeper não tinha um objetivo malicioso e apenas exibia a mensagem: "I'M THE CREEPER. CATCH ME IF YOU CAN!"

## O vírus Rabbit

Segundo a [InfoCarnivore](http://infocarnivore.com/the-very-first-viruses-creeper-wabbit-and-brain/), o vírus Rabbit (ou Wabbit) foi desenvolvido em 1974, tinha objetivo malicioso e era capaz de se duplicar. Quando entrava em um computador, fazia diversas cópias de si mesmo, reduzindo muito o desempenho do sistema e chegando até a travar a máquina. Foi por sua velocidade de replicação que ele ganhou esse nome.

## O primeiro cavalo de Troia

Chamado de ANIMAL, o primeiro cavalo de Troia (embora haja certa [polêmica](https://encyclopedia.kaspersky.com/knowledge/years-1970s/) sobre ele ser um cavalo de Troia ou apenas um outro vírus) foi desenvolvido pelo programador John Walker em 1975, segundo a [Fourmilab](http://www.fourmilab.ch/documents/univac/animal.html). Na época, eram populares os "programas de animais", que tentam adivinhar em qual animal o usuário está pensando em um jogo de 20 perguntas. A versão que Walker criou teve altíssima demanda e, para enviá-la aos amigos, era necessário gravar e transmitir fitas magnéticas. Para facilitar as coisas, Walker criou o PREVADE, que se instalava junto com o ANIMAL. Durante o jogo, o PREVADE examinava todos os diretórios do computador disponíveis ao usuário e depois fazia uma cópia do ANIMAL nos diretórios em que ele ainda não estava presente. Não havia um objetivo malicioso, mas o ANIMAL e o PREVADE se enquadravam na definição de cavalo de Troia: havia no ANIMAL um outro programa oculto que realizava ações sem a aprovação do usuário.

## O vírus do setor de inicialização Brain

O Brain, o primeiro vírus para PC, começou a infectar disquetes de 5,2" em 1986. Conforme relatos da [Securelist](https://encyclopedia.kaspersky.com/knowledge/years-1980s/), foi um trabalho de dois irmãos, Basit e Amjad Farooq Alvi, que tinham uma loja de computadores no Paquistão. Cansados dos clientes que faziam cópias ilegais de seus programas de software, eles desenvolveram o Brain, que substituía o setor de inicialização de um disquete por um vírus. O vírus, que também foi o primeiro vírus stealth, continha uma mensagem oculta de direitos autorais, mas não corrompia nenhum dado.

## O vírus LoveLetter

O surgimento de redes de banda larga confiáveis e velozes no início do século XXI mudou a maneira como os programas de malware eram transmitidos. Já não confinados a disquetes ou redes corporativas, os malwares conseguiam se propagar muito rapidamente por e-mail, sites populares ou até diretamente pela Internet. Consequentemente, os malwares modernos começaram a tomar forma. O cenário de ameaças se tornou um ambiente misto, compartilhado por vírus, worms e cavalos de Troia, por isso o nome "malware", um termo abrangente para software malicioso. Uma das epidemias mais graves dessa nova era foi a do LoveLetter, que apareceu em 4 de maio de 2000.

Conforme observado pela [Securelist](https://securelist.com/threats/2001/), ele seguia o padrão dos vírus de e-mail da época, mas, diferentemente dos vírus de macro que dominavam o cenário das ameaças desde 1995, ele não assumia a forma de um documento do Word infectado, mas sim de um arquivo VBS. Era simples e direto e, como os usuários não desconfiavam de e-mails não solicitados, funcionava. A linha de assunto era "I Love You" (Eu te amo), e cada e-mail continha um anexo, "LOVE-LETTER-FOR-YOU-TXT.vbs". O criador do ILOVEYOU, Onel de Guzman, projetou o worm para substituir arquivos existentes por cópias de si mesmo, que então eram usadas para propagar o worm para todos os contatos de e-mail das vítimas. Como a mensagem geralmente chegava na caixa de entrada das novas vítimas enviada por um conhecido, elas abriam o arquivo, fazendo do ILOVEYOU uma prova de conceito pela eficiência em engenharia social.

## O vírus Code Red

O worm Code Red não continha um arquivo. Ele existia somente na memória e não tentava infectar arquivos do sistema. Aproveitando uma falha no Microsoft Internet Information Server, o worm de replicação rápida causava muita confusão com a manipulação dos protocolos que permitem a comunicação entre computadores e se propagava globalmente em algumas horas. Mais à frente, conforme observado pela [Scientific American](http://www.scientificamerican.com/article/code-red-worm-assault-on/), as máquinas afetadas foram usadas para iniciar ataques de negação de serviço distribuído (DDoS) sobre o site da Casa Branca, Whitehouse.gov.

## Heartbleed

Um dos vírus importantes mais recentes entrou em cena em 2014. O Heartbleed surgiu repentinamente e colocou em risco servidores em toda a Internet. O Heartbleed, diferentemente dos vírus ou worms, surgiu a partir de uma vulnerabilidade do OpenSSL, uma biblioteca criptográfica geral de código aberto usada por empresas do mundo todo. O OpenSSL envia "heartbeats" (pulsações) periodicamente para garantir que os endpoints seguros continuam conectados. Os usuários podem enviar ao OpenSSL uma quantidade específica de dados, depois solicitar o mesmo volume de volta. Por exemplo, um byte. Se os usuários alegarem que estão enviando o máximo permitido, 64 KB, mas enviarem somente um byte, o servidor responderá com os últimos 64 KB de dados armazenados na RAM, observa o tecnólogo de segurança [Bruce Schneier](https://www.schneier.com/blog/archives/2014/04/heartbleed.html), podendo incluir de tudo, desde nomes de usuários até senhas de chaves de criptografia.

## O futuro dos vírus de computador

Há mais de 60 anos, os vírus de computador fazem parte da consciência coletiva, mas o que antes era simples vandalismo cibernético acabou se transformando rapidamente em crime virtual. Os worms, cavalos de Troia e vírus estão evoluindo. Os hackers são inteligentes e entusiasmados, e estão sempre dispostos a superar os limites de conexão e do código para desenvolver novos métodos de infecção. O futuro do crime virtual parece envolver mais invasões a PDVs (pontos de venda) e, talvez, o recente cavalo de Troia de acesso remoto [Moker](https://threatpost.com/new-moker-rat-bypasses-detection/114948/) seja um bom exemplo do que está por vir. Esse malware recém-descoberto é difícil de detectar e de remover, e contorna todas as defesas conhecidas. Não existem certezas. A mudança é a alma dos ataques e das defesas.