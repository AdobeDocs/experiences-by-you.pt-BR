---
title: Eleve suas análises de dados a um novo patamar com as Métricas calculadas
description: Saiba como um especialista ponto a ponto usa métricas calculadas para criar novas métricas sem alterar sua implementação e usar os dados já coletados para ajudar a responder a perguntas comerciais complexas.
feature-set: Analytics
feature: Calculated Metrics
role: User
level: Beginner
doc-type: Article
last-substantial-update: 2023-05-16T00:00:00Z
jira: KT-13266
thumbnail: KT-13266.jpeg
exl-id: 301ee179-b154-4cf2-b27e-77f38a8945a0
source-git-commit: 058d26bd99ab060df3633fb32f1232f534881ca4
workflow-type: tm+mt
source-wordcount: '1549'
ht-degree: 3%

---

# Eleve suas análises de dados a um novo patamar com as Métricas calculadas

A maioria dos novos usuários do [!DNL Adobe Analytics] estão familiarizados com Segmentos como uma maneira de cortar e dividir seus dados. Hoje, quero apresentar a vocês as métricas calculadas, a próxima melhor ferramenta da sua caixa de ferramentas de analistas.

Como um recurso avançado do [!DNL Adobe Analytics], as métricas calculadas permitem criar novas métricas sem alterar a implementação usando os dados que você já coletou. O Construtor de métricas calculadas pode usar várias funções matemáticas e estatísticas diferentes, para que você possa criar métricas que respondam até mesmo às perguntas comerciais mais complexas.

## Introdução às métricas calculadas

Para começar a usar métricas calculadas, vejamos um exemplo simples. Imagine que você queira entender se os usuários de autoatendimento online têm um valor médio de pedido (AOV) mais alto do que os usuários assistidos por chamada. Para criar uma métrica calculada para responder a essa pergunta, faça o seguinte:

Para abrir o Criador de métricas calculadas, use a navegação superior para clicar em → **Componentes** → **Métricas calculadas** → **+ Adicionar.** Ou clique no link **sinal +** acima **Métricas** no painel Componentes.


![Cálculo 01](assets/calc01.png) ![Cálculo 02](assets/calc03.png) ![Cálculo 03](assets/calc02.png)

![Cálculo 04](assets/calc04.png)

*Descrições abaixo para itens de interface do usuário*

Depois que o Construtor de métricas calculadas for aberto, adicione e/ou faça o seguinte:

**A.** Um nome para a métrica calculada. Esse nome é exibido na lista de componentes das métricas, portanto, deixe-o algo que ficará claro para você mesmo e para outras pessoas, como *AOV da central de atendimento*.

**B.** Uma descrição da métrica calculada. Essa descrição é exibida quando os usuários clicam no ícone **i**&#39; ao lado da métrica na lista de componentes, portanto, verifique se ela é informativa. Por exemplo, para o Call Center AOV, podemos adicionar *Calcula AOV para Pedidos Assistidos da Central de Atendimento*.

**C** O formato da métrica: escolha decimal, hora, porcentagem ou moeda e adicione casas decimais e polaridade. Aqui, nós escolheremos *Moeda para o Formato, 0 para o número de decimais e* ⬆ *Bom (verde) para polaridade.*

**D**. Se você estiver usando tags, que permitem aplicar tópicos e localizar rapidamente métricas calculadas, adicione aqui as tags que se aplicam. Adicionamos *AOV* e *Call center* específicos.

**E** Esta seção é para exibição - à medida que você cria a métrica calculada na seção F, a fórmula será exibida aqui.

**F** Aqui, você arrastará e soltará dimensões (H), métricas (I) ou segmentos (J) para criar sua métrica calculada, bem como os operadores da fórmula. Para cada métrica, se você clicar no botão de rolagem, será possível alterar o Tipo de métrica (Padrão/Total) e o Modelo de atribuição. *Arrastaremos e soltaremos a Receita da Central de Atendimento e, abaixo dela, nós*÷*. Aceitaremos o tipo de métrica padrão e o modelo de atribuição.*

