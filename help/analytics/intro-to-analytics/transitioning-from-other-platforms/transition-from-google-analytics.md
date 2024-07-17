---
title: Guia abrangente para transição do  [!DNL Adobe Analytics] para o Google [!DNL Analytics]
description: Saiba mais sobre a localização de funcionalidade equivalente e como usá-la com eficiência na transição do Google [!DNL Analytics] para [!DNL Adobe Analytics]
solution: Analytics
feature: Third-party Integration
role: User
level: Beginner
kt: 9830
thumbnail: 34749.jpg
exl-id: 646bdc8f-c95e-40be-b2f7-8e4ba5653d91
source-git-commit: 02e3a6dfa59df45113242bd8e874e18e9e1efd58
workflow-type: tm+mt
source-wordcount: '3323'
ht-degree: 0%

---

# Guia abrangente para transição do [!DNL Analytics] para o [!DNL Adobe Analytics] da Google{#comprehensive-guide-for-transitioning-to-adobe-analytics}

## 1. Introdução

Um dos maiores desafios na transição entre quaisquer ferramentas é saber onde encontrar a funcionalidade equivalente e aprender a usá-la com eficiência. Esta discussão faz parte de um guia maior, cujo objetivo é ajudar os usuários a fazerem a transição para o [!DNL Adobe Analytics] (seja como um novo usuário ou como um usuário vindo do Google [!DNL Analytics]) com mais facilidade. Uma comparação aprofundada com o GA, que possivelmente é a ferramenta com a qual a maioria dos usuários está familiarizada, será fornecida para ajudar os usuários a correlacionar o conhecimento existente com o novo conjunto de ferramentas. Quando não há substituto para a prática, isso ajuda a começar e a reduzir as frustrações que você pode encontrar durante esse período.

Devemos fazer uma rápida comparação de terminologia:

| **Descrição** | **[!DNL Adobe Analytics]** | **Google[!DNL Analytics]** |
|--------------------------------------------------------------------------------------------------------------------------------|---------------------|----------------------|
| Uma métrica de evento que representa que uma página (ou tela em um aplicativo) foi visualizada | Exibição da página | Pageview |
| Uma métrica que representa um grupo de interações no site ou aplicativo que ocorrem no mesmo intervalo de tempo | Visite a | Session |
| Uma métrica que define um dispositivo identificado (com base em vários critérios, incluindo cookies e outros padrões de comportamento para unir informações do usuário) | Visitante único | Usuário(a)  |

## 2. As interfaces

Quando as pessoas comparam [!DNL Adobe Analytics] e Google [!DNL Analytics], elas comentam que a interface de [!DNL Adobe] é intimidadora no início. Isso é verdade, mas também é; acredite ou não; uma força, não uma fraqueza. O [!DNL Adobe] fornece uma grande variedade de ferramentas e flexibilidade na visualização de dados, permitindo que você tenha muito mais liberdade para criar o que precisa.

Vamos começar observando os relatórios &quot;no site&quot;.

### 2.1. Relatórios no local

#### 2.1.1. Tela inicial

O [!DNL Adobe Analytics] e o Google [!DNL Analytics] fornecem uma maneira de personalizar a primeira exibição que um usuário vê ao fazer logon.

##### 2.1.1.1. Workspace / Configuração personalizada da tela inicial ([!DNL Adobe Analytics])

[!DNL Adobe Analytics] não apresenta um relatório pré-construído para todos os usuários visualizarem ao fazer logon. A página inicial padrão leva o usuário para a tela inicial do Workspace, que mostra a cada usuário todos os relatórios do espaço de trabalho que ele criou ou que foram compartilhados com ele. Além disso, cada usuário pode definir qualquer um desses relatórios como sua tela inicial, se desejar.

![espaço-de-trabalho-criar-projeto](assets/ga-to-aa_1.png)

Detalhes sobre o espaço de trabalho serão apresentados mais adiante neste guia. Consulte a Seção 2.1.2.1

>[!TIP]
>
>Crie alguns relatórios padrão e compartilhe com os outros da sua organização para que eles tenham um ponto de partida e vejam as informações sem que precisem criar os próprios relatórios imediatamente.



##### 2.1.1.2. Insights da tela inicial (Google [!DNL Analytics])

