---
title: Diferenças entre o construtor de segmentos e os segmentos rápidos no Analysis Workspace
description: Os segmentos podem ser uma das ferramentas mais eficientes no kit de ferramentas de análise de dados. Saiba mais sobre as diferenças entre o uso do construtor de segmentos e de segmentos rápidos no Analysis Workspace para eficiência.
feature-set: Analytics
feature: Segmentation
role: User
level: Beginner
doc-type: article
kt: KT-13118
exl-id: baeaa90e-8cce-4ddd-b099-fecd266e410c
source-git-commit: 849ec510944d3299c3515fcecd5fc57d74c3fa26
workflow-type: tm+mt
source-wordcount: '1267'
ht-degree: 0%

---

# Diferenças entre o construtor de segmentos e os segmentos rápidos no Analysis Workspace

Os segmentos podem ser uma das ferramentas mais eficientes no kit de ferramentas de análise de dados. Saiba mais sobre as diferenças entre o uso do construtor de segmentos e de segmentos rápidos no Analysis Workspace para eficiência.

>[!TIP]
>
> Clique na imagem na parte inferior da página para baixar um lembrete útil sobre quando usar cada ferramenta no Analysis Workspace.

Os segmentos podem ser uma das ferramentas mais eficientes no kit de ferramentas de análise de dados. Quando quiser ver grupos específicos de tráfego, seções do site ou jornadas do cliente, usar segmentos pode ser uma ótima maneira de concentrar a análise em um subconjunto específico de tráfego do site. Provenientes de um ambiente de varejo, alguns dos segmentos mais úteis que fiz são para diferentes tipos de grupos de clientes, por exemplo, clientes novos comparados aos existentes, clientes conectados a uma conta comparados a convidados e assim por diante. Mas você também pode criá-los para diferentes seções do site, clientes que executam ações específicas ou qualquer outra coisa em que possa pensar!

**Há duas formas principais de criar segmentos:**

* Uso do construtor de segmentos no menu Componentes
* Utilização de segmentos rápidos na parte superior de um painel

Se você construir seu segmento usando o construtor de segmentos, é possível salvá-lo para reutilização em outros projetos. Essa é uma ótima maneira de poder se concentrar em grupos específicos de clientes, por exemplo, pessoas que visitam determinadas seções do site e depois fazem uma compra. Por outro lado, se você estiver fazendo uma análise exploratória e quiser testar diferentes configurações de segmento, o construtor de segmentos rápido pode ser uma ótima ajuda. Vamos analisar alguns dos principais benefícios de cada método.

## Segmentos rápidos

Na parte superior de cada painel, você pode clicar no ícone de segmento rápido (um funil com o símbolo +) para abrir o construtor. Isso permitirá criar um segmento em qualquer nível (ocorrência, visita ou visitante) com até três condições. Semelhante ao construtor de segmentos principal, fornece uma indicação no lado direito que observa se o segmento está retornando dados e a porcentagem da população geral de tráfego incluída no segmento, embora seja uma versão mais simplificada do que a exibição completa do volume de segmentos exibida no construtor de segmentos. Ao adicionar mais de uma condição, é possível usar os operadores &quot;and&quot; e &quot;or&quot;. Infelizmente, não há opção &quot;então&quot; para segmentos rápidos, portanto, se você precisar de segmentos sequenciais, precisará usar o construtor de segmentos completo. Também há um limite de um contêiner em um segmento rápido. Já que ele realmente deve ser usado para segmentos básicos que podem ser criados e editados rapidamente. Depois que um segmento rápido é aplicado a um painel ou salvo, ele não pode mais ser editado no painel.

Ao fazer uma análise exploratória e testar diferentes tipos de segmentos para ver como diferentes grupos de clientes reagem ou como diferentes categorias se comportam, usar segmentos rápidos é muito mais rápido do que usar o construtor de segmentos. Além disso, esses segmentos só estão disponíveis no projeto em que foram criados, portanto, se não fornecer os resultados desejados, não será necessário se preocupar com a exclusão do segmento salvo da lista mestre. Se, depois de testar os segmentos, você perceber que ele será útil em outros projetos, sempre será possível clicar no botão &quot;abrir construtor&quot; para abrir o segmento no construtor de segmentos completo e salvá-lo como um segmento regular. No entanto, depois de fazer isso, não será mais possível editá-lo no construtor de segmentos rápido.

