---
title: Criação de uma cultura de dados e uma referência de design de solução melhor
description: Revolucione sua estratégia de dados e capacite sua equipe a criar um documento sólido de Referência de design de solução (SDR). Eliminar lacunas de medição e promover uma cultura de dados colaborativa por meio de metodologias passo a passo.
feature: Implementation Basics
topic: Administration
role: User
level: Experienced
doc-type: Article
duration: 72000
last-substantial-update: 2024-04-25T00:00:00Z
jira: KT-15338
thumbnail: KT-15338.jpeg
source-git-commit: 07b28edade263aa3c85348716bd45df4a053e239
workflow-type: tm+mt
source-wordcount: '1640'
ht-degree: 0%

---


# Criação de uma cultura de dados e uma referência de design de solução melhor

**Revolucione sua estratégia de dados e capacite sua equipe a criar um documento sólido de referência de design de solução (SDR). Eliminar lacunas de medição e promover uma cultura de dados colaborativa por meio de metodologias passo a passo.**

É finalmente hora. Você reúne uma Referência de design de solução (SDR) sólida. Este é o guia que você usa para implementar suas métricas e dimensões, como são chamadas, quando são disparadas e seus devotos adoraram. Você passou por todo o processo de implantação, escrevendo critérios de aceitação, examinando seus pontos de acesso, fazendo o controle de qualidade de tudo, e está pronto! Foi muito trabalho, e agora está feito. Sua instância do Adobe Analytics deve estar aumentando e diminuindo o marketing e o produto à medida que eles analisam os dados, obtêm novas revelações sobre seus clientes e encontram todas as áreas de sucesso e, bem, áreas de menos sucesso. Mas não está ouvindo os elogios que esperava.

De um acampamento, você ouve reclamações.

&quot;Por que não consigo descobrir a taxa de conversão nesse funil?&quot;

&quot;Por que não há uma métrica para isso?&quot;

&quot;Eu preciso de muito mais detalhes sobre isso! Uma métrica por si só não é suficiente. São necessárias pelo menos três dimensões diferentes para entender o desempenho. Por que você não as colocou?&quot;

Mas é o outro campo que é uma causa ainda maior de preocupação. Deles, você não ouve nada. Mas muito pior, você vê gráficos que foram claramente retirados de sua antiga solução de análise, aquele que não está mais sendo mantido, e cada dia está caindo cada vez mais em um pântano de decrepitude e dados sujos. Um sentimento de pavor o enche quando você pensa sobre as decisões que podem ser tomadas com essa bagunça.

O que deu errado? Por que existem lacunas na medição? Por que os membros da sua equipe não estão adotando isso?

Começarei por deixá-lo fora do gancho um pouco. Há *sempre* será uma revisão. Se o seu site ou aplicativo for complexo o suficiente para precisar de uma solução de análise corporativa, você não perderá nada. Mas não o suficiente para explicar as falhas de medição de que estou falando aqui. O que deu errado foi muito mais difícil de ser colocado em uma planilha. Você perdeu suas primeiras chances de criar uma cultura de dados colaborativa ao mesmo tempo em que criou seu SDR. Quero apresentar um método que eu e meus colegas desenvolvemos para criar um SDR melhor com menos lacunas e para fazer com que os usuários finais investissem e até mesmo ocasionalmente entusiasmados com sua nova instância do Adobe Analytics. Vamos analisar os shows e os porquês.

**O Como**

***A Conferência de medição:***

1. Reúna as partes interessadas, pessoalmente ou virtualmente, com o objetivo de descobrir o que medir. Isso deve incluir alguns executivos.
1. Você já tem alguns exemplos óbvios no painel de notas adesivas: coisas como receita, vendas ou leads, os KPIs mais importantes que você sabe serão medidos. Repita com dimensões, itens como estado conectado, categorias de produto ou termos de pesquisa.
1. Faça com que todos adicionem suas próprias notas adesivas, agrupando conforme necessário
1. Faça as pessoas votarem naquelas que elas acham que são importantes. Esses votos são ilimitados, pois talvez todas essas métricas e dimensões sejam importantes.
1. Para os que tiverem votos baixos, peça às partes interessadas que os pediram que explicassem para que vão usá-los. Se houver um bom caso de uso, guarde-o. Se há uma maneira melhor de obter esses dados, eles não podem explicar como é acionável, ou há outra boa razão para deixá-los de fora, tachá-los do painel.
1. Adicione essas métricas e dimensões ao seu SDR para uma análise inicial pelas partes interessadas que estavam presentes

***O mapa de funil***

1. Obtenha uma visualização de todos os funis, passo a passo, com cada estado incluído
1. Com os designers e gerentes de produtos, confira cada etapa e fale sobre o que eles consideram ser um sucesso nesse funil. É a taxa de conversão? Ele está escolhendo um caminho específico? Ele está usando determinados recursos?
1. Faça perguntas sobre quais métricas e dimensões são necessárias para entender o desempenho do funil em cada etapa do funil e em geral.
1. Acima de cada etapa do funil, adicione as métricas e dimensões que serão medidas nessa etapa, incluindo as métricas calculadas.
1. No início de cada funil, escreva os relatórios que serão inseridos no painel que o gerente de produto usará para rastrear o desempenho, coisas como um relatório de fallout, o mês atual e as taxas de conversão de tendência e qualquer coisa mais específica para esse funil.
1. Adicione as novas métricas e dimensões descobertas ao SDR e envie-o aos participantes para uma segunda revisão.