* A Tela Inicial do Google [!DNL Analytics] tem algumas visualizações pré-construídas para você. Elas abrangem, por exemplo:
* Usuários, Sessões, Taxa de rejeição e Duração da sessão nos últimos sete dias
* Usuários por hora do dia nos últimos 30 dias
* Usuários atuais agora e Principais páginas ativas
* Canal de tráfego, Source/Medium e Referências nos últimos sete dias
* Sessões por país nos últimos sete dias
* Principais páginas dos últimos sete dias
* Tendência de usuários ativos nos últimos 30 dias
* e mais

No GA4, os usuários têm mais opções para personalizar e adicionar seus próprios relatórios à tela inicial.

![google-analytics-interfaces](assets/ga-to-aa_2.png)

Isso é provavelmente o que você mais sente falta em [!DNL Adobe Analytics]. Não há uma tela inicial pré-construída para você. No entanto, você pode configurar facilmente um Workspace personalizado para replicar o que precisa da lista acima e configurá-lo como sua tela de aterrissagem. Mais informações sobre isso serão apresentadas mais adiante (ou consulte a Seção 2.1.2.1 [!DNL Adobe] do Workspace).

#### 2.1.2. Report Builder no local

Além dos Relatórios simples fornecidos pelas ferramentas de análise, cada ferramenta fornece ferramentas mais eficientes para criar seus próprios relatórios personalizados.

##### 2.1.2.1. Workspace [!DNL Adobe Analytics]

Este é o carro-chefe do [!DNL Adobe Analytics]. Desde sua introdução em 2017, ele se tornou o local de referência para a análise de [!DNL Analytics] e o principal motivo pelo qual a seção Relatórios está prestes a ser encerrada.

Essa ferramenta permite criar relatórios com liberdade quase total.

O relatório pode ser dividido em painéis que podem conter diversas visualizações. Os painéis podem ser definidos como informações comuns, como intervalo de datas e filtros de segmento comuns.

Tanto os painéis quanto as visualizações dentro deles podem ser redimensionados e arrastados para mostrar os itens lado a lado ou empilhados. Assim, se você quiser comparar dois conjuntos de dados diferentes lado a lado, você pode criar painéis divididos ao meio, mostrando os dois sites lado a lado, para facilitar a comparação.

Há uma variedade de visualizações disponíveis para os usuários:

* Tabela de forma livre
* Tabela de coorte
* Fallout
* Fluxo
* Gráficos
   * Área (empilhada e não empilhada)
   * Linha
   * Dispersão
   * Barra (empilhada e não empilhada)
   * Marcador
   * Rosquinha
   * Histograma
   * Barra horizontal (empilhada e não empilhada)
* Mapa
* Blocos de resumo
   * Alteração de resumo
   * Texto de resumo
   * Texto (campo de texto livre para inserir informações extras para fornecer contexto)
* Venn

Cada painel e visualização podem ser intitulados e ter uma descrição aplicada para ajudar a contextualizar o que as informações estão mostrando.
No [!DNL Adobe], os segmentos (essencialmente filtros de dados) se aplicam retroativamente e podem ser colocados em colunas das tabelas de forma livre para comparar os dados lado a lado. Por exemplo, se um usuário quiser comparar duas categorias diferentes em seu site para tráfego, ele pode criar um segmento para a &quot;Categoria A&quot; e um segmento diferente para a &quot;Categoria B&quot;.

![analytics-page-views-report](assets/ga-to-aa_3.png)

As tabelas de forma livre permitem ter várias colunas e segmentação, conforme necessário, para visualizar os dados da maneira que você desejar.

Se não quiser ver um detalhamento por data, basta arrastar e soltar outra dimensão ou segmento para ver os dados de uma maneira diferente. Por exemplo, use segmentos para o Tipo de dispositivo e adicione um detalhamento por sistema operacional para seus usuários de dispositivo móvel/tablet:

![analytics-compare-page-views-report](assets/ga-to-aa_4.png)

O Workspace permite que sua criatividade flua, você não fica limitado a detalhamentos &quot;padrão&quot;. Você pode criar as visualizações necessárias para aprofundar as comparações que precisam ser executadas.

>[!TIP]
>
>Não tenha medo de experimentar e explorar. Há muitas maneiras de pensar fora da caixa. Além disso, validar o que você criou mostra a sua opinião. A experiência ajuda.

