# FBI alerta sobre falha crítica em software usado por grandes empresas

Por [Dácio Castelo Branco](https://canaltech.com.br/equipe/dacio-castelo-branco/) | Editado por [Claudio Yuge](https://canaltech.com.br/equipe/claudio-yuge/) | 17 de Setembro de 2021 às 18h20

<iframe id="google_ads_iframe_/22189562696/retangulo_0" title="3rd party ad content" name="google_ads_iframe_/22189562696/retangulo_0" width="336" height="280" scrolling="no" marginwidth="0" marginheight="0" frameborder="0" role="region" aria-label="Advertisement" tabindex="0" sandbox="allow-forms allow-popups allow-popups-to-escape-sandbox allow-same-origin allow-scripts allow-top-navigation-by-user-activation" srcdoc="" data-google-container-id="3" data-load-complete="true" style="box-sizing: border-box; margin: 0px; padding: 0px; border: 0px; vertical-align: bottom;"></iframe>

O FBI, a Agência de Cibersegurança e Infraestrutura (CISA, na sigla em inglês) e o Comando Cibernético da Guarda da Costa Americana (CGCYBER) alertaram que, desde agosto, grupos criminosos estão usando uma falha encontrada em um software de gerenciamento de senhas para aplicar as chamadas Ameaças Persistentes Avançadas (APTs) — ciberataques prolongados que usam técnicas de invasão contínuas e sofisticadas para obter acesso a um sistema e permanecer dentro dele por um período.

- [Sequestros digitais aumentam em feriados e fins de semana, alerta FBI](https://canaltech.com.br/seguranca/sequestros-digitais-aumentam-em-feriados-e-fins-de-semana-alerta-fbi-194561/)
- [Conhecimento público geral sobre ciberataques ainda é baixo, confirma pesquisa](https://canaltech.com.br/seguranca/conhecimento-publico-geral-sobre-ciberataques-ainda-e-baixo-confirma-pesquisa-188542/)
- [Biden assina ordem executiva para combater ataques virtuais nos EUA](https://canaltech.com.br/seguranca/biden-assina-ordem-executiva-para-combater-ataques-virtuais-nos-eua-185034/)

O software explorado pelos bandidos é o [Zoho ManageEngine ADSelfService](https://www.manageengine.com/mobile/self-service-password/), usado por várias empresas de grande porte, como a [Apple](https://canaltech.com.br/empresa/apple/), [Intel](https://canaltech.com.br/empresa/intel/), [Nike](https://canaltech.com.br/empresa/nike-inc/), [PayPal](https://canaltech.com.br/empresa/paypal/) e HBO. Ele permite que usuários estejam conectados em contas de vários serviços a partir de apenas uma credencial.

A vulnerabilidade encontrada no programa, documentada como CVE-2021-40539, permite que invasores possam assumir o controle do sistema, executar códigos maliciosos e implementar *web shells* nele, comprometendo a segurança total dos dados de empresas que usam o software.

[Quer ficar por dentro das melhores notícias de tecnologia do dia? **Acesse e se inscreva no nosso novo canal no youtube, o Canaltech News.** Todos os dias um resumo das principais notícias do mundo tech para você!](https://canalte.ch/materia-ctnews)

*Web Shells* são interfaces de controle remoto que costumam ser usadas por invasores para implementar códigos maliciosos em sistemas, permitindo que eles observem e alterem configurações e dados das máquinas afetadas.

Segundo o comunicado conjunto das três agências, essa vulnerabilidade pode colocar em risco várias instituições acadêmicas e companhias de infraestrutura nos EUA que fazem uso do programa.

Ainda no alerta conjunto emitido pelas agências estadunidenses, a vulnerabilidade já foi explorada em alguns ataques. Nessas invasões, os criminosos implantaram *web shells* feitas em JavaServer Pages (JSP), conjunto de tecnologias usadas para criar páginas web dinâmicas, camufladas como certificados x509. A partir da brecha, os invasores se movem pela máquina por meio do software de gerenciamento empresarial Windows Management Instrumentation, realizando cópias de arquivos críticos de segurança e de bancos de dados.

## Como prevenir

Até agora, os grupos responsáveis pelos ataques tiveram como alvo setores de transporte, Tecnologia da Informação, indústria, comunicação, logística, infraestrutura, instituições acadêmicas e serviços de segurança. APT é o tipo de crime virtual cometido principalmente para espionagem industrial, com agentes maliciosos sendo implantado em sistemas para realizar cópia de documentos e arquivos sensíveis de empresas.

A [Zoho](https://www.zoho.com/pt-br/), em 6 de setembro, [lançou uma atualização](https://pitstop.manageengine.com/portal/en/community/topic/adselfservice-plus-6114-security-fix-release) para o Zoho ManageEngine ADSelfService que corrige a falha. Em um alerta de segurança emitido junto com o update, a empresa diz que não há provas que a vulnerabilidade foi usada.

O FBI, a CISA e o CGCYBER estão pedindo para que os usuários apliquem imediatamente a atualização; e que se certifiquem que o programa não está sendo acessado diretamente pela internet, além de que mudem as senhas se qualquer indicação de invasão for detectada.

Fonte: [Bleeping Computer](https://www.bleepingcomputer.com/news/security/fbi-and-cisa-warn-of-state-hackers-exploiting-critical-zoho-bug/), [ThreatPost](https://threatpost.com/cisa-fbi-state-backed-apts-exploit-critical-zoho-bug/174768/)