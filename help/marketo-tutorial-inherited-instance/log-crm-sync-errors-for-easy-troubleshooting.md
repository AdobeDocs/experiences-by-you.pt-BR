---
title: Registrar erros de sincronização do CRM para facilitar a solução de problemas
description: Saiba como usar um log de erros de sincronização do CRM para investigar problemas de sincronização do CRM e mantê-lo em execução sem problemas.
feature-set: Marketo Engage
feature: Administration
role: Admin
level: Intermediate, Experienced
doc-type: Tutorial
last-substantial-update: 2023-10-16T00:00:00.000Z
jira: KT-13875
thumbnail: KT-13875.jpeg
exl-id: 6a38f5dd-5d25-43d8-a1d3-e75ab396e555
product_v2:
  - id: fd1f54a9-f50c-467d-8956-cebbaf4f3eb8
    internal-label: Experience Manager
  - id: c68cd75e-5bca-4bc3-a60e-9e183f816441
    internal-label: Experience Manager Cloud Manager
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
feature_v2:
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
    internal-label: Administration
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
    internal-label: Intermediate
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
    internal-label: Experienced
source-git-commit: 749b293ab38b8ea5a5f72517bd5c3455399137c2
workflow-type: tm+mt
source-wordcount: '458'
ht-degree: 0%
---
# Registrar erros de sincronização do CRM para solução de problemas

Como administrador do [!DNL Marketo Engage], verificar se sua instância está sincronizada com o CRM deve ser uma parte essencial da sua [rotina diária](https://nation.marketo.com/t5/champion-program-blogs/my-marketo-morning-routine-tips-for-driving-marketing-operation/ba-p/247508){target="_blank"}. Embora a [seção Notificações](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/notification-types.html){target="_blank"} (localizada no canto superior direito da interface [!DNL Marketo Engage]) seja o local em que você começará a encontrar e investigar os problemas frequentes de sincronização, há uma dica profissional que pode ajudá-lo a gerenciar a integridade da instância de maneira organizada. [!DNL Adobe] Marketo Champion (2019-2022), Amy Goldfine recomenda que os usuários administradores mantenham um log dos erros de sincronização do CRM para facilitar a solução de problemas.

![Captura de tela da guia Erros de sincronização](/help/marketo-tutorial-inherited-instance/_assets/Marketo_Engage_Admin_Salesforce_Sync_Errors_Tab.png)

## Por que manter um registro de Erros de Sincronização do CRM?

Ao registrar os erros de Sincronização do CRM, os administradores do [!DNL Marketo Engage] podem examinar os problemas e as tendências com os administradores do CRM para corrigir a causa raiz. Siga as etapas abaixo para documentar seus problemas de Sincronização do CRM para sua instância.

## Como manter um log de erros de sincronização do CRM

Antes de começar, baixe o [modelo de Log de Erros de Sincronização do CRM](/help/marketo-tutorial-inherited-instance/_assets/downloads/Adobe-Marketo-Engage_CRM-Sync-Error-Log-Template.xlsx).

**Etapa 1:** vá para a seção *[!UICONTROL Administrador]* em [!DNL Marketo Engage]. Em *[!UICONTROL Integração]*, clique em *[!DNL Salesforce]*, *[!DNL Microsoft Dynamics]* ou *[!DNL Veeva]*, dependendo do [!DNL CRM] usado, em seguida, na guia *[!UICONTROL Erros de Sincronização]*.

**Etapa 2:** Você pode optar por [exportar os registros de erros como um  [!DNL CSV] arquivo por meio do painel [!UICONTROL Filtro]](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/salesforce-sync-errors.html#filter-sync-errors){target="_blank"}. Se você tiver poucas horas, copie e cole diretamente da guia *[!UICONTROL Erros de sincronização]*.

**Etapa 3:** Observe a data em que o erro ocorreu.

**Etapa 4:** Insira o número de registros de pessoas afetados por esse erro. (Às vezes, o CRM só emitirá um erro para uma pessoa. Às vezes, haverá muitas pessoas com o mesmo erro ao mesmo tempo.)

**Etapa 5:** Anote o endereço de email de uma pessoa afetada pelo erro. Isso facilita a referência e a discussão dos erros com o administrador do CRM.

**Etapa 6:** Colar links para o registro de pessoa em [!DNL Marketo Engage] e no [!UICONTROL Registro de Cliente Potencial/Contato do CRM] dessa pessoa.

**Etapa 7:** na última coluna, cole o texto real do erro.

## O que vem a seguir?

**Identificar códigos de erro:** Para entender os códigos de erro, procure as descrições na [tabela Códigos de Erro de Nível de Resposta](https://developers.marketo.com/rest-api/error-codes/#response_level_error_codes){target="_blank"} da documentação de desenvolvedores e localize as próximas etapas típicas para resolver os erros.

## Autores

**Amy Goldfine**\
[!DNL Adobe] Marketo Champion(2019-2022)
*Fundador, MarketingOpsAdvice.com*

![Amy Goldfine](/help/marketo-tutorial-inherited-instance/_assets/authors/Customer_Author_Amy_Goldfine.png){width="25%"}

**Amy Chiu**
*Gerenciador de marketing de adoção e retenção em[!DNL Adobe]*

![Amy Chiu](/help/marketo-tutorial-inherited-instance/_assets/authors/Adobe_Author_Amy_Chiu.png){width="25%"}
