---
title: Sincronizando Campos dos Conectores CRM Nativos
description: Saiba como simplificar sua integração inicial com o CRM selecionando estrategicamente os campos CRM essenciais para o Marketo Engage usar. Realize o exercício Dicionário de dados para identificar os campos necessários para uma sincronização perfeita do CRM que ajude as equipes de vendas e marketing a permanecerem alinhadas.
role: Admin
level: Beginner
doc-type: Article
solution: Marketo Engage
duration: 0
last-substantial-update: 2024-05-04T00:00:00Z
jira: KT-14811
thumbnail: KT-14811.jpeg
exl-id: 42b7ca3d-e445-4c11-ad3d-d4e70c101c8e
source-git-commit: 1205848b1985a99b91f9d4d25e1a79f0df379589
workflow-type: tm+mt
source-wordcount: '1567'
ht-degree: 0%

---

# Sincronizar campos dos conectores CRM nativos

Você está usando o Salesforce ou o Microsoft Dynamics em sua organização? Em caso positivo, com conectores CRM nativos do Marketo Engage (ou seja, Salesforce, Microsoft Dynamics e Veeva), é possível coordenar as atividades de marketing e vendas compartilhando perfeitamente informações relevantes entre o Marketo Engage e o CRM. Antes de configurar a sincronização inicial do CRM, identifique os campos que gostaria de sincronizar entre os dois sistemas para manter o banco de dados do Marketo Engage limpo.

Saiba mais sobre como conduzir esse exercício com as práticas recomendadas sugeridas pelo Adobe Professional Services. Siga as instruções para entender Campos padrão e Campos personalizados e documentar os relacionamentos entre o Marketo Engage e o seu CRM.

## Identifique os campos a serem sincronizados antes de integrar seu CRM ao Marketo Engage

Ao integrar seu CRM ao Marketo Engage, você provavelmente não precisará sincronizar todos os campos do CRM com o Marketo Engage. Ser estratégico com relação aos campos necessários pode ajudar sua instância do Marketo Engage a processar o fluxo de dados com mais eficiência.

A sincronização inicial entre seu sistema de Marketo Engage e CRM fará associações automaticamente para a maioria dos campos padrão existentes (ou seja, Email, Nome/Sobrenome, Empresa etc.). Além disso, o conector também sincroniza [Campos Personalizados](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/field-management/custom-field-type-glossary){target="_blank"} para seus Clientes Potenciais, Contatos, Contas e Oportunidades, criando novos campos no Marketo Engage que são mapeados automaticamente para esses campos do seu CRM.

Identificar e organizar os campos que você gostaria de sincronizar do seu CRM antes de executar a sincronização inicial é uma etapa crítica no processo de configuração do Conector nativo. Nos referimos a isso como um exercício de Dicionário de dados, que ajuda a minimizar o número de campos duplicados criados e fazer com que qualquer etapa subsequente de remapeamento seja realizada da maneira mais suave possível. Normalmente, esse exercício envolve informações das equipes de marketing e vendas e do seu administrador de CRM para garantir que apenas campos relevantes sejam sincronizados com a instância do Marketo Engage.

## Crie seu dicionário de dados

Geralmente, a prática recomendada é sincronizar apenas campos do CRM que serão necessários para fins de marketing. Comece com este exercício para organizar os campos do seu CRM que precisarão ser mapeados para Marketo Engage e executar a sincronização inicial do CRM corretamente na primeira vez.

