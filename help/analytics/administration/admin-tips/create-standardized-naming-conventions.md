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
source-git-commit: 058d26bd99ab060df3633fb32f1232f534881ca4
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 80%

---

# Criar convenções de nomenclatura padronizadas

**O QUE:** As convenções de nomenclatura padronizadas se aplicam ao próprio nome da variável quando habilitadas no [!DNL Adobe Analytics] (AA) Interface do administrador e os valores transmitidos para a dimensão. (ou seja, usaríamos “page name (v1)” como o nome da variável e, para os valores de nome de página que serão transmitidos, uma estrutura/hierarquia uniforme e específica, como “sitename|homepage” ou “sitename|search|searchresults”).

**POR QUE:** as convenções de nomenclatura são uma ótima maneira de manter a uniformidade e uma interface fácil de entender para seus usuários. Se você criá-las desde o início e aplicá-las na plataforma e no código, será mais fácil dimensioná-las.

**COMO:** a interface e o documento de marcação devem corresponder ao “Nome” e à “Descrição”; isso evita que os usuários precisem buscar um documento do Excel e permite que eles entendam seus dados diretamente na interface. Também é recomendável manter tudo em letras minúsculas por questões de uniformidade.

É sempre melhor manter os nomes de página uniformes em toda a plataforma (ou nomes de tela para aplicativos). Por exemplo, você pode definir “property:section:sub section:sub sub section:unique page name” em uma variável/dimensão. Se todos esses campos forem separados em sua camada de dados, você poderá criar o nome da página diretamente no arquivo JS/Launch. Ter todos esses elementos definidos em suas próprias dimensões também pode ajudar você a detalhar propriedades ou áreas específicas do site/aplicativo com mais facilidade e entender melhor o tráfego e os fluxos.

Qualquer coisa que facilite a compreensão e descoberta de dados para os usuários, incluindo algo tão simples quanto as convenções de nomenclatura, aumentará o uso de [!DNL Adobe Analytics] e fornecer melhores insights para os negócios.

## Autores(as)

Este documento foi coescrito por:

![Christel Guidon](assets/Christel-Headshot-150.png)

Christel Guidon, Digital [!DNL Analytics] Gerente de plataforma na NortonLifeLock
[!DNL Adobe Analytics] Campeão

![Rachel Fenwick](assets/Rachel-Fenwick-150.png)

Rachel Fenwick, consultora sênior da [!DNL Adobe]