Você pode criar métricas calculadas dinamicamente ou segmentos que vivem somente dentro do relatório para evitar a inundação do segmento e do repositório de cálculos. Isso permite criar itens focados que são necessários para relatórios específicos sem confundir sua organização com itens que não podem ser usados em outros contextos.

Esta discussão é apenas uma introdução a esta ferramenta; há outros guias abrangentes para começar. Depois de revisar esses guias, você cria relatórios abrangentes como os seguintes:

![painel-do-espaço-de-trabalho](assets/ga-to-aa_5.png)

Os espaços de trabalho não são salvos automaticamente, portanto, é mais fácil criar um relatório ad-hoc único sem encher seu repositório de relatórios.

Outro recurso poderoso dos espaços de trabalho é a capacidade de aplicar modificadores interativos a seus relatórios na forma de menus suspensos. Esses menus suspensos não funcionam em arquivos CSV ou PDF exportados dos relatórios. No entanto, no relatório em tempo real, eles permitem atualizar todas as visualizações em um painel para mostrar o mesmo relatório em condições diferentes. Vários menus suspensos podem ser usados e, desde que as opções não sejam mutuamente exclusivas, os itens selecionados serão empilhados para apresentar informações de maneira clara.

>[!IMPORTANT]
>
>Para saber mais sobre o uso de menus suspensos e detalhamentos de forma livre, consulte <https://experienceleaguecommunities.adobe.com/t5/adobe-analytics-discussions/the-power-of-dropdown-filters-and-dimension-breakdowns-in-adobe/td-p/434680>

##### 2.1.2.2. Google [!DNL Analytics]: Painéis, Relatórios personalizados e Relatórios salvos

O Google tem algumas ferramentas para criar relatórios na interface, mas seguem a mesma exibição e limitações da seção de relatórios.

Ao ler isto, os versados em Google [!DNL Analytics] podem pensar: &quot;Mas o Google Data Studio não é um equivalente melhor em relação ao Workspace de [!DNL Adobe]?&quot; Sim, mas o Data Studio tecnicamente não faz parte da ferramenta [!DNL Analytics] e permite conexões com diferentes fontes de dados. Essa ferramenta é abordada posteriormente na seção &quot;Acesso estendido a relatórios&quot;, mais especificamente na Seção 2.2.3.

Os painéis do Google e os relatórios personalizados permitem reunir várias visualizações em um relatório, mas, diferentemente do Workspace, você ainda fica limitado a correlações simples e a quais dados podem ser colocados em quais colunas.

Nos relatórios personalizados, um dos maiores desafios é que, ao criar um filtro, ele se aplica a todas as guias do relatório. Não há uma maneira de comparar dois filtros diferentes no mesmo relatório.

Ele funciona para comparações simples. Todos são semelhantes aos [!DNL Adobe] Painéis Herdados, Relatórios Personalizados e Marcadores. Ferramentas básicas fornecidas para atender às suas necessidades, que estão no conjunto de relatórios.

#### 2.1.3. Relatórios

O Google e o [!DNL Adobe] têm alguns relatórios navegáveis que são tabelas pré-criadas e gráficos de linha do tempo básicos baseados em uma dimensão.

##### 2.1.3.1. Relatórios de [!DNL Adobe Analytics]

O [!DNL Adobe Analytics] também tem uma seção Relatórios, embora ela esteja sendo removida em favor do Analysis Workspace. Na verdade, o fim da vida útil foi anunciado para essa interface, já que o Workspace é uma ferramenta mais eficiente. A maioria dessas tabelas pode ser criada e modificada com mais facilidade. As seções de [!DNL Adobe] estão muito mais detalhadas, e isso pode ser assustador:

![métricas-site-de-análise](assets/ga-to-aa_6.png)

Com a maioria dos itens acima acessíveis por meio dos Espaços de Trabalho, ofereço uma breve visão geral dessas seções e como elas se relacionam com o Google [!DNL Analytics], destacando também os relatórios que ainda são relevantes.

Métricas do site é algo que já conhecemos. Abrange as métricas padrão (exibições de página, visitantes únicos, visitas e eventos personalizados que você configurou). Isso é semelhante ao Relatório de comportamentos do GA, mas também inclui parte do que você encontraria no Audience (já que o [!DNL Adobe] não divide os tipos de métrica).