>[!NOTE]
>Se você tiver campos personalizados em seu CRM que já tenham um campo personalizado equivalente no Marketo Engage antes de iniciar a sincronização inicial, um novo campo &quot;duplicado&quot; será criado no Marketo Engage para o campo CRM. Você pode remapear o campo do CRM para o campo de Marketo Engage original e ocultar o campo duplicado quando a sincronização inicial estiver concluída, mas você precisa entrar em contato com o [Suporte ao Cliente do Adobe](https://experienceleague.adobe.com/en/docs/customer-one/using/home#create-a-support-ticket-with-admin-console){target="_blank"} para fazer isso. Consulte a etapa 7 para obter mais detalhes.

**Etapa 1:** crie uma lista resumida dos campos disponíveis no momento em seu CRM e marque se você deseja que eles apareçam no Marketo Engage.

* Inclua feedback de seu administrador de CRM e das equipes de marketing e vendas no processo de tomada de decisão.
* Documente os nomes da API e os tipos de campo para cada campo
* Determine qual nível de Marketo Engage de acesso deve ter para esses campos (ou seja, Somente leitura ou Leitura-gravação)


**Etapa 2:** Revise a [seção Admin > Gerenciamento de Campos](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/field-management/view-field-mappings-between-marketo-and-salesforce){target="_blank"} da sua instância do Marketo Engage para Identificar todos os campos personalizados criados anteriormente diretamente no sistema que você deseja incluir na sincronização.

* Documente os nomes da API e os tipos de campo de cada campo.
* Indique campos que já têm um campo equivalente em seu CRM.
* Indique campos que ainda não têm um campo equivalente em seu CRM.


**Etapa 3:** Comece a criar o Dicionário de Dados com os campos de mapa padrão

* Como o Marketo Engage usa um banco de dados simples, é recomendável formatar o dicionário de dados da seguinte maneira:

   * Primeira coluna: Marketo Engage Nomes de campos
   * Segunda coluna: nomes da API Marketo Engage
   * Terceira Coluna: [Tipo de Campo Marketo Engage](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/field-management/custom-field-type-glossary){target="_blank"} (isto é, Booleano, Moeda, Data, etc.)
   * Em colunas subsequentes, repita para os tipos de objeto do CRM (cliente potencial, contato, conta, oportunidade) com uma coluna adicional para o nível de acesso que você gostaria que o Marketo Engage tivesse (ou seja, Leitura, Gravação, Edição)
  <br>

  Aqui está um exemplo de como ele seria:
  ![Tabela do dicionário de dados](/help/marketo-tutorial-implementing-new-instance/assets/data_dictionary.png){width="100%" zoomable="yes"}


* Comece adicionando os campos padrão que serão mapeados automaticamente para o seu CRM:

   * [Salesforce](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/default-salesforce-field-mapping){target="_blank"}
   * [Microsoft Dynamics](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/microsoft-dynamics-sync-details/default-dynamics-field-mapping){target="_blank"}
   * [Veeva](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/veeva-crm-sync/sync-details/default-veeva-field-mapping){target="_blank"}

* Confirme se cada campo padrão em Marketo Engage corresponde ao campo no CRM com o qual você deseja sincronizar. Por exemplo, o campo &quot;Inscrição cancelada&quot; no Marketo Engage pode ser o campo &quot;Recusa de email&quot; no seu CRM.
* Ajuste o nome da API do CRM, os privilégios e o [tipo de dados](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/field-management/custom-field-type-glossary){target="_blank"} onde necessário.

**Etapa 4:** adicionar mais campos ao Dicionário de Dados

* Inclua o Nome de exibição, os privilégios de CRM desejados e o tipo de dados para cada campo.
* Se existir um campo no CRM, mas não no Marketo Engage, preencha a exibição do Marketo Engage e os nomes da API com os mesmos valores do campo CRM.
* Se existir um campo no Marketo Engage, mas não no CRM, preencha o nome de exibição do CRM com o valor desejado, mas deixe o nome da API do CRM em branco até que o campo seja criado.
* Se existirem campos equivalentes em ambos os sistemas, inclua-os na mesma linha e indique que eles precisam ser remapeados na seção &quot;Notas&quot; na extremidade direita da folha do Dicionário de dados.

>[!NOTE]
>Se você estiver planejando criar um campo Filtro de sincronização ([Salesforce](https://nation.marketo.com/t5/product-blogs/instructions-for-creating-a-custom-sync-rule/ba-p/242758){target="_blank"} | [Microsoft Dynamics](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/custom-dynamics-sync-filter-details/create-a-custom-dynamics-sync-filter){target="_blank"}), certifique-se de incluí-lo nesta etapa, mas deixe os nomes de API em branco até que o campo seja criado em seu CRM.

**Etapa 5:** Analise o Dicionário de Dados com o Administrador do CRM

* Crie campos no CRM para aqueles que já existem no Marketo Engage e atualize o Dicionário de dados com os nomes de exibição e API do novo campo do CRM.
* Executar mapeamento de campos entre objetos de Cliente Potencial e de Contato no seu CRM ([Salesforce](https://nation.marketo.com/t5/product-blogs/instructions-for-creating-a-custom-sync-rule/ba-p/242758){target="_blank"} | [Microsoft Dynamics](https://community.dynamics.com/blogs/post/?postid=8a91d93e-2181-45dd-a8fb-1092010bc8f1){target="_blank"}). Quando um cliente potencial é convertido em um Contato, isso garante que os campos possam ser consolidados em um único campo no Marketo Engage.
* Certifique-se de que o Perfil de sincronização do Marketo tenha privilégios apropriados para cada campo, conforme observado no Dicionário de dados:
   * [Definir permissões de perfil no Salesforce](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited#set-profile-permissions){target="_blank"}
   * [Definir permissões de perfil no Microsoft Dynamics](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-2-of-3-set-up#create-application-user-in-microsoft){target="_blank"}
   * [Definir permissões de perfil no Veeva](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/veeva-crm-sync/setup/step-2-of-3-create-a-veeva-crm-user-for-marketo-engage#set-profile-permissions){target="_blank"}

**Etapa 6:** Executar a sincronização inicial

* Verifique se todos os campos que você deseja sincronizar com o Marketo Engage têm os privilégios apropriados em seu CRM, conforme definido pelo dicionário de dados.
* Verifique se todos os campos que você **não** deseja sincronizar com o Marketo Engage estão [ocultos do Perfil de Sincronização do Marketo](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/hide-a-salesforce-field-from-the-marketo-sync){target="_blank"}. É muito mais fácil adicionar novos campos à sincronização depois do que remover campos que foram sincronizados involuntariamente.
* Você está conectando seu CRM ao campo Filtro de sincronização? Se você sincronizar com o Salesforce, entre em contato com o Suporte ao cliente do Adobe para garantir que a funcionalidade de filtro esteja ativada antes de iniciar sua sincronização inicial.


**Etapa 7:** revise a seção Gerenciamento de Campo no Marketo Engage

* Confirme/atualize os Nomes de exibição e API dos novos campos sincronizados.
* Identifique quaisquer campos duplicados que possam exigir remapeamento. Campos duplicados ocorrem em alguns cenários:
   * Os campos personalizados no CRM criariam um novo campo (potencialmente duplicado) no Marketo Engage na primeira vez que fossem sincronizados se um campo equivalente já existisse no Marketo Engage.
   * Campos personalizados exclusivos ao Marketo (ou seja, um campo criado diretamente no Marketo Engage) e você pode ter um campo equivalente sincronizado no CRM.



**Etapa 8:** Entre em contato com o Suporte ao Cliente da Adobe para executar o remapeamento se campos duplicados forem exibidos

* Entre em contato com o Suporte com as seguintes informações para os campos que precisam ser remapeados:
   * Exibir nomes de &amp; API para novos campos duplicados criados pelo CRM.
   * Nome para exibição do campo Marketo Engage para o qual você deseja que o campo do CRM mapeie.
   * Consulte este exemplo [AQUI](https://nation.marketo.com/t5/knowledgebase/re-mapping-sfdc-marketo-fields/ta-p/299284){target="_blank"}.
* Quando o remapeamento estiver concluído, revise os nomes de API dos campos remapeados em Marketo Engage e atualize os valores na coluna &quot;Nome de API&quot; do dicionário de dados para garantir que ela contenha as informações mais precisas.

## O que vem a seguir?

* Crie seu Dicionário de Dados para organizar seus campos para a integração com o CRM.
* Familiarizar-se com o processo de sincronização inicial do seu CRM

>[!BEGINTABS]

>[!TAB Salesforce]

Saiba como o Marketo Engage e o Salesforce se unem para manter seus dados de vendas e marketing sincronizados.

>[!VIDEO](https://video.tv.adobe.com/v/3424719/?learn=on)

+++**Links usados no vídeo:**

* [Entendendo a sincronização do Salesforce](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/salesforce-sync/understanding-the-salesforce-sync){target="_blank"}

* [Adicionar campos do Marketo ao Salesforce (Enterprise/Unlimited)](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited){target="_blank"}

* [Criar um usuário do Marketo no Salesforce (Enterprise/Unlimited)](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited){target="_blank"}

* [Conecte o Marketo e o Salesforce(Enterprise/Unlimited)](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited){target="_blank"}

* [Os usuários precisariam Configurar o Aplicativo Conectado no lado do Salesforce antes de prosseguir para o Marketo e o Salesforce Sync.](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/salesforce-sync/log-in-using-oauth-2-0){target="_blank"}

* [Status de sincronização do Salesforce](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/salesforce-sync/salesforce-sync-status){target="_blank"}

* [Ocultar e Reexibir um Campo](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/field-management/hide-and-unhide-a-field){target="_blank"}

* [Tutorial: Saiba mais sobre como sincronizar o Marketo com seu CRM](https://experienceleague.adobe.com/en/docs/marketo-learn/tutorials/lead-and-data-management/crm-sync-learn){target="_blank"}

+++

>[!TAB Microsoft Dynamics]

Saiba como a sincronização do Microsoft Dynamics 365 funciona e configure a configuração corretamente para permitir que os dois sistemas se comuniquem entre si.

>[!VIDEO](https://video.tv.adobe.com/v/3424737/?learn=on)

+++**Links usados no vídeo:**

* [Noções básicas sobre a sincronização do Microsoft Dynamics](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/understanding-the-microsoft-dynamics-sync){target="_blank"}

* [Baixar a Solução Marketo de Gerenciamento de Clientes Potenciais](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/sync-setup/download-the-marketo-lead-management-solution){target="_blank"}

* [Atualizar a Solução Marketo para Microsoft Dynamics](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/sync-setup/update-the-marketo-solution-for-microsoft-dynamics){target="_blank"}

* [Conceder consentimento para a ID do cliente e o registro do aplicativo](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/sync-setup/grant-consent-for-client-id-and-app-registration)

* [Validar a sincronização do Microsoft Dynamics](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/sync-setup/validate-microsoft-dynamics-sync){target="_blank"}

* [Status de sincronização](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/microsoft-dynamics-sync-details/sync-status){target="_blank"}

* [Corrigir Problemas De Sincronização De Validação Do Dynamics](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/fix-dynamics-validation-sync-issues){target="_blank"}

* [Criar um Filtro de Sincronização do Dynamics Personalizado](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/custom-dynamics-sync-filter-details/create-a-custom-dynamics-sync-filter.html){target="_blank"}

* [Exibir a URL do Serviço de Organização](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/sync-setup/view-the-organization-service-url){target="_blank"}

* [Editando Campos para Sincronização Antes de Excluí-los no Dynamics](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/microsoft-dynamics-sync-details/editing-fields-to-sync-before-deleting-them-in-dynamics){target="_blank"}

* [Tutorial: Saiba mais sobre como sincronizar o Marketo com seu CRM](https://experienceleague.adobe.com/en/docs/marketo-learn/tutorials/lead-and-data-management/crm-sync-learn){target="_blank"}

+++

>[!ENDTABS]

### Autores

{{peter-livadas}}

{{amy-chiu}}