**G**. Usar este **+Adicionar** opção para adicionar condições ou números estáticos adicionais, que não são necessários aqui.

**K.** E finalmente, conforme você faz seus cálculos, você pode visualizar os dados dos últimos 90 dias aqui.

Agora que criamos o AOV da Central de Atendimento, também precisamos de uma métrica calculada para o AOV Online. Fazíamos isso seguindo as mesmas etapas descritas acima.

Em seguida, podemos criar uma terceira métrica calculada, usando o Construtor de métricas calculadas ou dinamicamente na tabela de forma livre, para comparar a Central de atendimento e o AOV online, de modo que tenhamos algo como isso:

![Cálculo 05](assets/calc05.png)

Em nosso exemplo, vemos um aumento significativo quando os compradores usam a central de atendimento para ajudá-los a fazer uma compra. Esses dados podem informar nossas decisões sobre como ajudar os clientes a obter assistência com suas compras por meio de, por exemplo, ofertas pop-up ou outras experiências guiadas.

## Utilização de segmentos em métricas calculadas

Agora, vamos ver como podemos usar segmentos em métricas calculadas para obter mais informações sobre o comportamento, as preferências e as motivações do cliente. Com segmentos e métricas calculadas, podemos aprender o suficiente sobre os clientes para melhorar sua experiência, aumentar a receita e melhorar a satisfação e a fidelidade do cliente.

Já sabemos pelos exemplos de AOV acima que as compras assistidas pela central de atendimento normalmente têm uma AOV mais alta. No entanto, outras métricas nos informam que a maioria dos usuários não usa a central de atendimento para compras.

Então, quais categorias de varejo - e caminhos de usuário por meio dessas categorias - resultam no AOV mais alto?  Podemos descobrir ao combinar segmentos com métricas calculadas.

Para fazer isso, primeiro precisamos criar um nível de visita *include* e *excluir* para cada categoria de produto. Incluir ou excluir é determinado ao clicar no ícone **Opções** engrenagem no canto direito do recipiente. O padrão é Incluir.

![Cálculo 06](assets/calc06.png) ![Cálculo 07](assets/calc07.png)

Após criar esses segmentos, podemos criar uma métrica calculada para responder à sua pergunta. Abrimos o Criador de métricas calculadas e fazemos o seguinte:

1. Procure os segmentos recém-criados e arraste e solte os que queremos usar na área cinza na parte superior do **Definição** caixa. Por exemplo, se queremos criar uma AOV para usuários que visitaram as categorias Feminino e Masculino, mas não Infantil, podemos arrastar e soltar esses três segmentos nessa área: *Incluir femininos*, *Incluir masculinos*, e *Excluir da criança*. Nós chamamos isso de *empilhar segmentos*.

   ![Cálculo 09](assets/calc09.png) ![Cálculo 08](assets/calc08.png)

1. Em seguida, arrastamos e soltamos as **Receita online** no mesmo contêiner, em seguida **Pedidos online**. Como os contêineres funcionam como expressões matemáticas para determinar a ordem das operações, os itens nos contêineres são processados antes dos processos subsequentes, embora não tenhamos vários contêineres ou processos nesse cálculo.
1. Alteramos o operador entre as duas métricas para divisão ().
1. We Select **Moeda** como o formato, **0** casas decimais, e **PARA CIMA** para polaridade.
1. Nomeie a métrica calculada e forneça uma descrição.
1. Salvar.

Quando terminarmos, nossa métrica calculada ficará assim:

![Cálculo 10](assets/calc10.png)

Depois de criarmos métricas calculadas usando segmentos empilhados para cada combinação da jornada de categoria do visitante e analisarmos os dados, veremos o que aprendemos! Os usuários que visitam as categorias Feminino e Masculino durante sua visita têm o AOV mais alto e, quando comparado aos visitantes de uma única categoria, o aumento é significativo:

![Cálculo 11](assets/calc11.png) ![Cálculo 12](assets/calc12.png)

Sabendo disso, podemos otimizar o layout da página, as disposições do produto e as mensagens promocionais para inserir mais pessoas nessas categorias antes de concluir a compra.

## Valioso, mas não disponível em todos os lugares