![Segmento rápido](assets/quick-segement.png)

## Construtor de segmentos

O construtor de segmentos pode ser acessado clicando no símbolo + acima da lista de segmentos no menu à esquerda de componentes, ou clicando na lista suspensa de componentes e selecionando &quot;Criar segmento...&quot;. Ao contrário dos segmentos rápidos, isso tem todas as opções disponíveis. Para adicionar várias condições, você pode criar segmentos sequenciais usando o operador &quot;then&quot;. Segmentos sequenciais também permitem usar &quot;grupo lógico&quot; como nível (em vez de ocorrência, visita ou visitante). O construtor de segmentos também permitirá que você adicione uma descrição aos segmentos, o que pode adicionar contexto sobre quem criou o segmento ou que tipo de dados foi criado para filtrar, ou até mesmo simplesmente adicionar &quot;tags&quot; ao segmento para fins organizacionais, que não são possíveis no construtor de segmentos rápido.

Se você precisar usar contêineres ou quiser segmentos sequenciais, é essencial usar o construtor de segmentos quando seu segmento tiver mais de três condições. O construtor de segmentos completo tem muito mais opções para criar segmentos mais complexos, o que pode ajudá-lo a analisar diferentes tipos de clientes, categorias, jornadas de clientes e assim por diante. Após criar e salvar esses segmentos, eles são adicionados à lista mestre de segmentos, o que significa que podem ser marcados, aprovados, compartilhados, usados em vários relatórios e publicados no Experience Cloud. A publicação no Experience Cloud permite que você utilize o segmento em outros produtos do [!DNL Adobe], como no [!DNL Adobe] Target para direcionamento de personalização. Os segmentos criados no construtor de segmentos não podem ser editados no painel segmentos rápidos. Será necessário abrir o construtor de segmentos para fazer alterações. Felizmente, a visualização de visualização à direita fornece uma análise mais detalhada do tráfego que o segmento traria nos últimos 90 dias, o que significa que é mais fácil garantir que o segmento esteja trazendo o que você deseja antes de salvar.

![Construtor de segmentos](assets/segment-builder-quick.png)

## Casos de uso

Em setores diferentes, seus usos para criar segmentos personalizados podem ser diferentes. Trabalhando para a divisão de comércio eletrônico de um grande varejista, geralmente realizamos análises exploratórias para determinar quais caminhos os clientes estão tomando para comprar. Quando vemos picos ou quedas em ações como adicionar produtos a carrinhos ou fazer pedidos, é aqui que o uso de segmentos rápidos pode ser útil. Durante uma análise, posso criar rapidamente um segmento para um tipo específico de cliente ou para uma ação/link específico no qual eles clicam. Não sendo necessário abrir o construtor de segmentos e salvar cada segmento, posso adicionar as condições rapidamente e removê-las da mesma maneira. Isso economiza muito tempo ao tentar explicar por que vemos uma mudança em nosso site.

Como alternativa, há ocasiões em que o construtor de segmentos foi meu local de destino. Nem todos os clientes são iguais e, muitas vezes, queremos observar tipos específicos de clientes identificados por ações ou caminhos que eles tomam. Ao usar o construtor de segmentos, podemos adicionar várias condições para identificar os diferentes tipos de clientes e salvar os segmentos para que eles possam ser compartilhados e usados por vários analistas. É importante que esses tipos de segmentos sejam consistentes em todos os relatórios, para que um criado para que todos possam usar seja melhor do que cada pessoa criando sua própria versão, pois os resultados podem ser diferentes.

Em geral, os segmentos rápidos e o construtor de segmentos são ferramentas excelentes para usar na análise. Cada um deles tem seus objetivos, benefícios e desvantagens. Certifique-se de verificar nossa útil planilha de dicas e truques disponível abaixo para obter um guia de referência rápido.

## Autor

Este documento foi escrito por:

![Mandy George](assets/mandy-george-2.png)

**Mandy George**, analista digital III da Best Buy no Canadá

Adobe Analytics Champion

## Baixar

[![Download de Segmentos Rápidos](assets/quick-segments-download-small.jpg)] (assets/[!DNL Adobe]_[!DNL Analytics]_&#x200B;Segments_Vs_Segment_Builder_Reference_Guide.pdf)
