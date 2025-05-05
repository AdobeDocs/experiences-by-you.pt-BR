---
title: Criação de cultura de dados e uma referência de design de solução melhor
description: Revolucione sua estratégia de dados e capacite sua equipe a criar um documento sólido de Referência de design de solução (SDR). Elimine falhas de medição e promova uma cultura colaborativa de dados por meio de metodologias passo a passo.
feature: Implementation Basics
topic: Administration
role: User
level: Experienced
doc-type: Article
duration: 72000
last-substantial-update: 2024-04-25T00:00:00Z
jira: KT-15338
thumbnail: KT-15338.jpeg
exl-id: 99fcf68f-5698-4270-9055-ab224e6323a1
source-git-commit: b2e05ff39e065691dda530ed17762a55cf2e6778
workflow-type: tm+mt
source-wordcount: '1647'
ht-degree: 0%

---

# Criação de uma cultura de dados e uma referência de design de solução melhor

_Revolucione sua estratégia de dados e capacite sua equipe a criar um documento sólido de Referência de Design de Solução (SDR). Elimine as lacunas de medição e promova uma cultura de dados colaborativa por meio de metodologias passo a passo._

É finalmente hora. Você junta um SDR sólido. Um SDR é o guia usado para implementar suas métricas e dimensões. Você definiu como eles são chamados quando são disparados e seus desenvolvedores adoram. Você passou por todo o processo de implantação, escreveu critérios de aceitação, passou pelos seus limites, testou e está pronto! Sua instância do [!DNL Adobe Analytics] deve celebrar as equipes de marketing e produtos enquanto analisam os dados, obtêm novas revelações sobre os clientes e encontram todas as áreas de sucesso e, bem, as áreas de menos sucesso. Mas não está ouvindo os elogios que esperava.

De uma equipe, você ouve reclamações como:

&quot;Por que não consigo descobrir a taxa de conversão nesse funil?&quot;

&quot;Por que não há uma métrica para isso?&quot;

&quot;Preciso de mais detalhes! Uma métrica por si só não é suficiente. Há pelo menos três dimensões diferentes que eu preciso para entender desempenho. Por que você não as colocou?&quot;

Mas é a outra equipe que é uma causa ainda maior de preocupação. Deles, você não ouve nada. Pior, você vê gráficos que foram claramente retirados de sua antiga solução de análise (aquele que não é mais mantido e todos os dias está caindo ainda mais em um pântano de decrepitude e dados sujos). Um sentimento de pavor o enche quando você considera as decisões que podem ser tomadas com essa bagunça original.

_O que deu errado?_

_Por que existem lacunas na medição?_

_Por que os membros da sua equipe não estão adotando este procedimento?_

Vou começar deixando você um pouco fora do gancho. Haverá _sempre_ alguma revisão. Se o site ou aplicativo for complexo o suficiente para precisar de uma solução de análise corporativa, você perderá algo. Mas neste caso, você não perdeu o suficiente para explicar as falhas de medição que estou descrevendo.

O que deu errado foi muito mais difícil de ser colocado em uma planilha. Basicamente, você perdeu sua primeira chance de criar uma cultura de dados colaborativa ao criar seu SDR.

Quero apresentar um método que meus colegas e eu desenvolvemos para criar um SDR melhor com menos intervalos e para fazer com que os usuários finais se interessem (e até mesmo ocasionalmente entusiasmados) pela nova instância do [!DNL Adobe Analytics]. Vamos analisar como e por que você deve considerar esse método.

## O How

_Saiba mais sobre a conferência de medição. Use um mapa de funil para visualizar cada etapa do plano. Crie painéis de modelos para revisar como um grupo. Criar um dicionário de dados para usuários._

### A conferência de medição