**Portanto, as métricas calculadas, simples e complexas, são super valiosas para analistas!**

No entanto, essas métricas não estão disponíveis em todas as áreas do [!DNL Adobe Analytics]. Não é possível usar métricas calculadas em:

- Fallout na Analysis Workspace
- Análise de coorte no Analysis Workspace
- Data Warehouse
- Relatórios em tempo real
- Relatórios de Dados atuais
- [!DNL Analytics] para o Target
- Report Builder

## Práticas recomendadas de métricas calculadas

Agora que você sabe o quanto as métricas calculadas podem ser valiosas, vamos dar uma olhada nas práticas recomendadas para criá-las.

1. **Verifique a sintaxe da fórmula.** Verifique se a sintaxe da fórmula está correta e segue a [!DNL Adobe Analytics] para garantir que você obtenha informações significativas.
1. **Verifique a ordem das operações.** Certifique-se de usar os contêineres com cuidado e colocar as coisas na ordem matemática correta de operações.
1. **Não conte dados duas vezes**. É possível evitar a contagem dupla de dados, garantindo que a fórmula usada na métrica calculada não conte os mesmos dados várias vezes. Isto é frequentemente conseguido combinando *Incluir* e *Excluir* condições na métrica calculada ou por meio do uso de segmentos.
1. **Verifique a granularidade de tempo.** Verifique se a métrica calculada tem a mesma granularidade de tempo que as métricas de origem usadas na fórmula.
1. **Usar dados precisos:** Você só obterá resultados valiosos se usar dados precisos e confiáveis no cálculo.

## Práticas recomendadas do segmento personalizado

Ao criar segmentos no [!DNL Adobe Analytics], lembre-se destas práticas recomendadas:

1. **Mantenha simples.** Evite complicar o segmento em excesso. Mantenha o mais simples possível e use apenas as condições necessárias para garantir a precisão.
1. **Usar os tipos corretos de contêiner**. Use o tipo correto de contêiner (visitante, visita ou ocorrência) na definição do segmento para evitar resultados incorretos.
1. **Não conte dados duas vezes**. Assim como com as métricas calculadas, verifique se o segmento não conta os mesmos dados várias vezes. Os contêineres Incluir e Excluir podem ajudar.
   1. Quando um container de inclusão é usado, ele *inclui* *todo o conteúdo da visita* se alguma ocorrência corresponder à condição na visita.
   1. Quando um container de exclusão é usado, ele *exclui todo o conteúdo da visita* se alguma ocorrência corresponder à condição na visita.
1. **Aninhar contêineres corretamente**. Determine quais dados são incluídos usando o contêiner mais externo e aplique regras aninhadas aos dados restantes. À medida que regras aninhadas são aplicadas, o fluxo de segmento atua como um funil e as regras subsequentes não se aplicam a nenhuma ocorrência excluída pela primeira regra.
1. **Verifique se os seus dados estão atualizados.** Use dados precisos e atualizados na definição de segmento para obter resultados precisos.
1. **Teste o segmento.** Sempre teste o segmento para verificar se ele está funcionando como pretendido antes de liberá-lo para outras pessoas.
1. **Considere o desempenho.** Os segmentos podem retardar o processamento de relatórios, portanto, considere esse impacto ao criá-los.

## Principais aprendizados

Combinação de segmentos e métricas calculadas no [!DNL Adobe Analytics] podem levar a análises de dados mais robustas e eficazes. Ao cortar e cortar seus dados e criar cálculos para comparação, você pode obter insights mais profundos sobre o comportamento do cliente que pode usar para otimizar suas campanhas de marketing e criar painéis e relatórios personalizados. No entanto, lembre-se de que as métricas calculadas não estão disponíveis em todas as áreas do [!DNL Adobe Analytics]e siga as práticas recomendadas para garantir que você obtenha dados precisos e úteis.


## Autor

Este documento foi escrito por:

![Debbie Kern](assets/calc13.jpeg)

**Debbie Kern**, Sênior [!DNL Adobe Analytics] Gerente na Adobe

![Resposta](assets/calc14.png)
