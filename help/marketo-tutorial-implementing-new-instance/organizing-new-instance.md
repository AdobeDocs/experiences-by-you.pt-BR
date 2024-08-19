---
title: Organizar uma Nova Instância e Estabelecer Convenções de Nomenclatura
description: Saiba como configurar uma boa organização na instância do Marketo Engage, permitindo que futuros profissionais de marketing em sua organização naveguem facilmente pelos programas, modifiquem os ativos e obtenham relatórios.
role: Admin
level: Beginner
doc-type: Article
solution: Marketo Engage
duration: 0
last-substantial-update: 2024-05-03T00:00:00Z
jira: KT-14813
thumbnail: KT-14813.jpeg
exl-id: 19b3de9e-53f3-4308-b46e-7b8f756c30a0
source-git-commit: 1205848b1985a99b91f9d4d25e1a79f0df379589
workflow-type: tm+mt
source-wordcount: '1166'
ht-degree: 2%

---

# Organize uma nova instância e estabeleça convenções de nomenclatura

Como administrador de implementação de uma nova instância do Marketo Engage, você está estabelecendo a base para permitir que futuros profissionais de marketing na organização naveguem facilmente pela instância. Conhecer a estrutura de pastas de árvore e as convenções de nomenclatura manterá sua instância organizada e configurada para obter sucesso a longo prazo. Este tutorial abrange exemplos recomendados pelo Adobe e Marketo Engage Champion(2019-2020), Natalie Kremer, para ajudá-lo a [organizar as pastas e nomear os ativos de forma consistente](https://nation.marketo.com/t5/champion-program-blogs/keep-marketo-engage-organized-with-folders-and-naming/ba-p/245630){target="_blank"}.

## Por que é necessário estruturar pastas e aplicar convenções de nomenclatura?

Manter-se organizado em sua instância facilita para você e seus colegas rastrear campanhas, programas e ativos e relatar o desempenho do programa. Para organizar a árvore de navegação em sua instância e compilá-la em escala, é recomendável usar [pastas](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/understanding-folders){target="_blank"}, [convenções de nomenclatura padrão](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/programs/working-with-programs/best-practice-how-to-organize-your-programs#naming-schemes){target="_blank"} e recursos como [clonagem](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/programs/working-with-programs/best-practice-how-to-organize-your-programs#cloning){target="_blank"}.

## Como organizar uma instância do Marketo Engage

>[!VIDEO](https://video.tv.adobe.com/v/3421577/?quality=12&learn=on)

### Etapa 1 - Configuração de uma estrutura de pastas para colocar seus programas em ordem

A primeira etapa para organizar sua instância é [configurar uma estrutura de pastas](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/create-new-campaign-folder.html) para hospedar seu programa e seus ativos de maneira fácil de encontrar e ordenada.

Estas são algumas dicas rápidas ao estruturar as pastas na árvore:

* Mantenha uma estrutura de pasta simples para fins de descoberta.
* Estruturar suas pastas para refletir a estrutura de equipe da organização (por exemplo, Região ou Equipe) ou as iniciativas (por exemplo, Boletins informativos).
* Inclua rótulos com base no tempo para permitir a pesquisa e sinalizar o tempo apropriado para arquivamento (por exemplo, 2024).
   * Recomenda-se que os administradores arquivem as pastas pelo menos uma vez por ano. Usando um nome de pasta anual, você pode desativar facilmente as Campanhas inteligentes ativas e arquivar toda a pasta no final do ano.

Abaixo estão exemplos de pastas como colocar essas dicas em prática.

**Nome da Pasta na Árvore**

>[!BEGINTABS]

>[!TAB Atividades de marketing]

![Atividades de marketing de pastas](/help/marketo-tutorial-implementing-new-instance/assets/folders-marketing-activities.png)

>[!TAB Design Studio]

![Estúdio de Design de Pasta](/help/marketo-tutorial-implementing-new-instance/assets/folders-design-studio.png)

>[!TAB Banco de dados]

![Banco de Dados de Pastas](/help/marketo-tutorial-implementing-new-instance/assets/folders-database.png)

>[!ENDTABS]

### Etapa 2 - Criação de pastas nos programas

Agora, vamos aplicar a estrutura de pastas no nível do programa. Como prática recomendada, hospedar os ativos locais em subpastas ajudará a manter os programas organizados e permitirá que os usuários internos modifiquem ou relatem os programas com eficiência. As subpastas comuns incluem emails, landing pages, Campanhas inteligentes, Listas, Relatórios, etc.

**Nome da pasta dentro dos programas**
* Campanhas - *Pasta para todas as campanhas que gerenciam interações e o rastreamento de status.*
* Assets Local - *Pasta para todos os ativos específicos deste Programa.*
   * Emails
   * Páginas de aterrissagem
   * Campanhas inteligentes
   * Listas - *Necessário somente quando há Listas específicas do Programa.*
   * Forms - *Necessário somente quando há Forms específicos do Programa; a maioria das Forms são Assets Globais.*
   * Relatórios - *Necessário somente quando há Relatórios específicos do Programa.*

### Etapa 3 - Criar convenções de nomenclatura para seus programas e ativos

Depois de ter a estrutura de pastas na Árvore, você desejará nomear os programas e ativos consistentemente. Isso ocorre quando a padronização de convenções de nomenclatura seria útil para aumentar o processo de nomenclatura internamente. Estes são alguns componentes que você pode usar para estabelecer uma convenção de nomenclatura para garantir a capacidade de pesquisa:

* Abreviação do tipo de programa - Email, Conteúdo, Orientação, Webinário etc.
* Categoria - Tipo de programa - Email independente, Boletim informativo, etc.
* Datas - Data de lançamento do programa
* Descrição curta - Breve descrição sobre o programa

Agora, vamos colocar os valores na fórmula e gerar os nomes dos programas para vários tipos de programas.

#### Fórmula de nomeação do programa

| **Abreviação do Tipo de Programa** | **AAAA** | **\-** | **MM** | **\-** | **DD(Opcional)** | **Categoria** | **\-** | **Breve Descrição do Programa** |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| EM - Envio de email (Programa de email) | AAAA | \- | MM | \- | DD(Opcional) | Categoria | \- | Breve descrição do programa |
| NL - Informativo | AAAA | \- | MM | \- | DD(Opcional) | Categoria | \- | Breve descrição do programa |
| ENG - Programa de engajamento | AAAA | \- | MM | \- | DD(Opcional) | Categoria | \- | Breve descrição do programa |
| WBN - Webinário | AAAA | \- | MM | \- | DD(Opcional) | Categoria | \- | Breve descrição do programa |
| IW - Webinário interativo | AAAA | \- | MM | \- | DD(Opcional) | Categoria | \- | Breve descrição do programa |
| TS - Feira de Negócios | AAAA | \- | MM | \- | DD(Opcional) | Categoria | \- | Breve descrição do programa |
| LE - Evento ao vivo (Roadshow) | AAAA | \- | MM | \- | DD(Opcional) | Categoria | \- | Breve descrição do programa |
| UG - Grupo de usuários | AAAA | \- | MM | \- | DD(Opcional) | Categoria | \- | Breve descrição do programa |
| WC - Conteúdo do Site | AAAA | \- | MM | \- | DD(Opcional) | Categoria | \- | Breve descrição do programa |
| CS - Content Syndication | AAAA | \- | MM | \- | DD(Opcional) | Categoria | \- | Breve descrição do programa |
| LI - Importação de Lista | AAAA | \- | MM | \- | DD(Opcional) | Categoria | \- | Breve descrição do programa |
| OA - Advertising Online | AAAA | \- | MM | \- | DD(Opcional) | Categoria | \- | Breve descrição do programa |
| PPC - Pagamento por clique | AAAA | \- | MM | \- | DD(Opcional) | Categoria | \- | Breve descrição do programa |

| **Exemplos** |
| --- |
| Conteúdo fechado ES 2023-10 - Informe oficial XYX |
| WC-2023-10- Webinário mensal - Estudo de caso da ABC |

#### Fórmula de nomeação de ativos

Em um nível, é melhor não repetir o nome do programa e usar identificadores curtos e genéricos para uso futuro de clonagem. Estas são algumas dicas rápidas para você ter em mente:

* Numere os ativos com base em sua sequência no processo do programa.
* Use &quot;-&quot; (hífen) para separar os componentes de nomenclatura em vez de &quot;.&quot;(ponto) ou &quot;\_&quot;(sublinhado).
   * Por quê? O Marketo Engage usa um ponto para separar o Nome do programa do Nome da campanha. Usar &quot;\_&quot; impedirá que você o veja quando o ativo estiver com hiperlink.
* Use acrônimos padrão nos nomes de ativos para encurtar a referência e ainda permitir um reconhecimento fácil.

Com isso em mente, aplicaremos essas dicas aos seguintes ativos e criaremos fórmulas para gerar nomes:

##### Nomeie os ativos com base na sequência no processo do programa

| **Sequência no Processo do Programa** | **\-** | **Descrição** |
| --- | --- | --- |
| 01 | \- | Descrição |
| 02 | \- | Descrição |
| 03 | \- | Descrição |

| **Exemplos: Smart List** |
| --- |
| 01-Enviar e-mail |
| 02-Aberto |
| 03-Clicado |
| 04-Formulário preenchido |
| 05-Influenciado (Sucesso do programa) |
| 06-Cancelamento de assinatura |

##### Nomeie os ativos com a abreviação do tipo de ativo

| **Abreviação do tipo de ativo** | **Tipo de ativo** | **\-** | **Descrição da meta** |
| --- | --- | --- | --- |
| LP - Página inicial | LP | \- | Descrição da meta |
| EMAIL - Email (saída) | EMAIL | \- | Descrição da meta |
| ALERTA - Alerta por email | ALERTA | \- | Descrição da meta |
| WF - Formulário web | WF | \- | Descrição da meta |
| EXCL - Lista de exclusões | EXCL | \- | Descrição da meta |
| SLST - Lista inteligente | SLST | \- | Descrição da meta |
| LST - Lista estática | LISTA | \- | Descrição da meta |

| **Exemplos** |
| --- |
| LP-Registro |
| LP-ThankYou |
| E-MAIL de saída |
| EMAIL-informativo |
| EMAIL - Convite |
| Lembrete de EMAIL |
| EXCL-Concorrentes |

##### Nomeie os arquivos baixáveis (.pdf) com a abreviação do tipo de ativo

| **Tipo de ativo** | **Descrição do conteúdo** | **\-** | **Abreviação do tipo de ativo** | **.** | **PDF** |
| --- | --- | --- | --- | --- | --- |
| WP - White paper | Descrição do conteúdo | \- | WP | . | pdf |
| CS - Estudo de caso | Descrição do conteúdo | \- | CS | . | pdf |
| DS - Folha de dados | Descrição do conteúdo | \- | DS | . | pdf |

| **Exemplos: Arquivos de PDF baixáveis** |
| --- |
| XYZ-Gadget-DS.pdf |
| Acme-Company-CS.pdf |
| How-XYZ-Gadgets-make-life-easier-WP.pdf |

>[!CAUTION]
>
>Ao nomear arquivos nos exemplos acima, não use espaços e evite o uso de sublinhados &quot;\_&quot;

## O que vem a seguir?

* Baixe a Planilha: [Organização de Marketo Engage e Convenções de Nomenclatura](./assets/adobe-marketo-engage-organization-and-naming-conventions.xlsx){target="_blank"} para dar suporte à criação da estrutura de pastas e convenções de nomenclatura.
* Depois de determinar os componentes necessários em sua convenção de nomenclatura padrão, considere criar fórmulas em uma Planilha do Google ou no Microsoft Excel. Para uso futuro, basta inserir seus valores na planilha para gerar os nomes do programa.
* Depois de se alinhar em uma estrutura geral de pastas, é hora de pensar nos modelos necessários com base nos casos de uso mais frequentes e nas solicitações mais comuns que sua equipe recebe. Em seguida, comece a criar seu primeiro modelo de programa. Leia para começar com [modelos de programa do Adobe Marketo Engage](https://business.adobe.com/blog/how-to/get-started-with-marketo-engage-program-templates){target="_blank"}.

### Autores

{{natalie-kremer}}

{{amy-chiu}}