1. Reúna as partes interessadas, pessoalmente ou virtualmente, com o objetivo de descobrir o que medir. Essa reunião deve incluir alguns executivos.
1. Você já tem exemplos óbvios no fórum sobre notas adesivas, como receita, vendas ou leads; os KPIs (indicadores-chave de produto) que você sabe que serão medidos. Repita com dimensões como estado conectado, categorias de produto ou termos de pesquisa.
1. Peça a todos que adicionem suas próprias notas adesivas, agrupando conforme necessário.
1. Peça às pessoas para votarem naquelas que elas acham importantes. São votos ilimitados porque todas essas métricas e dimensões provavelmente importam.
1. Para qualquer métrica e dimensão com votos baixos, peça às partes interessadas que os solicitaram que expliquem por que esses componentes seriam usados. Se houver um bom caso de uso, mantenha esses componentes. Se houver uma maneira melhor de obter esses dados, se ninguém conseguir explicar como esses dados são acionáveis ou se houver outro bom motivo para remover as métricas e dimensões, faça isso.
1. Adicione essas métricas e dimensões ao seu SDR para uma revisão inicial pelas partes interessadas que estavam presentes.

### O mapa do funil

1. Obtenha uma visualização de todos os funis, passo a passo, com cada estado incluído.
1. Com os designers e gerentes de produtos, analise cada etapa e discuta o que todos consideram o sucesso nesse funil. É o índice de conversão? Ele está escolhendo um caminho específico? Ele está usando determinados recursos?
1. Faça perguntas sobre quais métricas e dimensões são necessárias para entender o desempenho do funil em cada etapa do funil e em geral.
1. Acima de cada etapa do funil, adicione as métricas e dimensões medidas nessa etapa, incluindo as métricas calculadas.
1. No início de cada funil, escreva os relatórios que vão no painel que o gerente de produto pode usar para rastrear o desempenho. Esses relatórios incluem um [relatório de fallout](https://experienceleague.adobe.com/pt-br/docs/analytics/analyze/analysis-workspace/visualizations/fallout/fallout-flow), [mês atual](https://experienceleague.adobe.com/pt-br/docs/analytics/analyze/analysis-workspace/components/calendar-date-ranges/custom-date-ranges), [taxas de conversão de tendência](https://experienceleague.adobe.com/pt-br/docs/analytics/analyze/analysis-workspace/visualizations/line) e qualquer coisa mais específica para esse funil.
1. Adicione as novas métricas e dimensões descobertas ao SDR e envie-o aos participantes para uma segunda revisão.

### Os painéis de visualização

1. Usando o mapa de funil como guia, crie painéis de modelo.
1. Deve haver uma exibição geral, como um [Painel de resumo executivo](driving-success-with-executive-summary-dashboards.md), e painéis para cada um dos funis.
1. Também haverá alguns mais específicos para seu site ou aplicativo, como desempenho do produto ou desempenho do conteúdo.
1. Distribua isso aos participantes relevantes e obtenha feedback sobre o design.
1. Faça as atualizações solicitadas e, se novas métricas ou dimensões forem necessárias, adicione-as ao seu SDR.
1. Envie os painéis de visualização atualizados e o SDR para uma revisão final.

### Ferramentas de democratização de dados

1. Crie um dicionário de dados. O SDR é para seus desenvolvedores, mas o dicionário de dados é para os usuários finais. Torne-o legível para que todos possam pesquisar facilmente quais dados estão disponíveis e saber como usá-los. Seus usuários finais devem ser os aprovadores finais disso.
1. Anotar. Em cada organização, há certas datas que importam a cada ano e outras que aparecerão. Colete as datas relevantes das partes interessadas e adicione-as como anotações para aumentar a compreensão dos dados que elas veem.
1. Preparar. Se o SDR for grande, pode ser avassalador. A paralisia da escolha não se aplica apenas aos seus clientes. Veja o que é importante para cada grupo de usuários e prepare os elementos que eles verão.

## O porquê

_Saiba mais sobre como reunir requisitos, criar uma cultura de dados, refletir profundamente sobre os dados, criar um sentimento de propriedade sobre os dados e simplificar os dados._

### Coletar requisitos

Coletar requisitos é óbvio, mas há várias maneiras eficazes de fazer isso. Já usei entrevistas individuais, questionários e revisões de relatórios existentes. Essas estratégias funcionam, mas não tão bem quanto os métodos que acabei de descrever. no entanto, não acho que a diferença entre os métodos de coleta de requisitos seja significativa. O método que descrevi leva você a 95% do caminho até lá, e esses outros métodos levam você a 90% do caminho.

Então, o que é _por quê_?

### Criar cultura de dados

Com esse processo, você:

* Spark reflete bem como medir o sucesso
* Crie um senso de propriedade em suas partes interessadas
* Facilitar a compreensão dos dados pelas partes interessadas

### Spark com uma reflexão profunda sobre os dados

Para muitas das pessoas na sua empresa, os dados são algo que consomem. Eles usam. Eles o analisam. Eles não pensam profundamente sobre isso. Algumas pessoas herdaram relatórios e processos de seus antecessores, mas não os alteraram por causa da continuidade. Talvez essas pessoas nunca precisaram pensar sobre o _por que_ dos dados.

Esse processo oferece a eles uma oportunidade de _compreender_ dados. Fazendo perguntas como: O que é sucesso? Como você saberia se fosse bem-sucedido? Como você saberia o que mudar se não fosse bem-sucedido? Essas perguntas precisam ser respondidas no início da criação de todos os sites, aplicativos e produtos — mas, com muita frequência, não são. Ao fazer essas perguntas, você ajuda a aprofundar a compreensão de uma pessoa não apenas dos dados, mas também de seu produto.

### Criar um senso de propriedade sobre os dados

Um senso de propriedade não é algo que uma pessoa adquira facilmente. Não foi encontrado na reunião de 30 minutos em que compareceram há 3 meses. Não é criado por isso um questionário irritante que eles responderam muito rapidamente por causa de outras questões de trabalho urgentes, como demonstrações e datas de lançamento sprint.

A propriedade é o produto do pensamento profundo de alguém e de seu trabalho com você e seus colegas. Foi por isso que eles olharam várias vezes, forneceram feedback contínuo e o que aprovaram depois que esse feedback foi incorporado. É deles! O fato de que é útil se deve a eles. São _os dados_ deles e foi esse processo que os tornou seus.

### Simplifique os dados

Você também mostrou a eles como usarão o processo e como ele será por meio dos [painéis de visualização](#the-preview-dashboards). Qualquer nova solução é _rígida_. Há muito a aprender e, dada a tremenda personalização do [!DNL Adobe Analytics], a curva de aprendizado pode ser íngreme. Você removeu 80% disso. Mesmo antes da primeira linha de código ser escrita, as partes interessadas sabem como os painéis serão. Eles saberão como lê-los e obter significado deles. Eles vão saber como o sucesso se parece literalmente porque eles falaram que métricas e dimensões definem o sucesso. E você contou a eles como esse sucesso será visualizado para eles. A entrega dos painéis de controle reais é uma tarefa de atualização e não uma nova tarefa de aprendizado assustadora.

Esta não é necessariamente a maneira mais rápida de obter um SDR juntos. É muito trabalho e requer muita coordenação de horários, especialmente porque é vital que você tenha alguns executivos na combinação. No final, no entanto, uma solução de análise corporativa é um enorme investimento de tempo e dinheiro, e você deseja garantir que a adoção e a satisfação sejam altas. Esse método leva a um longo caminho para fazer isso acontecer.

**Autor**

Este documento foi escrito por:

![gitai-headshot](assets/gitai-headshot-150.jpg)

Gitai Ben-Ammi, gerente associado de arquitetura de negócios da Accenture

[!DNL Adobe Analytics] Especialista
