---
title: Desenvolver um guia de governança de instância com a documentação
description: Saiba como estabelecer um procedimento robusto para criar e manter a documentação e o log de alterações do [!DNL Marketo Engage] instância. Isso não só economizará tempo para o compartilhamento de conhecimento da sua equipe, como também melhorará a integridade e a eficiência da sua instância.
feature-set: Marketo Engage
feature: Administration
role: Admin
level: Intermediate, Experienced
doc-type: Tutorial
last-substantial-update: 2023-10-16T00:00:00Z
jira: KT-14103
thumbnail: KT-14103.jpeg
hide: false
exl-id: e127b84d-ef92-4527-a0e6-a36af35b7ee0
source-git-commit: 058d26bd99ab060df3633fb32f1232f534881ca4
workflow-type: tm+mt
source-wordcount: '933'
ht-degree: 1%

---

# Desenvolver um guia de governança de instância com a documentação

Ao entrar em um [!DNL] herdado [!DNL Marketo Engage]], ela geralmente apresenta o desafio de não ter uma documentação funcional e técnica atualizada. Como administrador, estabelecer diretrizes para garantir o controle adequado da instância é uma responsabilidade principal que não pode ser ignorada. É uma das estratégias [impulsionar a eficiência à medida que você trabalha em um ambiente [!DNL Marketo Engage] instância](https://nation.marketo.com/t5/champion-program-blogs/3-tips-to-increase-your-efficiency-in-an-inherited-instance/ba-p/247582).

Este tutorial passo a passo tem como origem o [!DNL [!DNL Adobe] O Marketo Champion] (2018), Nick Hajdin, guiará você por esse processo para destacar sua configuração de instância, documentar seus principais programas operacionais e manter uma [!DNL changelog] para aplicar uma política de governança rigorosa.

## Por que desenvolver um guia e uma documentação de governança de instância para sua instância herdada?

Documentação detalhada e um [!DNL changelog] são vitais para a transferência eficiente de conhecimento e gerenciamento no [!DNL [!DNL Marketo Engage]] instância. Acompanhar as alterações e decisões tomadas durante a configuração da instância pode ajudar a:

1. Treine usuários internos com mais facilidade e de maneira escalável.
2. Criar com mais eficiência no [!DNL [!DNL Marketo Engage]] a longo prazo.
3. Mantenha a integridade e a higiene de sua instância avançando para evitar que você passe horas pesquisando emails, [trilha de auditoria](https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/audit-trail/audit-trail-overview.html), e [log de atividades](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/locate-the-activity-log-for-a-person.html) para obter contexto.
4. Economizar tempo ao transferir [!DNL [!DNL Marketo Engage]] conhecimento para um novo [!DNL [!DNL Marketo Engage]] administrador se sua equipe passar por algum giro.

## [!DNL [!DNL Marketo Engage]] guia de governança 101

Um guia de governança serve como a fonte da verdade dos requisitos de configuração da instância e do design do sistema. As principais informações recomendadas para inclusão neste documento são:

* Estruturas de programa/pasta
* Permissão de usuário e função
* Limites de comunicação
* Padrões de governança
* Treinamento interno do usuário antes de conceder a ele acesso à plataforma

## Como desenvolver e manter um guia de governança para o seu [!DNL [!DNL Marketo Engage]] instância

### Etapa 1: identificar o estado atual do guia de governança e da documentação

* **Não consigo localizar nenhuma documentação para minha instância herdada:** Se você iniciou recentemente uma nova função e não pode localizar nenhuma documentação para sua instância herdada, **ir para a etapa 2** e começar com um modelo que podemos baixar.
* **Tenho a documentação em arquivo:** Parabéns, este é um bom sinal! Revise sua relevância para ver quando a última alteração está sendo feita. Se os membros da sua equipe não estiverem fazendo a manutenção ativa, é recomendável atualizá-los e informar seus usuários internos sobre como mantê-los atualizados.

### Etapa 2: identificar os elementos a serem incluídos no [!DNL [!DNL Marketo Engage]] Documentação e [!DNL Changelogs]

O formato varia de uma plataforma baseada em nuvem para um documento compartilhado. Você pode projetar o formato que atenda às necessidades da sua organização. [Aqui está uma documentação simples e um modelo do Excel para changelog](/help/marketo-tutorial-herdado-instance/_assets/downloads/[!DNL Adobe]_Marketo_Engage_Inherited_Instance_Documentation-Changlog.xlsx) cobrindo os elementos importantes com os quais você pode começar. As melhorias incluem:

* Documentação
   * Nome do modelo de programa
   * Canal
   * Data da criação
   * Criada por
   * Finalidade do programa
   * Status
   * Vincular ao modelo do programa
   * Observação
* Changelog
   * Nome do modelo de programa
   * Data da alteração
   * Atualizado por
   * Finalidade da atualização
   * Experiência antes da alteração (incluir links/capturas de tela)
   * Experiência após a alteração (incluir links/capturas de tela)
   * URL para o programa

### Etapa 3: identificar e documentar o estado atual dos programas operacionais principais

Comece identificando os principais programas operacionais com impactos no nível da assinatura. Os exemplos incluem Gerenciamento de dados [!DNL Campaign]s, Ciclo de vida do lead, Pontuação do lead, [!DNL CRM] Sincronização e entregabilidade.

Para cada programa operacional identificado, documentar o seu estado atual. Isso inclui detalhes sobre a finalidade do programa, a configuração, as campanhas inteligentes associadas e a integração com outras ferramentas (se aplicável).

### Etapa 4: Impor [!DNL Changelog] Manutenção

A próxima etapa é estabelecer uma política de governança rigorosa para o seu [!DNL [!DNL Marketo Engage]] instância que exige &quot;[!DNL Changelog] manutenção.&quot; Essa política garante que todas as atualizações feitas nos programas operacionais em toda a instância sejam documentadas detalhadamente.

Informe sua equipe sobre a importância desses documentos e como acessá-los e atualizá-los corretamente. Pode ser útil atribuir responsabilidades para manter o log de alterações, de modo que alguns membros ou administradores designados da equipe de Operação de marketing estejam constantemente registrando alterações e fornecendo aprovações.

### Etapa 5: Centralizar a documentação

Estabeleça um local central ou repositório para armazenar toda a documentação relacionada ao [!DNL [!DNL Marketo Engage]] instância. Pode ser uma unidade compartilhada, uma pasta dedicada ou um sistema baseado em nuvem.

### Etapa 6: revisar e atualizar regularmente

Programe revisões regulares de sua documentação para garantir que ela permaneça precisa e atualizada. Pode ser facilmente ignorado durante os horários de maior movimento. Configure lembretes proativamente no seu calendário para garantir que sua equipe faça atualizações regularmente para refletir quaisquer alterações ou otimizações em seus programas operacionais.

## O que está por vir?

Introdução ao baixar este [modelo simples](/help/marketo-tutorial-herdado-instance/_assets/downloads/[!DNL Adobe]_Marketo_Engage_Inherited_Instance_Documentation-Changlog.xlsx).

Siga as etapas acima para desenvolver seu guia de governança e documentação. Ao trabalhar durante o processo, lembre-se das seguintes regras básicas:

**Atualize sua documentação existente:**
É crucial manter sua documentação atualizada. Se não tiver sido modificado nos últimos 3 anos, confirme tempo para revisar sua documentação enquanto audita sua instância.

**Compartilhar e treinar:**
Compartilhe sua documentação e [!DNL changelog] com membros da equipe relevantes e informá-los sobre como atualizar esses registros.

**Revisão Periódica:** programar o tempo para revisá-los e mantê-los durante todo o ano para incluir quaisquer novas alterações, otimizações ou ajustes à medida que ocorrerem.

Manutenção de uma documentação abrangente e atualizada para o seu [!DNL Marketo Engage] economizará tempo e esforço a longo prazo e facilitará o gerenciamento eficaz de instâncias.

### Autores(as)

**Nick Hajdin**
[!DNL [!DNL Adobe] Marketo Champion] (2018)
*[!DNL Digital Technology Senior Manager at Accenture]*

![Nick Hajdin](/help/marketo-tutorial-inherited-instance/_assets/authors/Customer_Author_Nicholas_Hajdin.png){width="30%"}

**Amy Chiu**
*Gerente de marketing de adoção e retenção,[!DNL Adobe]*

![Amy Chiu](/help/marketo-tutorial-inherited-instance/_assets/authors/Adobe_Author_Amy_Chiu.png){width=30%}
