---
title: Criação de modelos de pontuação de pessoas para programas do Marketo Engage
description: O Adobe Marketo Engage permite criar modelos de pontuação desde o início. Antes de pular diretamente no Marketo Engage para criar seus programas de pontuação, será necessário configurar os campos de pontuação essenciais, como Pontuação demográfica, Pontuação comportamental e Pontuação total de pessoa. Saiba mais sobre as estratégias usadas pelos especialistas em Marketo Engage para desenvolver Modelos de pontuação de que sua empresa precisa.
role: Admin
level: Beginner
doc-type: Article
solution: Marketo Engage
duration: 0
last-substantial-update: 2024-05-04T00:00:00Z
jira: KT-14810
thumbnail: KT-14810.jpeg
source-git-commit: 47ab8875bc4e41595cd40550330e43a88357b68d
workflow-type: tm+mt
source-wordcount: '2111'
ht-degree: 2%

---

# Criação de um modelo de pontuação de pessoa

A pontuação de pessoa ajuda você a identificar as pessoas que estão mais envolvidas com sua empresa e são seu Perfil de cliente ideal, para que você possa compartilhar esses leads com sua equipe de vendas e fechar negócios! Juntamente com as vendas, você determina quais leads deseja entregar a eles usando um programa de pontuação de lead/pessoa no Adobe Marketo Engage. Isso pode ser determinado por um mínimo de pontuação comportamental, pontuação demográfica ou ambos.

Neste tutorial, vamos orientá-lo por três exercícios sugeridos pelas campeãs de Marketo Engage Christina Zuniga e Katja Keesom. Acompanhe para determinar quais atividades e características são indicadores importantes que um cliente potencial está interessado em comprar (pontuação comportamental), é a mais adequada para você (pontuação demográfica) e leve em conta as nuances dos mercados.

## Por que desenvolver e usar um modelo de pontuação de pessoa?

Você pode ter muitos clientes em potencial em seu banco de dados, mas como saber quais estão prontos para comprar seus produtos e serviços agora? Conforme sua organização de marketing busca otimizar a qualidade dos clientes potenciais e a disponibilidade de vendas, o modelo de pontuação é aplicado nesse ponto.

Ao pontuar pessoas em seu banco de dados de Marketo Engage, você pode medir o nível de qualificação de seus leads gerados e definir critérios para quando eles estão prontos para vendas. Isso permite que sua equipe de vendas se concentre nos clientes potenciais com maior probabilidade de fechar, enquanto a equipe de marketing continua a nutrir as outras pessoas no banco de dados por meio de seus programas de marketing.

## Exercício 1 - Determinar o interesse do comprador com pontuações comportamentais

A pontuação comportamental dá um valor numérico às ações rastreáveis que um cliente potencial toma que indicam interesse em seus produtos e serviços e intenção de comprar. Por exemplo, visitar o site mostra interesse e visitar a página de preços pode mostrar intenção. Por outro lado, visitar a página de carreiras pode indicar que a pessoa não vai comprar.

**Etapa 1** - Faça uma lista de atividades de prospecto que sejam importantes para o seu processo de vendas ou que sejam valiosas para a sua organização. Pode ser útil trabalhar com sua equipe de vendas para determinar quais atividades indicam que um cliente potencial tem a intenção de comprar, ajudando você a alinhar os critérios com as vendas e priorizar com base em suas observações de ofertas fechadas. Aqui estão algumas sugestões de perguntas que você pode fazer à sua equipe de vendas:

* Quais atividades indicam um cliente em potencial bom ou ruim para você?
* Que tipo de conteúdo consumido por um cliente potencial tem uma intenção mais forte de comprar?

**Etapa 2** - Lista ações que indicam que um cliente potencial não está interessado em seu produto. Certifique-se de listar as atividades que são rastreáveis por meio do Marketo Engage.

**Exemplo 1a - Atividades que indicam a intenção de comprar**

| **Atividades indicando intenção de compra** | **Atividades indicando NENHUMA intenção de comprar** |
| --- | --- |
| Visitar página de preços | Nenhuma interação nos últimos 90 dias |
| Participar do evento anual do cliente | Visitar página de carreiras |
| Registrar-se no webinário | Cancelamentos de assinatura |
| Baixar white paper |     |
| Preencha o formulário de demonstração de solicitação |     |

**Etapa 3** - Analise e escolha uma pontuação de limite de entrega de vendas.