Aqui, você encontra os relatórios de &quot;Bot&quot;. O tráfego de bots é excluído de todos os seus relatórios padrão. No entanto, há dois relatórios que fornecem insight sobre o que está acontecendo e quais bots estão chegando ao seu site. Isso é especialmente bom se você configurar Regras de bot personalizadas para excluir bots de spam conhecidos que acessam frequentemente seu site. Você pode obter alguns insights sobre o que esses bots estão fazendo sem que seus relatórios principais sejam inundados por esse tráfego. Os relatórios de bot estão indisponíveis no Workspace no momento (mas os novos recursos de relatório em breve também permitirão que os usuários obtenham essas informações lá).

O Conteúdo do Site é um agrupamento de [!DNL Adobe] dimensões padrão: Nome da Página, Seções do Site, Hierarquias, Servidores e muito mais. Todas essas dimensões estão disponíveis no Workspace.

Dispositivos móveis é um agrupamento de dados específicos de dispositivos móveis, incluindo dispositivos, tipos de dispositivos e muito mais. Eles estão disponíveis no Workspace.

Os caminhos não estão disponíveis no Workspace. O Workspace tem um diagrama de Fluxo em que você pode ver os fluxos de entrada e saída para uma única página/valor. Por outro lado, os Caminhos permitem que você veja os caminhos mais comuns usados no site. Por padrão, Páginas é o primeiro relatório de caminho configurado para você. No entanto, é possível ativá-lo para propriedades personalizadas, como um valor de &quot;Tipo de página&quot;. Você pode ver a definição de caminho dentro dos tipos de página. A outra coisa interessante em Caminhos é a maneira simples como as informações são apresentadas. O diagrama de fluxo no espaço de trabalho (dependendo da quantidade que você está tentando ver) pode ficar grande. Recomendo experimentar ambos. Cada um tem seu uso e valor, dependendo do que você está tentando alcançar. Observe que qualquer dimensão pode ser usada em Fluxos, enquanto a Definição de caminho deve ser configurada em uma propriedade no painel Administrador.

Os relatórios de Fontes de tráfego, [!DNL Campaign]s e Canais de marketing são semelhantes ao relatório de Aquisição no Google. As Fontes de Tráfego se concentram nos Referenciadores Reais, os [!DNL Campaign]s se concentram nos Códigos [!DNL Campaign] e os Canais de marketing também se concentram nos Códigos [!DNL Campaign], mas aplicam uma lógica extra, determinada por você, sobre como processar as informações. [!DNL Adobe] oferece mais liberdade sobre como configurar suas regras. Por outro lado, a Google faz várias coisas para você, e isso traz uma mudança de pensamento. Por padrão, a atribuição do Google para Códigos [!DNL Campaign] é de seis meses. Por padrão, a atribuição de [!DNL Adobe] está definida como uma semana. Isso pode ser alterado nas configurações de administrador, mas no Workspace é possível aplicar uma atribuição personalizada sobre qualquer dimensão, proporcionando muito mais flexibilidade &quot;instantânea&quot;.

Os relatórios de Retenção de visitante e Perfil do visitante são semelhantes aos relatórios de Público no Google [!DNL Analytics]. O foco da Retenção está mais na frequência de retorno, enquanto o foco do Perfil do visitante está mais na geografia e tecnologia dos usuários.

Os relatórios Conversão personalizada e Tráfego personalizado são relatórios de dimensão personalizados. As conversões são eVars. Você pode definir uma expiração personalizada para o valor, como ocorrência, visita, mês e ano. Esse valor permanece consistente para um usuário no intervalo de tempo configurado, a menos que seja substituído. As variáveis de tráfego são props. Você também pode configurá-las para Relatórios de definição de caminho ou como itens de lista, que detalharão vários valores com base em um delimitador de sua escolha.

A Mídia é para coisas como vídeos ou arquivos de áudio, onde você configurou um rastreamento de mídia especial.

Relatórios personalizados é uma seção na qual um usuário pode personalizar as colunas e os detalhamentos criados na interface dos relatórios e salvá-los como um relatório personalizado. No entanto, como mencionado acima, como o Workspace permite detalhamentos e correlações muito mais avançados, qualquer personalização deve ser realizada lá. Essa era uma boa solução antes de a Workspace existir.

A seção Marcadores é semelhante aos Relatórios personalizados, onde os relatórios usados com frequência podem ser marcados na interface dos relatórios para facilitar sua localização.

