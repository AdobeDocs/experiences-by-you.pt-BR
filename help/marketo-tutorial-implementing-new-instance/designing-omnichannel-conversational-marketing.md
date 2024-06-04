---
title: Criar marketing conversacional omnicanal com o Dynamic Chat
description: Comece rapidamente a criar marketing de conversação com o Adobe Dynamic Chat, o canal nativo de engajamento conversacional no Adobe Marketo Engage. Este tutorial oferece receitas acionáveis para implementar casos de uso, como reservas de reuniões de vendas, engajamento no conteúdo do site e promoção de eventos/webinários.
role: Admin
level: Beginner
doc-type: Article
duration: 0
last-substantial-update: 2024-05-23T00:00:00Z
jira: KT-14814
source-git-commit: 4ac24e1297287adbd6832030fda5590b696e45ed
workflow-type: tm+mt
source-wordcount: '1409'
ht-degree: 0%

---


# Criar marketing conversacional omnicanal com o Dynamic Chat

Profissionais de marketing, seu site é essencial para gerar leads, impulsionar conversões e acelerar os ciclos de vendas. O envolvimento com visitantes em tempo real em seu site permite que sua equipe de vendas qualifique compradores com mais eficiência. o Adobe Dynamic Chat, o canal de chat nativo na sua assinatura do Adobe Marketo Engage, permite que você automatize conversas para estender os recursos do Marketo Engage.

Este tutorial descreve o processo de reflexão e os casos de uso principais compartilhados por Sara Barriuso, gerente de operações de marketing da Cornerstone OnDemand, durante o evento &quot;Aprenda com seus colegas&quot;. Ela explicou como sua organização usou o Dynamic Chat para maximizar as capacidades de Marketo Engage.

## Integração do engajamento conversacional à sua estratégia de geração de demanda

Os visitantes navegam pelo site por um motivo. Eles podem estar buscando conteúdo em seus produtos ou serviços ou procurando informações de contato para falar com seus representantes de vendas. Eles também podem ser seus clientes que procuram informações adicionais sobre o produto. O chat permite que os visitantes do site se autoatendam e se autoqualifiquem se estiverem prontos para falar com a equipe de vendas.

Quando Sara Barriuso implementou o Dynamic Chat, ela se sentiu atraída por sua integração perfeita com o Marketo Engage e o [acionadores de atividade pré-criados](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/dynamic-chat-activities){target="_blank"} que ativam programas Marketo Engage e vice-versa. Ela desenvolveu suas estratégias de engajamento conversacional com três segmentos de público-alvo em mente:

1. Prospetos desconhecidos: ofereça chamadas de demonstração de forma proativa para gerar novos leads.
2. Clientes potenciais conhecidos: aumente o tempo gasto pelos visitantes ao navegar pelo conteúdo e ofereça chamadas de demonstração para gerar oportunidades de venda adicional e venda cruzada.
3. Clientes atuais/potenciais: forneça experiências personalizadas estendendo os esforços de campanhas de marketing.


## Principais casos de uso para começar a criar suas caixas de diálogo

Para implementar essas estratégias, Sara criou seus diálogos de Dynamic Chat sobre os seguintes casos de uso:

1. Caixa de diálogo padrão para capturar tudo: forneça uma opção inicial a todos os visitantes, orientando-os a realizar suas tarefas com mais eficiência.

2. Promover o registro de eventos e webinários: incentive os visitantes do site a se registrarem em eventos e webinários para direcioná-los para o estágio de compra mais rapidamente.

3. Estender o engajamento do conteúdo da campanha: ofereça contexto adicional ou aborde possíveis perguntas quando os visitantes navegarem pelo conteúdo no site.

Vamos ver esses casos de uso em ação, à medida que Sara exibe seu processo, desde o mapeamento do fluxo de conversação até a configuração das Caixas de diálogo e o direcionamento no Dynamic Chat e no Marketo Engage.

### Caso de uso 1: caixa de diálogo padrão &quot;pega tudo&quot; para todos os visitantes do site

Essa caixa de diálogo fornece cinco opções iniciais para os visitantes do site escolherem entre elas, criando uma experiência autoguiada que os ajuda a encontrar as informações necessárias com base em sua persona. Para começar, você pode explorar sua caixa de entrada de email &quot;Fale conosco&quot; para identificar temas comuns e categorizá-los em opções de caixa de diálogo que se aplicam aos visitantes do site. Assista à demonstração e siga as etapas abaixo para criar sua caixa de diálogo catch-all padrão:

