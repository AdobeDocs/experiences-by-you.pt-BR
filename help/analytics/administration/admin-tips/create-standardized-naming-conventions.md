---
title: Criar convenções de nomenclatura padronizadas
description: As convenções de nomenclatura padronizadas se aplicam ao próprio nome da variável quando habilitadas na interface do administrador do AA e aos valores transmitidos para a dimensão.
solution: Analytics
feature-set: Analytics
feature: Implementation Basics
topic: Administration
role: Admin
level: Beginner
doc-type: article
thumbnail: 10531.jpg
kt: 10531
exl-id: 79cec21e-2b52-4e7b-88ad-db137a8cef4e
product_v2:
  - id: e55547f1-a1ff-40c6-8978-026e40ab7fa4
    internal-label: Analytics
feature_v2:
  - id: a421fb65-2c82-457a-921c-28c46b697a39
    internal-label: Analytics basics
subfeature_v2:
  - id: c24fe15a-643a-47bd-8278-5e027df49785
    internal-label: Implementation basics
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
    internal-label: Beginner
source-git-commit: 749b293ab38b8ea5a5f72517bd5c3455399137c2
workflow-type: tm+mt
source-wordcount: '323'
ht-degree: 0%
---
# Criar convenções de nomenclatura padronizadas

**O QUE:** as convenções de nomenclatura padronizadas se aplicam ao próprio nome da variável quando habilitadas na interface do administrador do [!DNL Adobe Analytics] (AA) e aos valores transmitidos para a dimensão. (ou seja, os nomes de página seriam &quot;page name (v1)&quot; como um nome de variável, e os valores de nome de página transmitidos deveriam ser uniformes e seguir uma estrutura/hierarquia específica, como &quot;sitename|homepage&quot; ou &quot;sitename|search|searchresults&quot;).

**POR QUE:** as convenções de nomenclatura são uma ótima maneira de manter a uniformidade e uma interface fácil de entender para seus usuários. Se você criá-los desde o início e aplicá-los na plataforma e no código, será mais fácil dimensioná-los.

**COMO:** a interface e o documento de marcação devem corresponder ao &quot;Nome&quot; e à &quot;Descrição&quot; - isso evita que os usuários precisem buscar um documento do Excel e permite que eles entendam seus dados diretamente na interface. Também é recomendável manter tudo em letras minúsculas por questões de consistência.

É sempre melhor manter os nomes de página consistentes em toda a plataforma (ou nomes de tela para aplicativos). Por exemplo, você pode definir &quot;`property:section:sub section:sub sub section:unique page name`&quot; em uma variável/dimensão. Se todos esses campos forem separados em sua camada de dados, você poderá criar o nome da página diretamente no arquivo JS/Launch. Ter todos esses elementos definidos em suas próprias dimensões também pode ajudar você a detalhar propriedades ou áreas específicas do site/aplicativo com mais facilidade e entender melhor o tráfego e os fluxos.

Qualquer coisa que facilite a compreensão e descoberta de dados para os usuários, incluindo algo tão simples quanto as convenções de nomenclatura, aumentará o uso do [!DNL Adobe Analytics] e fornecerá melhores insights para os negócios.

## Autores

Este documento foi coescrito por:

![Christel Guidon](assets/Christel-Headshot-150.png)

Christel Guidon, gerente de plataforma [!DNL Analytics] digital do NortonLifeLock
[!DNL Adobe Analytics] Especialista

![Rachel Fenwick](assets/Rachel-Fenwick-150.png)

Rachel Fenwick, consultora sênior do [!DNL Adobe]