***Os Painéis de Visualização***

1. Usando o Mapa de funil como guia, crie painéis de modelo.
1. Deve haver uma visão geral, como um Painel de resumo executivo e painéis para cada um dos funis.
1. Também haverá alguns mais específicos para seu site ou aplicativo, como desempenho do produto ou desempenho do conteúdo.
1. Distribua isso aos participantes relevantes e obtenha feedback sobre o design.
1. Faça as atualizações solicitadas e, se novas métricas ou dimensões forem necessárias, adicione-as ao seu SDR.
1. Envie os painéis de visualização atualizados e o SDR para uma revisão final.

***Ferramentas de democratização de dados***

1. Criar um dicionário de dados. O SDR é para os seus devs. O dicionário de dados é para os usuários finais. Torne-os legíveis para os usuários finais para que eles possam pesquisar facilmente quais dados estão disponíveis e saber como usá-los. Seus usuários finais devem ser os aprovadores finais disso.
1. Anotações. Em cada organização, há certas datas que importam a cada ano e outras que aparecerão. Certifique-se de coletar os relevantes das partes interessadas e adicioná-los como anotações para aumentar a compreensão dos dados que eles veem.
1. Curadoria. Se o SDR for grande, pode ser avassalador. A paralisia da escolha não se aplica apenas aos seus clientes. Veja o que é importante para cada grupo de usuários e prepare os elementos que eles verão.

**O porquê**

***Para obter requisitos***

Essa é uma evidência, mas há outras maneiras eficazes de obter requisitos. Eu pessoalmente usei um em um entrevistas, questionários e revisões de relatórios existentes. Elas funcionarão, embora eu pense que não tão bem quanto os métodos que acabei de descrever. Sinceramente, não acho que a lacuna na coleta de requerimentos seja tão grande assim. O método que descrevi vai te levar até 95% do caminho, e esses outros métodos vão te levar até 90% do caminho. Então, qual é o grande por quê?

***Para construir a cultura de dados***

Com esse processo, você:

- Spark reflete bem como medir o sucesso
- Crie um senso de propriedade em suas partes interessadas
- Facilitar a compreensão dos dados pelas partes interessadas

***Suscitando uma profunda reflexão sobre os dados***

Para muitas das pessoas na sua empresa, os dados são algo que consomem. Eles usam. Eles o analisam. Eles não pensam profundamente sobre isso. Alguns deles herdaram relatórios e processos de seus antecessores que não foram alterados por causa da necessidade de continuidade. Eles nunca precisaram pensar sobre o porquê dos dados.

Esse processo lhes dá uma oportunidade de *compreender* dados. Fazendo as perguntas, o que é sucesso? Como você saberia se fosse bem-sucedido? Como você saberia o que mudar se não fosse bem-sucedido? Esse é um exercício que deve ser feito no início da criação de cada site, aplicativo e produto, mas com muita frequência não é. Ao fazer essas perguntas, você ajuda a aprofundar a compreensão deles não apenas dos dados, mas também do próprio produto.

***Criação de um senso de propriedade sobre os dados***

Isso não é algo que foi transmitido do alto. Não foi uma reunião de trinta minutos há três meses. Isso não é o questionário irritante que eles foram perseguidos por uma semana para responder e que eles fizeram isso com pressa, porque eles tinham uma demonstração para chegar para que eles pudessem fazer a data de lançamento sprint. Isso é o produto de seu pensamento profundo e seu trabalho com você e seus colegas, o que eles pesquisaram várias vezes, forneceram feedback contínuo, e que eles aprovaram depois que esse feedback foi incorporado. É deles! O fato de que é útil se deve a eles. É *seus* e foi o processo que os tornou seus.

***Facilitando a compreensão dos dados***

Você também mostrou a eles como eles irão usá-lo e como ele será por meio dos painéis de visualização. Qualquer nova solução é *rígido*. Há muito a aprender e dada a tremenda personalização do Adobe Analytics, a curva de aprendizado pode ser bastante acentuada. Você removeu 80% disso. Mesmo antes da primeira linha de código ser escrita, as partes interessadas sabem como os painéis serão. Eles saberão como lê-los e obter significado deles. Eles vão saber como o sucesso se parece literalmente porque eles falaram sobre quais métricas e dimensões definem o sucesso, e vocês falaram para eles como isso será visualizado. A entrega dos painéis de controle reais é uma tarefa de atualização e não uma nova tarefa de aprendizado assustadora.

Esta não é a maneira mais rápida de obter um SDR juntos. É muito trabalho e requer muita coordenação de horários, especialmente porque é vital que você tenha alguns executivos na combinação. No final, uma solução de análise corporativa é um enorme investimento de tempo e dinheiro, e você deseja garantir que a adoção e a satisfação sejam altas. Esse método leva a um longo caminho para fazer isso acontecer.

**Autor**

Este documento foi escrito por:

![gitai-headshot](assets/gitai-headshot-150.jpg)

Gitai Ben-Ammi, gerente associado de arquitetura de negócios da Accenture

Especialista no Adobe Analytics

