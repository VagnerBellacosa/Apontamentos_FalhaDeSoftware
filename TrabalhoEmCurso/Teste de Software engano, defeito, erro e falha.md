# Teste de Software: engano, defeito, erro e falha.

[![Romulo Martins](https://miro.medium.com/fit/c/56/56/2*6_37WbinS3aYi6BQkJQwsA.jpeg)](https://medium.com/@romuluxs?source=post_page-----ca4bd0a07c0b-----------------------------------)

[Romulo Martins](https://medium.com/@romuluxs?source=post_page-----ca4bd0a07c0b-----------------------------------) - [Jun 25, 2020·2 min read](https://medium.com/@romuluxs/qual-a-diferença-entre-engano-defeito-erro-e-falha-ca4bd0a07c0b?source=post_page-----ca4bd0a07c0b-----------------------------------)

A área de teste de software possui uma série de conceitos e uma vasta terminologia. Entender esses pontos é fundamental para um melhor entendimento de artigos e livros da área. Um desses conceitos que confunde muita gente é a distinção entre **engano**, **defeito**, **erro** e **falha**.

Vamos tentar entender melhor estes conceitos? Partiu!

Um **engano** é basicamente uma ação humana equivocada, por exemplo, um trecho de código incorreto que foi incluído no projeto de software, como um sinal que foi trocado em uma fórmula matemática ou um argumento lógico que era pra ser um *or* e foi escrito um *and* no lugar. Este trecho incorreto de código é um **defeito**, ou seja, uma instrução que pode gerar resultados inconsistentes com o esperado.

O **erro** é o que foi causado pelo defeito, por exemplo, ao inserir o número 6 em um método esperávamos o resultado 12 mas ele retornou 16.

A **falha** pode ser considerada como uma consequência do erro, por exemplo, suponha que aquele método que possui um cálculo defeituoso acaba fazendo com que um personagem de um jogo pule mais alto do que realmente deveria, logo não se comporta como deveria, ou formalmente podemos dizer que não teve a saída esperada do que foi especificado.

Talvez você esteja pensando “Ah meu deus, não entendi nada”. Calma, talvez o diagrama abaixo ajude a entender melhor:

![img](https://miro.medium.com/max/1400/0*-3jSXEvLyiHROefw)

fonte: https://edisciplinas.usp.br/pluginfile.php/1196441/mod_resource/content/1/Aula09_TesteSoftware_Parte1.pdf

Em outras palavras podemos dizer que um engano cometido por um programador pode introduzir um defeito no código do sistema, este defeito produz um erro interno e durante a execução do sistema, este erro pode propagar uma falha para o usuário. Para complementar acho que a figura abaixo resume bem estes conceitos.

![img](https://miro.medium.com/max/60/0*3jMEkLsXcpO34h__?q=20)

![img](https://miro.medium.com/max/537/0*3jMEkLsXcpO34h__)

fonte: https://testesw.wordpress.com/conceitos-basicos/

Bem, tentei apresentar aqui alguma das terminologias básicas do teste de software. Se tiverem dúvidas ou sugestões deixem nos comentários. Até mais!

# Referência

MALDONADO, José Carlos; BARBOSA, Ellen Francine; VINCENZI, Auri Marcelo; *et al.* Introdução ao teste de software (versão 2004–01). [S.l: s.n.], 2004.