O Painel era um produto herdado que permitia às pessoas combinarem reportlets de dados em uma visualização. No entanto, a funcionalidade no Workspace (Seção 2.1.2.1) é tão mais fácil de usar, que só existe como um ponto de acesso para relatórios herdados que devem ser recriados antes que esse recurso seja descontinuado.

As metas permitem que as pessoas criem um relatório com base em uma meta em um determinado período. As equipes monitoram campanhas para ver se elas estão no caminho para atingir suas metas de tráfego.

Todos os relatórios aqui permitiam várias colunas de métrica e detalhamentos de dimensão. No entanto, a simplicidade das visualizações e parte da lógica por trás de quais elementos podem ser correlacionados pode ser frustrante às vezes.

##### 2.1.3.2. Relatórios do Google [!DNL Analytics]

O Google [!DNL Analytics] divide esses relatórios nas seguintes seções: Tempo Real, Público-Alvo, Aquisição, Comportamento, Conversas (no GA3), Ciclo de Vida (com as subseções: Aquisição, Envolvimento, Monetização, Retenção) e Usuário (com as subseções: Demografia e Tecnologia).

![google-analytics-interface-compare](assets/ga-to-aa_7.png)

É possível fazer pequenos ajustes nessas visualizações, adicionar um detalhamento de dimensão secundário, alterar a visualização, criar um filtro dos dados e muito mais. Você pode salvar suas personalizações como um Relatório salvo.

Eles fornecem insights rápidos e fáceis para seus dados. No entanto, você não pode comparar itens como Usuários a exibições de página para uma página na mesma tabela e não pode adicionar mais de uma dimensão extra para ver dados adicionais.

São boas para dados analíticos rápidos, mas se você realmente precisa pesquisar fundo, elas sofrem com as limitações.

### 2.2. Acesso estendido ao relatório

Além do &quot;Relatório no local&quot;, a maioria das ferramentas oferece funcionalidade estendida que permite levar sua análise para fora das ferramentas e criar algo um pouco mais personalizado.

#### 2.2.1. Report Builder [!DNL Adobe Analytics] (Extensão do Microsoft® Excel)

O Workspace é uma ótima ferramenta, mas, às vezes, é necessário inserir seus dados em uma planilha personalizada, para que você possa unir várias fontes de dados. É aqui que o Report Builder entra em cena.

O Report Builder é um plug-in para o Microsoft® Excel que permite criar conexões com seus dados do [!DNL Adobe Analytics] para obter dados tabulares que podem ser manipulados no Excel. Geralmente, para usar isso com eficiência, você puxaria os dados para algumas guias de dados brutos, usaria referências de células do Excel para extrair dados dessas guias em um único relatório consolidado e criaria gráficos e visualizações.

>[!NOTE]
>
>O Report Builder tem uma permissão especial que precisa ser aplicada aos usuários para acessar este plug-in. Isso deve ser concedido a usuários que aprenderam a usar a ferramenta corretamente.

#### 2.2.2. Conexão de API [!DNL Adobe Analytics]

Se você precisar que os dados de [!DNL Adobe Analytics] sejam processados por algo diferente do Excel e desejar que eles incluam as exclusões de regra de bot, use a API de [!DNL Adobe] para obter os dados diretamente. Em seguida, processe os dados usando um script ou adicione-os a um banco de dados para uso com outro sistema.

Observe que a API ainda extrai dados de correlação aplicando os detalhamentos e segmentos conforme especificado na solicitação de obtenção.

O Workspace do [!DNL Adobe] (Seção 2.1.2.1) usa a API para criar os relatórios e, se você habilitar o modo de depuração no Workspace, ele mostrará as chamadas de API usadas. Essa é uma maneira rápida de criar suas chamadas de API. Ao usar o Workspace para criar e validar os dados que deseja obter, você pode usar essas chamadas de API para obter os dados para seu próprio processamento.


#### 2.2.3. Data Studio do Google [!DNL Analytics]

Se você está lendo este documento, já sabe que mencionei o Data Studio como equivalente ao Workspace de [!DNL Adobe]. O Data Studio permite extrair dados do Google [!DNL Analytics], mas também dados de outras fontes. Isso é bom se você quiser consolidar os dados de análise com outros dados coletados. No entanto, com o Google [!DNL Analytics], o mesmo tipo de limitação de visualização está presente. A forma como as linhas e colunas são formadas ainda é limitada.

