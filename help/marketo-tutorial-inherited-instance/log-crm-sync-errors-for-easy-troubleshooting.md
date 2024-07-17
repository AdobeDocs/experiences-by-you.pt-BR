---
title: Registrar erros de sincronização do CRM para facilitar a solução de problemas
description: Saiba como usar um log de erros de sincronização do CRM para investigar problemas de sincronização do CRM e mantê-lo em execução sem problemas.
feature-set: Marketo Engage
feature: Administration
role: Admin
level: Intermediate, Experienced
doc-type: Tutorial
last-substantial-update: 2023-10-16T00:00:00Z
jira: KT-13875
thumbnail: KT-13875.jpeg
hide: false
exl-id: 6a38f5dd-5d25-43d8-a1d3-e75ab396e555
source-git-commit: b2e05ff39e065691dda530ed17762a55cf2e6778
workflow-type: tm+mt
source-wordcount: '408'
ht-degree: 0%

---

# Registrar erros de sincronização do CRM para facilitar a solução de problemas

Como administrador do [!DNL Marketo Engage], verificar se sua instância está sincronizada com o CRM deve ser uma parte essencial da sua [rotina diária](https://nation.marketo.com/t5/champion-program-blogs/my-marketo-morning-routine-tips-for-driving-marketing-operation/ba-p/247508){target="_blank"}. Embora a [seção Notificações](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/notification-types.html){target="_blank"} (encontre-a no canto superior direito da interface do [!DNL Marketo Engage]) seja onde você começará a encontrar e investigar problemas frequentes de sincronização, há uma dica profissional que pode ajudá-lo a gerenciar a integridade da instância de maneira organizada. Especialista em Marketo do [!DNL Adobe] (2019-2022), Amy Goldfine recomenda que os usuários administradores mantenham um log dos erros de Sincronização do CRM para facilitar a solução de problemas.

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

## O que está por vir?

**Identificar Códigos de Erro:** Para entender os códigos de erro, procure as descrições na [tabela Códigos de Erro de Nível de Resposta](https://developers.marketo.com/rest-api/error-codes/#response_level_error_codes){target="_blank"} da documentação de desenvolvedores e localize as próximas etapas típicas para resolver os erros.

## Autores

**Amy Goldfine**\
[!DNL Adobe] Marketo Champion(2019-2022)
*Fundador, MarketingOpsAdvice.com*

![Amy Goldfine](/help/marketo-tutorial-inherited-instance/_assets/authors/Customer_Author_Amy_Goldfine.png){width="25%"}

**Amy Chiu**
*Gerenciador de marketing de adoção e retenção em[!DNL Adobe]*

![Amy Chiu](/help/marketo-tutorial-inherited-instance/_assets/authors/Adobe_Author_Amy_Chiu.png){width="25%"}
