---
title: Desbloquear insights com histogramas; além das médias no [!DNL Analytics]
description: Descubra o impacto dos histogramas no Analytics para obter insights além das médias.
feature-set: Analytics
feature: Visualizations
role: User
level: Experienced
doc-type: Article
last-substantial-update: 2023-08-18T00:00:00Z
jira: KT-13833
thumbnail: KT-13833.jpeg
exl-id: 46a9dab2-17f8-435e-949c-45d4a60343f0
source-git-commit: 058d26bd99ab060df3633fb32f1232f534881ca4
workflow-type: tm+mt
source-wordcount: '1082'
ht-degree: 4%

---

# Desbloquear insights com histogramas: além das médias no [!DNL Analytics]

_Descubra o impacto dos histogramas no Analytics para obter insights além das médias. Os histogramas revelam padrões de dados no comportamento do cliente, no envolvimento do visitante, no desempenho técnico e em erros de formulário, permitindo insights mais profundos e decisões informadas no [!DNL Adobe] Espaço de trabalho._

Vamos pular direto. Você deveria estar usando [histogramas](https://experienceleague.adobe.com/docs/analytics/analyze/analysis-workspace/visualizations/histogram.html?lang=pt-BR). Vou explicar por que, mas quero responder sua primeira pergunta: O que diabos é um histograma? Entendi. Na maioria das vezes, quando você vê um monte de barras subindo, você pode pensar que é um gráfico de barras. Sim, os histogramas são parecidos, mas eu garanto que são diferentes. Um gráfico de barras compara as coisas, enquanto um histograma mostra a frequência com que uma variável ocorreu. Dê uma olhada. Aqui está um gráfico de barras:

![Gráfico de barras 1](assets/bar-chart-1.png)

Temos seis modelos, e podemos comparar a receita de cada modelo. Vemos que o modelo de Joanesburgo tem mais receitas, enquanto Berlim tem menos.

Agora, vejamos um histograma:

![Histograma 1](assets/histogram-1.png)

Na parte inferior do eixo x, temos o número de unidades compradas por cada cliente. A primeira barra representa a frequência com que um cliente comprou uma unidade, a segunda barra mostra quantos clientes compraram duas unidades e assim por diante, até clientes que compraram dez ou mais unidades.

Então, como isso é útil? Bem, vemos que a maioria das pessoas só compra uma unidade. Continua diminuindo até chegarmos a 5 unidades. Então ele decai novamente até chegarmos a dez unidades. Isso aponta para o fato de que os clientes realmente gostam de comprar em múltiplos de cinco, e talvez devêssemos oferecer preços especiais ou embalagens para aproveitar isso. Mas certamente há muitos outros usos também.

## Noções básicas sobre o engajamento do visitante

Se o site ou aplicativo depende de tráfego repetido, você quer saber quantos visitantes estão voltando e com que frequência. Um dos histogramas mais simples que você pode usar é descobrir quantos visitantes estão retornando mais de uma vez. À medida que você acompanha esse histograma ao longo do tempo, você pode ver seu progresso, como esperamos que as barras da direita fiquem mais altas e as da esquerda, mais curtas.

Talvez você queira manter as pessoas no site, lendo artigos. Um histograma que mostra quantos visitantes leem números diferentes de artigos forneceria informações sobre o nível de engajamento. Por que isso é útil? Digamos que a maioria dos visitantes leia um artigo e saia, mas alguns visitantes altamente engajados leem três artigos e saem. Essa é uma ótima informação! Agora você sabe que deve personalizar a página do primeiro e do terceiro artigos lidos com o objetivo de fazer com que os visitantes leiam mais um artigo.

## Noções básicas sobre o comportamento do cliente

O proprietário do produto para os registros dos pacientes de um sistema hospitalar pediu-me alguns dados. Havia seis regiões para escolher para obter seus registros médicos. Ela queria saber quantas pessoas estavam clicando em mais de um. Criei um histograma que mostrava quantos visitantes clicavam nas opções 1, 2, 3, 4, 5 ou 6. Isso pode parecer excessivo, mas mais da metade dos visitantes clicavam em pelo menos duas opções e 3,2% dos visitantes clicavam em todas as seis. Com aquele histograma à sua frente, ela saltou para a ação, reorganizou seu roteiro e simplificou as opções para duas. Isso tornou a experiência do paciente muito mais simples.

## Noções básicas sobre desempenho técnico

Se você configurar um histograma para quantos visitantes experimentam quantos erros técnicos, poderá obter uma excelente compreensão de como está o desempenho técnico do site. Muitos visitantes que enfrentam muitos erros técnicos são um sinal para começar a priorizar essas correções técnicas.

## Noções básicas sobre o desempenho do formulário

As mensagens de erro em um formulário são uma questão diferente. Esses são erros do visitante, não erros da sua parte. Mas você pode se beneficiar de um histograma que mostra quantos visitantes estão tendo quantos erros. Se você vir um histograma indicando que muitos visitantes estão enfrentando muitos erros, a culpa pode não ser deles. Isso seria uma ótima indicação de que seu formulário tem campos com nomes incorretos, instruções pouco claras ou talvez um design que oculta campos obrigatórios.

## Por que não uma métrica calculada?

Você pode perguntar, como isso difere de apenas ter uma métrica calculada? Ei, eu pareço uma boa métrica calculada. Eu acho que elas são ferramentas absolutamente essenciais para entender o desempenho do seu site. O problema para muitos dos casos de uso que listei, no entanto, é que uma média pode mostrar a você o tamanho do problema, mas obscurecer o escopo dele. Vamos analisar como os histogramas fornecem informações adicionais para alguns dos casos de uso acima:

- Engajamento do visitante - Se você tiver um número médio de histórias lidas de 1,2, a personalização do primeiro artigo é bastante evidente. Você vai sentir falta de outro grande grupo que sai depois de ler o terceiro artigo, que é o que o histograma deixa óbvio.

  ![Histograma 2](assets/histogram-2.png)

- Erros técnicos - Se você visse uma média de 8,7 erros por visitante, saberia que tinha um problema. O histograma pode mostrar que 97% dos visitantes experimentam um ou menos erros, mas alguns outliers estão aumentando a média. Você pode então decidir que não vale a pena dedicar muito tempo para melhorar a experiência para esse pequeno grupo de outliers.

  ![Histograma 3](assets/histogram-3.png)

- Erros de formulário - Se você tiver uma média de 3,6 mensagens de erro de formulário por visitante, isso é um indicador de um problema. Você pode ter o mesmo problema atípico dos erros técnicos, mas também há informações a serem obtidas ao ver um pico no histograma em um número específico de erros. Um grande pico em um erro? Isso pode ser um problema comum que todos esses visitantes experimentam ou talvez todos tenham um erro diferente uma vez. Um pico gigante com três erros? Ah, agora isso é interessante. Se isso solicitar uma investigação que mostre que são os mesmos três erros, você zerou os dados que fornecem uma compreensão de seus visitantes e ajudam a corrigir o que provavelmente é um grupo de problemas inter-relacionados.

  ![Histograma 4](assets/histogram-4.png)

Como você pode ver, os histogramas não só têm seus próprios usos, mas também aprofundam a compreensão que você obtém de uma média. Eles são uma visualização pronta para uso no [!DNL Adobe Analytics] e fácil de criar. Esperamos que esses casos de uso sejam úteis para você ou despertem alguma inspiração. Feliz visualização!

## Autor

Este documento foi escrito por:

![Gitai Ben-Ammi](assets/gitai-headshot.png)

**Gitai Ben-Ammi**, Consultor principal do Concentrix Catalyst

[!DNL Adobe Analytics] Campeão