* Quando um lead indicar interesse suficiente ao executar algumas das atividades definidas na Etapa 1 e a pontuação total exceder esse limite, você os entregará às vendas. Esse limite será simplesmente um número que ajuda a definir um referencial para as pontuações atribuídas a comportamentos individuais.
* Seu número limite deve ser grande o suficiente para que uma pessoa precise concluir várias interações com sua marca para atingi-lo. Por exemplo, é improvável que um email aberto seja um qualificador suficiente. Se você acabou de começar, tente trabalhar com um limite de 100 e criar sua pontuação de pessoa a partir daí.
* Definir um limite alto ou baixo depende de quais clientes potenciais sua equipe de vendas está mais interessada em receber e desenvolver oportunidades de negócios. Se você tiver dados existentes sobre suas recentes negociações de vendas, analise-os e veja quais ações as pessoas tomaram em negociações bem-sucedidas. Isso pode ajudá-lo a determinar quantos pontos de contato entram em um lead de vendas qualificado e a extrapolar de lá qual deve ser seu número limite.

**Exemplo 1b - Limite para entrega de vendas:**

| Número médio de pontos de contato para lead qualificado | 4 |
| --- | --- |
| Limite para entrega de vendas | 50 |

**Etapa 4** - Atribua uma pontuação a cada atividade listada no &quot;Exemplo 1a - Atividades indicando intenção de comprar&quot;.

* Use uma pontuação de comportamento positiva para as atividades que indicam interesse para aumentar a pontuação geral de lead de um cliente potencial, e uma pontuação negativa para indicar desinteresse.
* Usando seu limite do &quot;Exemplo 1b - Limite para entrega de vendas&quot; como um referencial, determine suas pontuações de comportamento em relação à importância de suas ações. Por exemplo, os clientes potenciais que solicitarem uma demonstração devem ir direto para as vendas. Atribuir a essa ação um valor de ponto igual ao limite de entrega do cliente potencial fará mais sentido. Entretanto, o download de um livro branco não é um indicador tão forte de interesse de compra e, portanto, deve valer menos pontos.

**Exemplo 1c - Pontuação de atividades indicando a intenção de comprar:**

| Limite para entrega de vendas = 50 pontos |     |
| --- | --- |
| Atividade | Pontuação |
| Preenchido &quot;solicitar um formulário de demonstração&quot; | +50 |
| Nenhuma interação nos últimos 90 dias | \-10 |
| Baixar um white paper | +5 |
| Visite-nos em uma feira | +15 |

**Etapa 5** - Lembre-se, a pontuação é um processo iterativo! Revise e ajuste continuamente pontuações e limites à medida que coletar mais dados para análise.

## Exercício 2 - Identificação do ajuste certo com pontuações demográficas

Agora que você definiu as atividades indicando a intenção de compra, deve concluir o modelo de pontuação com os Perfis de cliente potencial ideal. Para identificar se um cliente potencial é a opção certa para futuras conversas de vendas, é importante atribuir pontuações demográficas além de pontuações comportamentais para que o modelo ajude a determinar os melhores leads em termos de adequação e intenção.

**Etapa 1** - Faça uma lista de características para seus clientes potenciais ideais.

* Considere a listagem de atributos como setor, empresa, departamento e função. Verifique se essas características correspondem aos campos demográficos disponíveis na instância do Marketo Engage.
* Trabalhe com sua equipe de vendas para determinar quais clientes potenciais respondem mais às consultas de vendas e são contatos importantes durante as oportunidades de vendas.
   * Pode ser útil analisar oportunidades recentes de ganhos fechados para ver quais características seus melhores clientes têm. Por exemplo,
      * Analisar as oportunidades fechadas perdidas para os padrões do pode levar você a encontrar dados demográficos que deseja evitar.
      * Identifique tomadores de decisão e líderes internos que impulsionam seus esforços de vendas. Aprofunde-se nos dados e leve suas descobertas a um workshop com algumas de suas equipes de vendas para validar ou refinar suas conclusões.
   * Você também pode entrevistar sua equipe de vendas com as seguintes perguntas de exemplo:
      * Com qual departamento eles estão geralmente se envolvendo?
      * Quais são os cargos das pessoas envolvidas em demonstrações de produtos e quem são as pessoas que precisam aprovar a compra?

**Exemplo 2a — características ideais do cliente potencial**

| **Categoria** | **Características ideais de prospecção** |
| --- | --- |
| Setor | Espaço aéreo, fabricação |
| Tamanho da empresa | 100 - 999, 1.000 - 9.999 |
| Cargo | Director, Vice-presidente, Nível C |
| Departamento | HR |

**Etapa 2** - Atribua uma pontuação a cada característica de acordo com sua relevância no perfil de cliente potencial ideal. Use pontuações positivas para características desejáveis e pontuações negativas para características que tornam o lead menos adequado ao seu produto.

