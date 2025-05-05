---
title: Crie um diagrama de fluxo de dados para entender sua pilha de tecnologia de marketing
description: Saiba como criar um diagrama de "Líder e fontes de dados" para entender o universo de dados, auditar e organizar a instância com eficiência.
feature-set: Marketo Engage
feature: Administration
role: Admin
level: Intermediate, Experienced
doc-type: Tutorial
last-substantial-update: 2023-10-16T00:00:00Z
jira: KT-13877
thumbnail: KT-13877.jpeg
hide: false
exl-id: 088bdcf1-4e49-44a7-ac78-a03742ff680b
source-git-commit: 1205848b1985a99b91f9d4d25e1a79f0df379589
workflow-type: tm+mt
source-wordcount: '569'
ht-degree: 2%

---

# Criar um diagrama de fluxo de dados para entender sua pilha de tecnologia de marketing

Como um administrador que assume uma instância do [!DNL Marketo Engage] que está ativa há anos, é como uma missão impossível auditar e organizar a instância com eficiência. Quando [!DNL Adobe] [!DNL Marketo Champion] (2019), Kelly Jo Horton, entrou em uma instância há muito estabelecida, ela enfrentou esse desafio ao [criar um diagrama de &quot;Líder e fontes de dados&quot;](https://nation.marketo.com/t5/employee-blogs/understand-your-marketing-technology-and-data-create-this/ba-p/296774){target="_blank"} para se familiarizar com o universo de dados. Neste tutorial, você aprenderá a criar seu próprio diagrama de fluxo de dados, aproveitando os exemplos compartilhados por Kelly Jo Horton. Vamos conhecer seu ecossistema da MarTech!

## Por que criar um diagrama de arquitetura para sua instância herdada?

1. **Familiarize-se com a pilha de tecnologia de marketing herdada de uma instância ativa.** Todos os gerentes de operações de marketing/gerentes de operações de plataforma são incentivados a realizar esse exercício ao iniciar uma nova empresa. Esse processo de criação permite que os usuários administradores vejam a imagem completa dos dados e atividades enviados de integrações externas para o [!DNL Marketo Engage] e solucionem facilmente os erros da API.
2. **Familiarize-se com as principais partes interessadas que gerenciam as integrações externas.** Uma dica que Kelly Jo Horton usa para identificar as partes interessadas rapidamente é fazer referência à lista de usuários da API.
   1. **Navegue até a guia &#39;Integração>LaunchPoint&#39; na seção &#39;Administrador&#39;.** Saiba mais sobre como navegar até a guia &#39;LaunchPoint&#39;: [Crie um Serviço Personalizado para Usar com a API REST](https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/create-a-custom-service-for-use-with-rest-api.html?lang=pt-BR){target="_blank"}.
   2. Encontre estatísticas de uso de API por usuário de API na guia Integração>Serviços da Web na seção Informações sobre chamada de API. Ao clicar no número da chamada da API, é possível visualizar as chamadas individuais específicas feitas por cada usuário.

## Como fazer este exercício de diagrama de fluxo de dados visuais

### Etapa 1: Diagrama de Estado Atual

Crie um diagrama de &quot;Estado atual&quot;. Exemplo:

![Diagrama de estado atual](/help/marketo-tutorial-inherited-instance/_assets/data-flow-diagram/Current_State_Lead_Data_Sources_KellyJo_Horton.png){align="center"}


### Etapa 2: diagrama do estado futuro

Crie um diagrama de &quot;Estado futuro&quot; que possa ser usado ao apresentar o roteiro de tecnologia e sistemas para participantes não técnicos. Exemplo:

![Diagrama de estado futuro](/help/marketo-tutorial-inherited-instance/_assets/data-flow-diagram/Future-State-Lead-Data-Sources-KellyJo-Horton.png){align="center"}

### Etapa 3: Versão técnica

Crie uma versão técnica que mostre detalhes como o nome de usuário da API para cada integração, uma breve descrição do tipo de dados que está sendo enviado por push para [!DNL Marketo Engage] ou extraído de [!DNL Marketo Engage] e um diagrama detalhado de quaisquer fluxos e acionadores de middleware.  Exemplo:

![Versão técnica](/help/marketo-tutorial-inherited-instance/_assets/data-flow-diagram/Lead-Data-Source-Diagram-KellyJo-Horton.png){align="center"}


## O que vem a seguir?

**Introdução aos Exemplos:**
Baixe um dos diagramas de fluxo de dados de amostra para mapear o estado atual de sua pilha de tecnologia de marketing, pessoa e fluxo de dados ou crie um diagrama para seu universo de dados do zero enquanto audita a instância:


<table style="table-layout:fixed">
   <tr>  
      <td style="border: 0;">
      <div style="text-align: center;">
          <a href="./_assets/downloads/Current_Future_State_Lead_Data_Sources.zip">
            <strong>Estado atual e estado futuro</strong>
         </a>
      </div>
      </td>
      <td style="border: 0;">
      <div style="text-align: center;">
         <a href="./_assets/downloads/Detailed_Layers_by_Functional_Category_Stacked_Technologies.zip">
         <strong>Camadas Detalhadas por Categoria Funcional </strong>   
         </a>
      </div>
      </td>
      <td style="border: 0;">
         <div style="text-align: center;">
         <a href="./_assets/downloads/Lead_Data_Source.zip">
           <strong>Fluxo de clientes potenciais e de dados do Source </strong>  
         </a>
         </div>
       </td> 
       <td style="border: 0;">
         <div style="text-align: center;">
         <a href="./_assets/downloads/Simple_World_Class_Stage_Stack.zip">
          <strong>Diagrama simplificado</strong>  
         </a>
         </div>
        </td>  
   </tr>
   <tr>
    <td style="border: 0;">
         <div>
          <img alt="Diagrama do Estado Atual e do Estado Futuro" src="./_assets/Thumbnail_Current-Future State Lead_Data Sources_KellyJo_Horton.png"/>
         </a>
      </div>
      </td>
      <td style="border: 0;">
         <div>
         <a href="./_assets/downloads/Detailed_Layers_by_Functional_Category_Stacked_Technologies.zip">
         <img alt="Diagrama de Camadas Detalhadas por Categoria Funcional" src="./_assets/Thumbnail_Detailed_Layers_by_Functional_Category_Stacked_Technologies_KellyJo_Horton.png" />
       </a>
         </div>
      </td>
       <td style="border: 0;">
         <div>
            <a href="./_assets/downloads/Lead_Data_Source.zip">
         <img alt="Diagrama de Fluxo de Source de Dados e Cliente Potencial" src="./_assets/Thumbnail_Lead-Data Source Diagram_KellyJo_Horton.png" />
         </a>
         </div>
      </td>
     <td style="border: 0;">
         <div>
            <a href="./_assets/downloads/Simple_World_Class_Stage_Stack.zip">
             <img alt="Diagrama simplificado" src="./_assets/Thumbnail_Simple_World_Class_Stage_Stack.png" />
         </a>
         </div>
      </td>
</table>

Estas são algumas ferramentas que você pode usar: draw.io (Google Docs), [!DNL Adobe] XD, Figma, Gliffy (em Confluência)

**E se já houver diagramas de arquitetura?** Os novos membros da equipe podem ter perspectivas diferentes. É importante que os novos administradores do [!DNL Marketo Engage] façam esse exercício como parte do processo de integração e o compartilhem com outras pessoas.

## Autores

**Kelly Jo Horton**\
[!DNL Adobe] Marketo Champion (2019)
*Parceiro Cliente Sênior na Etumos*

![Kelly Jo Horton](/help/marketo-tutorial-inherited-instance/_assets/authors/Customer_Author_Kelly_Jo_Horton.png){width="30%"}

**Amy Chiu**
*Gerenciador de Marketing de Adoção e Retenção,[!DNL Adobe]*

(/help/marketo-tutorial-inhereted-instance/_assets/author/[!DNL Adobe]_Author_Amy_Chiu.png){width=30%}
