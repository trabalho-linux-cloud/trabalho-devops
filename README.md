# Autores do trabalho
- Edivan Ludvig (edivanludvig@gmail.com)
- Paulo Both (pauloboth95@gmail.com) 

# Descrição do trabalho
Desenvolvimento de um pipeline com fluxos de CI/CD utilizando as ferramentas GithHub, CircleCI e Heroku para o aperfeiçoamento dos conhecimentos obtidos durante as aulas da disciplina de DevOps.

# Porque escolhemos essas ferramentas
## CircleCI
- É uma ferramenta gratuita com bastante margem para realização dos testes. No plano Free possui 2500 créditos por semana, em que os gastos são baseados no uso de uma máquina com 2 CPUs e 4GB de memória, assim a cada minuto em que a máquina está rodando são consumidos 10 créditos. Ao final de diversos testes durante uma semana foram gastos somente 30% dos créditos, o que permite realizar centenas de testes semanais.
- A ferramenta permite configurar os pipelines e acompanhar sua execução através de uma página web de fácil navegação e verificação dos logs.
- O build dos pipelines do CircleCI se iniciam automáticamente após a integração com a ferramenta GitHub, necessitando apenas fazer alguma alteração no branch configurado.
- A ferramenta suporta várias linguagens como C++, Javascript, .NET, PHP, Python, e Ruby.
## Heroku
- É uma ferramenta gratuita para realização de uma avaliação.
- Heroku possui um mercado de add-ons que pode facilitar o processo de desenvolvimento em caso de precisar de alguma ferramenta ou banco de dados.
- A ferramenta suporta várias linguagens como Node.js, Ruby, Python, Java, PHP, Go, Scala e Clojure.
- Possui uma documentação oficial bem completa para cada linguagem suportada.
- Possui um espaço privado para gerenciamento dos aplicativos.
- Identificação automática da linguagem da aplicação.

# Requisitos técnicos avaliados para escolha
- Tanto a ferramenta CircleCI como o Heroku  permitem a realização de todo o processo na nuvem, sem a dependência de instalação e criação de um ambiente para execução.
- São aplicações que não possuem um valor muito alto em planos pagos.
## CircleCI
- Compatível com AWS, Azure, Heroku, Docker e servidor exclusivo.
- Aplicação SaaS.
## Heroku
- Realiza um build rápido da aplicação e disponibiliza uma URL hospedada com SSL dentro do seu próprio domínio.
- Aplicação SaaS.

# Vantagem em relação a outras ferramentas
- Ambas as ferramentas possuem um plano gratuito para utilização e realização de uma avaliação.
## CircleCI
- Ferramenta Cloud, não exige instalação em um servidor dedicado.
- Permite a realização de SSH para acessar o contêiner e verificar problemas.
- Possui um sistema de notificações que pode ser implementado.
- Paralelização automática.
- Processo de configuração com Github simples.
## Heroku
- Permite paralelismo de até 16 nós.
- As aplicações são executadas isoladas em containers.
- Forte compatibilidade com Javascript.

# Instruções para testes
- A atual projeto se encontra disponível no link https://github.com/trabalho-linux-cloud/trabalho-devops em um repositório público.
- A alteração de algum arquivo neste repositório inicia a construção de um pipeline na aplicação CircleCI. As configurações do pipeline e das suas respectivas etapas estão em um arquivo no diretório /.circleci/config.yml.
- Todo o projeto se encontra na branch master.
- O pipeline é composto por quatro etapas: Build, Test, Publish e Deploy.
- A etapa Build prepara o ambiente para a execução das próximas etapas.
- A etapa Test faz alguns testes referentes à aplicação, como por exemplo verificar se a aplicação está disponível.
- A etapa Publish faz a atualização dos dados que estão no repositório GitHub para a aplicação dentro da plataforma Heroku.
- A etapa Deploy é a etapa de finalização em que a aplicação é atualizada. Este processo já ocorre dentro do próprio Heroku, ou seja, assim que é feito o push da aplicação para o repositório do Heroku, este já atualiza as alterações na aplicação em produção.
- O projeto do Heroku pode ser acessado pelo link https://trabalho-devops.herokuapp.com.


# Links em que foram baseados os estudos para o uso das ferramentas citadas
- https://bitbar.com/blog/top-continuous-integration-tools-for-devops
- https://hackernoon.com/continuous-integration-circleci-vs-travis-ci-vs-jenkins-41a1c2bd95f5
- https://comparisons.financesonline.com/jenkins-vs-salesforce-app-cloud-heroku-enterprise
- https://www.educba.com/jenkins-vs-circleci/
- https://knapsackpro.com/ci_comparisons/heroku-ci/vs/jenkins
- https://www.slant.co/versus/625/2477/~circleci_vs_jenkins
- https://circleci.com/docs/2.0/credits