**Exemplo 2b - Atribuição de pontuações a características de prospecto ideais e indesejáveis**

| **Característica** | **Pontuação** |
| --- | --- |
| Setor - Aeroespacial | +10 |
| Setor - Produção | +5 |
| Tamanho da empresa - 100 - 999 | +5 |
| Tamanho da empresa - 1.000 - 9.999 | +10 |
| Tamanho da empresa - &lt;10 | \-10 |

## Exercício 3 - Incorporação de flexibilidade local no modelo de pontuação

Com os modelos básicos de pontuação comportamental e demográfica que você concluiu, você pode elevar o nível ao permitir flexibilidade local. Os valores comerciais podem variar em diferentes mercados quando uma organização opera globalmente. No exercício a seguir, você aprenderá a aplicar pontuações para refletir o valor comercial real das atividades ou características principais em diferentes situações.

Você prefere uma apresentação em vídeo para este exercício? Ajuste como a Marketo Engage Champion Katja Keesom demonstra a criação de flexibilidade local no modelo de pontuação.

>[!VIDEO](https://video.tv.adobe.com/v/3426914/?learn=on)

**Etapa 1** - Tire as atividades e características dos exercícios 1 e 2 e determine se cada item varia de acordo com a localização ou a linha de produtos.

**Exemplo 3a - Sinais nos mercados globais e locais:**

| **Sinal** | **Global** | **Local** |
| --- | --- | --- |
| Atividades | <ul><li>Preenchido o formulário &quot;Solicitar uma demonstração&quot;</li><li>Nenhuma interação nos últimos 90 dias (cerca de 3 meses)</li></ul> | <ul><li>Visite-nos na feira</li><li>Baixar um white paper</li></ul> |
| Características | <ul><li>Departamento</li><li>Cargo</li></ul> | <ul><li>Setor</li><li>Tamanho da empresa</li></ul> |

**Etapa 2** - Definir a matriz de pontuação para os mercados locais:

* Configurar uma matriz diferente para elementos demográficos e de comportamento.
* Determine os tópicos de prioridades para você solicitar a entrada da equipe local.
* Defina o número de valores usados para classificar em seus tópicos.
* Atribua valores individuais alinhando o valor relativo às pontuações globais.
* Considere definir cenários comuns quando os clientes potenciais interagem com sua marca e teste sua pontuação geral para eles.
   * Por exemplo, uma jornada de cliente potencial comum que você vê seria uma pessoa entrar em seu site em uma página de conteúdo, depois clicar em uma página de produto e baixar um folheto. Você poderia direcioná-los com um convite de webinário, e eles responderão a ele se registrando, mas não participando. Considere se suas vendas já desejam falar com essa pessoa ou não e avalie se seu modelo de pontuação obtém esses clientes potenciais para a pontuação geral correta para refletir esse nível de interesse.

**Exemplo 3b - Matriz de pontuação demográfica:**

| **Matriz demográfica** | **Prioridade 1** | **Prioridade 2** | **Prioridade 3** |
| --- | --- | --- | --- |
| Valores altos | 20 pontos | 10 pontos | 7 pontos |
| Valores médios | 10 pontos | 7 pontos | 3 pontos |
| Valores baixos | 5 pontos | 3 pontos | 1 ponto |

**Etapa 3** - Colete informações de suas equipes de vendas locais ou regionais para desenvolver uma visão holística. Você observará que nenhuma pontuação individual está incluída no exemplo 3c. Isso permite que a equipe de vendas se concentre no valor relativo dos diferentes tópicos durante o processo de revisão. Entretanto, seu modelo completo deve ser documentado como material de apoio para outros administradores de Marketo Engage.

* Bloqueie o que não pode ser ajustado para consistência global (aqui, na coluna &quot;Implementar tópico&quot;).
* Marque (aqui, nas colunas &quot;Prioridade&quot; e &quot;Pontuação&quot;) o que pode ser ajustado para influências locais.

**Exemplo 3c - Valor relativo dos tópicos de pontuação:**

<table>
 <tr>
    <th>#</th>
    <th>Implementar tópico</th>
    <th>Demográfico/comportamental</th>
    <th>Tópico</th>
    <th>Prioridade</th>
    <th>Valores</th>
    <th>Pontuações</th>
 </tr>
 <tr>
    <td rowspan="6">1</td>
    <td rowspan="6"><b>OBRIGATÓRIO</b></td>
    <td rowspan="6">Demográfico</td>
    <td rowspan="6">Setor</td>
    <td rowspan="6"><b>2</b></td>
    <td>Tecnologia</td>
    <td><b>Alta</b></td>
  </tr>
  <tr>
    <td>Moda</td>
    <td><b>Alta</b></td>
  </tr>
  <tr>
    <td>Varejo</td>
    <td><b>Médio</b></td>
  </tr>  
  <tr>
    <td>Manufatura</td>
    <td><b>Médio</b></td>
  </tr>
  <tr>
    <td>Serviços de saúde</td>
    <td><b>Baixa</b></td>
  </tr>
  <tr>
    <td>...</td>
    <td><b>Baixa</b></td>
  </tr>
<tr>
    <td rowspan="3">2</td>
    <td rowspan="3"><b>Sim</td>
    <td rowspan="3">Demográfico</td>
    <td rowspan="3">Tamanho da empresa (funcionários)</td>
    <td rowspan="3"><b>3</td>
    <td>Mais de 1000 funcionários</td>
    <td><b>Alta</td>
  </tr>
  <tr>
    <td>250-999 funcionários</td>
    <td><b>Médio</td>
  </tr>
  <tr>
    <td>1-249 funcionários</td>
    <td><b>Baixa</td>
  </tr>  
<tr>
    <td rowspan="3">3</td>
    <td rowspan="3"><b>Não</b></td>
    <td rowspan="3">Comportamento</td>
    <td rowspan="3">Visitas à página no seu site</td>
    <td rowspan="3"><b>2</b></td>
    <td>&gt;Páginas de informações do produto</td>
    <td><b>Baixa</b></td>
  </tr>
  <tr>
    <td>Páginas de preços</td>
    <td><b>Médio</b></td>
  </tr>
  <tr>
    <td>Página de solicitação de demonstração</td>
    <td><b>Alta</b></td>
  </tr>
</table>

## O que está por vir?

* Baixe o [folha de exercícios de pontuação da pessoa](./assets/build-person-scoring-model-and-local-flexibility-in-adobe-marketo-engage.docx){target="_blank} para desenvolver seu modelo de pontuação offline.
* Desenvolva a pontuação da sua pessoa no Marketo Engage. Marque isto [tutorial](https://experienceleague.adobe.com/en/docs/marketo-learn/tutorials/lead-and-data-management/lead-scoring-watch){target="_blank} e [demonstração](https://experienceleague.adobe.com/en/docs/events/marketo-and-mochas-recordings/2023/lead-scoring){target="_blank} para começar. Você pode importar um programa de pontuação de cliente potencial/pessoa [modelo](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/programs/working-with-programs/import-a-program){target="_blank} da Biblioteca de referência do Marketo Engage para acelerar a criação do programa.
* Criar duas versões do programa de pontuação:
   * Um programa central que executa todas as pontuações que não podem ser atualizadas localmente.
   * Uma cópia local com os elementos de pontuação que são configuráveis.
* Configure os valores de pontuação como tokens no programa de pontuação. Isso garante a consistência, mesmo que você ajuste as pontuações ao longo do tempo.
   * Um exemplo comum de pontuações tokenizadas é ter um token para atividades de alto valor que atingem automaticamente seu limite, como solicitar uma demonstração ou reservar uma reunião com sua equipe de vendas. Mesmo que você altere a pontuação mínima necessária para atingir seu limite, é possível atualizar facilmente todas as atividades de alto valor de uma só vez, atualizando um token.
* Ajuste sua Campanha inteligente local para cada local:
   * Determine quais atividades demográficas e comportamentais devem ter pontuação apenas uma vez (ou seja, a indústria) e quais devem ter pontuação sempre que um cliente potencial se qualificar (ou seja, participou de um webinário). Isso garante que possíveis contatos acionados pela alteração do valor dos dados sejam relevantes para as vendas.
   * Certifique-se de que suas opções sejam mutuamente exclusivas.
   * Faça suas atualizações em ambas as etapas do fluxo para que a Pontuação de pessoa seja atualizada de maneira idêntica à Pontuação demográfica. Dessa forma, a Pontuação de pessoa permanece em conformidade com a combinação de pontuação de comportamento e pontuação demográfica.
* Teste a Campanha inteligente depois de concluir a criação do programa. Por exemplo, vá para o formulário de demonstração, preencha com um email de teste e verifique a pontuação da pessoa de teste em [banco de dados Marketo Engage](https://experienceleague.adobe.com/en/docs/marketo/using/getting-started-with-marketo/quick-wins/simple-scoring#step-view-the-person-info){target="_blank}.
* Depois de criar seu modelo, considere configurar um alerta para ir para vendas assim que a pontuação da pessoa atingir seu limite de entrega de vendas. Saiba mais sobre como configurar um alerta com este [tutorial](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert){target="_blank}.

### Autores

{{christina-zuniga}}

{{katja-keesom}}

{{amy-chiu}}