Ainda é uma ferramenta poderosa, e eu de forma alguma desaconselharia as pessoas a usá-la. A minha experiência pessoal é que considero o comportamento rígido bastante limitante.


#### 2.2.4. Extensão das Planilhas Google

Para uso próprio, quando preciso extrair dados de maneira estendida do Google [!DNL Analytics], minha ferramenta pessoal de escolha é a Extensão de Planilha do Google. Embora eu precise fazer várias conexões com minhas tabelas de GA, posso fazer referência às células dos dados brutos e criar os relatórios que preciso. Em seguida, visualizo-os usando os recursos gráficos das Planilhas Google.


## 3. Exportações de dados brutos

Quando você realmente precisa de dados brutos, o [!DNL Adobe] e o Google oferecem os recursos para obter informações nesse formato.

### 3.1. Feed de dados do [!DNL Adobe]

Na Seção 2.2.2, mencionei que a API [!DNL Adobe Analytics] extraía de &quot;dados processados&quot;. O feed de dados brutos extrai dados processados pelas &quot;Regras de processamento&quot; que foram configuradas no painel de administração, mas esses dados brutos incluem todos os dados excluídos em qualquer outro lugar.

Isso significa que todas as exclusões de bot, dados filtrados por IP interno e outros dados excluídos estão nos feeds de dados brutos. Existem sinalizadores para identificar esses dados, portanto, se você criar um data lake, a equipe de engenharia poderá criar uma lógica para processar esses dados adequadamente.

Os feeds de dados brutos podem ser personalizados para enviar todas as colunas de dados ou apenas colunas específicas se você precisar de um feed mais focado.

Os feeds podem ser enviados diretamente para o FTP, SFTP ou S3.


### 3.2. Google Big Query

Infelizmente, essa é uma ferramenta do Google que eu não tenho experiência em usar. Em teoria, ele deve ser semelhante ao Feed de Dados de [!DNL Adobe], permitindo que sua equipe de engenharia acesse dados brutos da sua conta do Google [!DNL Analytics].

No entanto, em vez de fornecer um despejo completo de dados brutos, ele permite que os engenheiros acessem os dados por meio de consultas SQL para obter dados brutos direcionados ou todas as colunas de dados brutos.

## 4. Conclusão

Como qualquer sistema, a prática é necessária para se familiarizar com a ferramenta. Esperamos que este guia o ajude a começar ou forneça dicas para melhorar o uso do [!DNL Adobe Analytics].

No entanto, eu recomendaria o uso do [!DNL Adobe Analytics] e do Google [!DNL Analytics] em sua estratégia de implementação (mesmo que o Google [!DNL Analytics] seja apenas a versão gratuita). Isso permite ter um sistema de backup para garantir que você tenha dados, pois nenhum sistema é infalível.

Há muitos recursos disponíveis para você além deste guia que podem ajudar a melhorar sua estratégia:

* [[!DNL Adobe] Experience League](https://experienceleague.adobe.com/?lang=pt-BR#home) - Contém tutoriais, vídeos, documentação e fóruns da comunidade
* [[!DNL Adobe] Grupos de usuários](https://analytics-augs.adobe.com/) - Um hub de eventos executados pela comunidade para ajudar os usuários a se conectarem e melhorar suas implementações.
* [[!DNL Adobe Analytics] Canal YouTube de Grupos de Usuários](https://www.youtube.com/channel/UCQOHnCs7KZgsuFHVzwboQuA) - Não foi possível criar uma sessão de grupo de usuários [!DNL Adobe Analytics]? Assista novamente às sessões anteriores de grupos de usuários em todo o mundo para saber mais sobre como seus colegas estão usando a ferramenta.
* [Canal de Slack de Chat de Medida](https://www.measure.chat/) - Conecte-se com [!DNL Adobe Analytics] usuários em todo o mundo e compartilhe aprendizados do setor, faça perguntas a seus colegas e participe de grupos de interesse com foco em medição.
* e muito mais!

## Autor

Este documento foi escrito por:

![Jennifer Dungan](assets/Jennifer_Dungan_Headshot150.png)

Jennifer Dungan, gerente de otimização [!DNL Analytics] na Torstar

[!DNL Adobe Analytics] Especialista
