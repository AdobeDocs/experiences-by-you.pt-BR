---
title: Introdução à governança de instâncias e documentação
description: Conheça as estratégias essenciais e as práticas recomendadas para começar a usar a governança e a documentação do Marketo Engage. Descubra como criar documentação escalável, otimizar o treinamento de usuários e garantir a criação com uma estrutura na sua instância do Marketo Engage.
role: Admin
level: Beginner
doc-type: Article
solution: Marketo Engage
duration: 0
last-substantial-update: 2024-05-08T00:00:00Z
jira: KT-14815
thumbnail: KT-14815.jpeg
source-git-commit: 47ab8875bc4e41595cd40550330e43a88357b68d
workflow-type: tm+mt
source-wordcount: '815'
ht-degree: 0%

---


# Introdução à governança de instâncias e documentação

Uma boa documentação pode ser quase tão importante quanto a própria implementação da instância real. Um guia de governança é um recurso essencial que descreve os detalhes de configuração da instância do Marketo Engage, abrangendo tópicos como estruturas de programa/pasta, limites de comunicação e muito mais. Este documento dinâmico é uma referência para o administrador de Marketo Engage ou usuários avançados, mostrando práticas recomendadas específicas e padrões de governança personalizados para sua instância e organização de Marketo Engage.

Mas não pára por aí. Sua equipe pode precisar de documentos complementares de capacitação ou materiais de treinamento para melhorar sua proficiência com o Marketo Engage. Esses recursos podem incluir exercícios interativos, questionários de acesso ou diretrizes sobre ações permitidas no Marketo Engage, beneficiando todos os usuários do Marketo Engage na organização. Seja criando um guia de governança abrangente ou documentando os principais aspectos de configuração inicialmente, registrar as decisões tomadas durante a integração é fundamental para garantir o sucesso com o Marketo Engage para a sua equipe atual e as futuras gerações de novas contratações.

Ao entender a importância da documentação e do controle, este tutorial aborda as práticas recomendadas fornecidas por colegas especialistas [Introdução à documentação de treinamento e governança do Marketo Engage](https://nation.marketo.com/t5/product-blogs/getting-started-on-your-marketo-governance-and-training/ba-p/242421){target="_blank} e [Como documentar sua instância?](https://nation.marketo.com/t5/product-discussions/how-do-you-document-your-instance/td-p/72877){target="_blank} para ajudar você a colocar um processo em vigor e manter a documentação relevante para os usuários internos.

## Por que documentar alterações e decisões durante a implementação da instância é essencial

Aborde sua documentação do Marketo Engage como se você estivesse orientando um novo funcionário não familiarizado com a tecnologia a integrar-se à instância. É fácil ignorar o conhecimento fundamental quando você ganha experiência com o Marketo Engage. Como administrador, você deve garantir que seus documentos de ativação e governança atendam aos iniciantes. Para facilitar o aprendizado de novos usuários, um método prático está incorporando definições e práticas recomendadas diretamente no material de treinamento.

A criação da documentação da instância durante a configuração da instância oferece vários benefícios:

* Simplifique o processo de treinamento para novos usuários de maneira escalável.
* Facilite o desenvolvimento de programas de longo prazo no Marketo Engage, desenvolvendo uma base de documentação sólida.
* Mantenha a integridade e a organização da sua instância ao longo do tempo.
* Facilite a transição para novos administradores de Marketo Engage em caso de mudança de equipe.

Em última análise, anotar as decisões que você toma durante a implementação ajudará você e sua equipe a serem bem-sucedidos com o Marketo Engage, sem depender de uma ou algumas pessoas para aplicar os processos.

## Como criar a governança e a documentação da instância do Marketo Engage

### Etapa 1 - Descrever os principais tópicos na documentação da instância

Definir uma configuração de padrões do que deve ser documentado e do que não é necessário documentar. Isso permitirá que a organização adote o processo. À medida que você expande o documento, é importante documentar o motivo por trás da configuração. Isso ajuda outros administradores, assim como você, a evitar perder tempo com decisões que não produziram resultados.

Guie seu plano de governança e documentação começando com o exemplo de outline abaixo:

1. A finalidade do Marketo Engage para nossa organização
1. Finalidade desta documentação
1. O processo para manter/fazer alterações no Guia de governança
1. Configuração Administrativa
   * Assinatura(s)
   * Espaços de trabalho e partições (se aplicável)
   * Configuração técnica (DKIM/SPF/Munchkin)
   * Funções e responsabilidades*
   * Usuários*
   * Configurações inteligentes de campanha/email/programa
   * Limites de comunicação
   * Segurança
   * Canais*
   * Tags
1. Estrutura de dados
   * Estrutura do campo
   * Objetos personalizados
1. Programas Operacionais
   * Pontuação de pessoa
   * Ciclo de vida da pessoa
   * Gerenciamento de dados
1. Criação na instância do Marketo Engage
   * [Centro de excelência (COE)](https://business.adobe.com/blog/perspectives/center-of-excellence-top-10-questions-to-ask-yourself){target="_blank}
   * Estrutura de pastas
   * Convenções de nomenclatura
   * Organização do programa
   * Modelos de programa*
   * Ativos do Design Studio (modelos de email, modelos de landing page, trechos, formulários)
   * Processos padronizados
   * Listas de verificação
   * Segmentações
   * Políticas de arquivamento
   * Central de assinaturas
1. Integração do CRM
   * Como a sincronização funciona
   * Sincronização de campanha
   * Dicionário de dados
1. Outras integrações
1. GDPR e conformidade

\* No mínimo, sua documentação deve incluir os detalhes dos usuários e funções, modelos de programas e canais assim que a configuração for concluída.

### Etapa 2 - Criar um Log de Alterações

Outra maneira crítica de governança de instâncias é criar um Changelog e impor sua utilização. Sempre que você alterar uma configuração na seção &quot;Administrador&quot; ou em um programa operacional, a equipe deverá anotá-la em um local centralizado, como uma planilha compartilhada. Isso pode ajudá-lo a lembrar por que você fez uma alteração e como ela era antes. Os campos que você deve documentar no Changelog incluem:

1. Data
1. Nome do programa
1. Link do programa
1. Nome da campanha inteligente
1. Link do Campaign inteligente
1. Alteração feita
1. Motivo da alteração
1. Quem fez a alteração

## O que está por vir?

* Baixe o [documentação de amostra e Changelog](/help/marketo-tutorial-implementing-new-instance/assets/template-adobe-marketo-engage-instance-documentation.xlsx) e adaptá-los com base nas necessidades de sua organização.
* Armazene a documentação em uma plataforma acessível na qual sua organização prefira fazer referência e atualizar regularmente. Por exemplo, alguns Marketo Engage Champions usam Confluence (de Atlassian) ou Excel Spreadsheet.
* Certifique-se de que cada regra criada para o controle tenha um proprietário para aplicá-la e adaptar a documentação, mantendo-a atualizada ao longo do tempo.

### Autor

{{amy-chiu}}