>[!VIDEO](https://video.tv.adobe.com/v/3429194/?learn=on)

>[!BEGINTABS]

>[!TAB Dynamic Chat]

#### Fase 1

1. Crie a caixa de diálogo e crie um link de teste.
2. Adicione uma meta para rastrear as conversões (por exemplo, envio de solicitação de demonstração).
3. Peça a duas ou três pessoas que testem e coletem feedback.

#### Fase 2

1. Em &quot;Público-alvo&quot;, adicione um URL da página da Web em &quot;Público-alvo&quot; para indicar onde a caixa de diálogo será exibida.
2. Em &quot;Configurações&quot;, adicione o nome da campanha, a descrição, a prioridade e o idioma.
3. Clique em &quot;Publicar&quot;

>[!TAB Marketo Engage]

#### Fase 1

1. Crie a Campanha inteligente de rastreamento.
2. Em &quot;Smart List&quot;, use um acionador &quot;Atinge a meta da caixa de diálogo&quot;. Use a mesma meta (por exemplo, Solicitação de demonstração) que você usou a caixa de diálogo
3. Em &quot;Fluxo&quot;, inclua uma etapa &quot;Alterar status do programa&quot; para rastrear a conversão.
4. A fonte será exibida como &#39;dynamicChat&#39;. Você pode criar uma Campanha inteligente para atualizar a origem para um nome que faça sentido para você.

#### Fase 2

1. Teste novamente o rastreamento da Campanha inteligente quando ela estiver ativa.

>[!ENDTABS]

#### Nível superior: marketing baseado em conta

Você pode aprimorar ainda mais a caixa de diálogo abrangente padrão incorporando conteúdo direcionado para o setor, tornando as conversas ainda mais úteis para os visitantes. Por exemplo, sugira whitepapers específicos do setor ou estudos de caso para seus visitantes baixarem. Assista à demonstração e siga as etapas abaixo para criar uma caixa de diálogo abrangente padrão para marketing baseado em conta:

>[!VIDEO](https://video.tv.adobe.com/v/3429195/?learn=on)

>[!BEGINTABS]

>[!TAB Dynamic Chat]

1. Clonar a &quot;caixa de diálogo padrão&quot; e renomeá-la.
2. Em &quot;Stream Designer&quot;, adapte as mensagens de diálogo ao setor de destino (apenas um fluxo + a pergunta inicial).
3. Peça a duas ou três pessoas que testem a caixa de diálogo e coletem feedback.
4. Crie um link de teste e compartilhe-o.
5. Em &quot;Público-alvo&quot;, adicione um URL da página da Web onde a caixa de diálogo exibirá e atualizará o público-alvo para o setor desejado.
6. Em &quot;Configurações&quot;, adicione o nome da campanha, a prioridade da descrição e o idioma.
7. Clique em Publicar.

>[!TAB Marketo Engage]

1. Crie o Campaign inteligente de rastreamento e teste a meta.
2. Teste novamente o rastreamento da Campanha inteligente após a publicação da caixa de diálogo.

>[!ENDTABS]

### Caso de uso 2: Promover o registro de eventos e webinários

Eventos e webinários são táticas de marketing populares para empresas B2B gerarem demanda. Eles oferecem experiências envolventes e informações avançadas que atraem clientes em potencial. Conectar os visitantes do seu site a eventos e webinários futuros permite qualificar clientes em potencial com ainda mais rapidez. A criação dessa caixa de diálogo é de baixo esforço e custo, e pode demonstrar rapidamente o sucesso, ajudando você a obter suporte das partes interessadas de marketing para adicionar envolvimento conversacional ao seu plano de automação omnicanal. Assista à demonstração e siga as etapas abaixo para criar sua caixa de diálogo de promoção de evento/webinário:

>[!VIDEO](https://video.tv.adobe.com/v/3429196/?learn=on)

>[!BEGINTABS]

>[!TAB Dynamic Chat]

#### Fase 1

Crie um modelo para a caixa de diálogo &quot;Registro de evento&quot; para uso contínuo da campanha.

#### Fase 2

1. Clonar o modelo.
2. Copiar e colar texto na mensagem de diálogo para um novo evento
3. Atualize os parâmetros de UTM usados no link do evento (por exemplo, utm_medium=website&amp;utm_source=adobe).
4. Crie um link de teste, clique em &quot;Publicar&quot; e compartilhe-o com o solicitante.
5. Exame pelos pares e aplicação de feedback.


>[!TAB Marketo Engage]

#### Fase 1

1. Crie seu rastreamento de Campanha inteligente no modelo de webinário/programa de evento e teste-o.

#### Fase 2

1. Adicione o nome da campanha ao rastreamento da Campanha inteligente no Marketo Engage e teste-a.

>[!ENDTABS]


#### Nível superior: Registrar pessoas conhecidas

Você pode oferecer uma experiência ainda melhor aos visitantes do site, registrando-os em seus eventos e webinários, sem que eles precisem preencher um formulário. Experiências personalizadas geram confiança e mostram aos visitantes que você se lembra delas. Vamos ver como elevar o nível da caixa de diálogo de promoção de evento e webinário em ação.

>[!NOTE]
>Considere o potencial risco de segurança envolvido em determinados estados/países de proteção e implemente essa personalização com cuidado, consultando sua equipe jurídica.

>[!VIDEO](https://video.tv.adobe.com/v/3429197/?learn=on)

>[!BEGINTABS]

>[!TAB Dynamic Chat]

1. Clonar a caixa de diálogo de promoção de Evento/Webinar.
2. No Stream Designer, depois que o usuário responder &quot;Sim&quot;, adicione um cartão de pergunta &quot;Você compartilhou anteriormente seu endereço de email conosco. Você gostaria de guardar isso para os detalhes do evento?&quot;
3. Se a resposta for &quot;Sim&quot;, adicione um cartão de mensagem &quot;Você receberá um email de confirmação no seu email com os detalhes do evento/webinário&quot;.
4. Se eles responderem &quot;Não&quot;, adicione uma mensagem de cartão &quot;Preencha o formulário na página de registro&quot;.
5. Crie um link de teste, clique em &quot;Publicar&quot; e compartilhe-o com o solicitante.
6. Na guia Público-alvo, adicione [o email não está vazio].

>[!TAB Marketo Engage]

1. Adicione essa nova caixa de diálogo ao rastreamento do Campaign inteligente no Marketo Engage e teste-a.

>[!ENDTABS]

### Caso de uso 3: Extensão do engajamento no conteúdo da campanha

Imagine uma janela cativante que chama sua atenção e o atrai para uma loja. Se um recepcionista o ajudar a selecionar produtos ou responder suas perguntas, você pode se sentir mais confortável em fazer uma compra. Para replicar essa experiência online, você pode ter sua caixa de diálogo Dynamic Chat exibida nas páginas da Web onde suas campanhas de marketing direcionam os visitantes. Conforme os usuários se envolvem com o conteúdo da Web, o Dynamic Chat exibe imediatamente conversas relevantes, sugerindo conteúdo adicional ou abordando possíveis perguntas. Isso é feito aproveitando acionadores de automação para ativar campanhas de Dynamic Chat com base no engajamento do usuário nos programas de Marketo Engage. Agora, vamos ver como dar vida a esse caso de uso.

>[!VIDEO](https://video.tv.adobe.com/v/3429199/?learn=on)

Estender o envolvimento com o conteúdo do Campaign - Configuração:

>[!VIDEO](https://video.tv.adobe.com/v/3429200/?learn=on)

>[!BEGINTABS]

>[!TAB Dynamic Chat]

1. Gere novos clientes em potencial para suas campanhas por email e pontos de contato de campanhas sociais. Neste exemplo, a pesquisa Talent health index é hospedada no site da marca.
2. Clonar um modelo de caixa de diálogo existente (por exemplo, caixa de diálogo padrão &quot;catch-all&quot;) para criar três caixas de diálogo para os seguintes cenários e atualizar o &quot;URL de destino&quot; na guia &quot;Público-alvo&quot; adequadamente:
   * Quando os visitantes da Web vinham dos seus canais de marketing e chegavam à sua página da Web.
   * Na página de agradecimento
   * Qualquer visitante que retorne ao seu site dentro de 45 dias após se envolver na campanha de marketing (redirecionamento)

>[!ENDTABS]

## O que está por vir?

* Mapear o fluxo de conversação no [Designer de fluxo](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/automated-chat/stream-designer){target="_blank"} ou um fluxograma offline.
* Criar uma caixa de diálogo padrão catch-all no Dynamic Chat.
* Ative os diálogos após o engajamento da campanha usando acionadores de automação no Marketo Engage.


## Autores

{{sara-barriuso}}

{{amy-chiu}}