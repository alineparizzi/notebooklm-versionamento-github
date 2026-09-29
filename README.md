# Gestão de Versionamento, Arquitetura de Branching e Automação no GitHub

## 1. Contexto e Objetivos
- Assunto escolhido: Versionamento com Github
- Por que escolhi: É um tema que preciso aprimorar
- Objetivos de estudo: Aprender gitflow e githubflow para definir a melhor forma de controlar as versões de uma aplicação

## 2. Curadoria de Fontes
Utilizei 46 fontes no NotebookLM para ampliar o contexto do caderno. Para esta entrega, destaco 5 fontes principais (seção 2.1), que concentram o núcleo do miniguia. As 41 restantes estão catalogadas na seção 2.2, agrupadas por tipo de material.

### 2.1. Principais fontes
1. **Arquitetura e Gestão de Versionamento de Software no GitHub: Estratégias Estruturadas para Features e Bugfixes** - [Documento Markdown]
2. **Git Branching Strategies: GitFlow, Github Flow, Trunk Based... - Wingify** - https://wingify.com/blog/git-branching-strategies/
3. **Trunk-Based Development vs Git Flow - DEV Community** - https://dev.to/acestus/trunk-based-development-vs-git-flow-2kb5
4. **GitHub - googleapis/release-please: generate release PRs based on the conventionalcommits.org spec** - https://github.com/googleapis/release-please
5. **Release Please: automation of your GitHub releases | Padok - Theodo** - https://www.theodo.com/blog/automate-your-github-releases-with-release-please

### 2.2. Fontes Complementares
1. **Adding Tags, Versioning, and Releases in Github | Git & Source Control #13** - [Vídeo no YouTube]
2. **Automating Elixir Releases with Release Please | Blog** - https://elixirschool.com/blog/managing-releases-with-release-please
3. **Backport merged pull requests to selected branches · Actions · GitHub Marketplace** - https://github.com/marketplace/actions/backport-merged-pull-requests-to-selected-branches
4. **Cherry-pick changes with Git - GitLab Docs** - https://docs.gitlab.com/topics/git/cherry_pick/
5. **Comandos essenciais de terminal para desenvolvedores - Gerenciamento de arquivos e diretórios** - [Vídeo no YouTube]
6. **Como clonar/copiar apenas um arquivo ou diretório do repositório remoto git | Code Pitch #3** - [Vídeo no YouTube]
7. **Controle de Versão, Git e GitHub - IX** - [Vídeo no YouTube]
8. **Controle de Versão, Git e GitHub - VIII** - [Vídeo no YouTube]
9. **Controle de Versão, Git e GitHub - X** - [Vídeo no YouTube]
10. **Controle de Versão, Git e GitHub - XI** - [Vídeo no YouTube]
11. **Controle de Versão, Git e GitHub - XII** - [Vídeo no YouTube]
12. **Controle de Versão, Git e GitHub - XIII** - [Vídeo no YouTube]
13. **Controle de Versão, Git e GitHub - XIV** - [Vídeo no YouTube]
14. **Controle de Versão, Git e GitHub - XV** - [Vídeo no YouTube]
15. **Controle de Versão, Git e GitHub - XVI** - [Vídeo no YouTube]
16. **Controle de Versão, Git e Github - III** - [Vídeo no YouTube]
17. **Controle de Versão, Git e Github - IV** - [Vídeo no YouTube]
18. **Controle de Versão, Git e Github - Prática I** - [Vídeo no YouTube]
19. **Controle de Versão, Git e Github - Prática II** - [Vídeo no YouTube]
20. **Controle de Versão, Git e Github - V** - [Vídeo no YouTube]
21. **Controle de Versão, Git e Github - VI** - [Vídeo no YouTube]
22. **Controle de Versão, Git e Github - VII** - [Vídeo no YouTube]
23. **Fast and flexible GitHub action to cherry-pick merged pull requests to selected branches. Secure drop-in replacement for korthout/backport-action.** - https://github.com/step-security/backport-action
24. **GITFLOW | TODO programador PRECISA saber o que é isso** - [Vídeo no YouTube]
25. **Git #1 - Conceitos e principais comandos de versionamento** - [Vídeo no YouTube]
26. **Git #2 - Trabalhando com Branch's e diferenciando Merge, Squash e Rebase** - [Vídeo no YouTube]
27. **Git #3: Stash - Escondendo arquivos para navegar entre branchs** - [Vídeo no YouTube]
28. **Git #4 - Repositórios remotos (push, pull x fetch, clone, reflog e cherry-pick)** - [Vídeo no YouTube]
29. **Git - Padronização de commits - gitmoji, commitlint e commitizen** - [Vídeo no YouTube]
30. **Git - Pull requests, Code review e contribuição em projetos públicos no github e gitlab** - [Vídeo no YouTube]
31. **Git - git flow na prática** - [Vídeo no YouTube]
32. **Git - git flow na prática** - [Vídeo no YouTube]
33. **Git Flow // Dicionário do Programador** - [Vídeo no YouTube]
34. **Git dicas - Profissionalize seus commits e entregas** - [Vídeo no YouTube]
35. **GitFlow: o que é, como funciona e quando realmente usar** - [Vídeo no YouTube]
36. **GitHub Docs** - https://docs.github.com
37. **Porque eu não gosto de Git Flow** - [Vídeo no YouTube]
38. **Strategies for Github Tagging and Release Management** - [Vídeo no YouTube]
39. **Trabalhando em equipe com Git Flow** - [Vídeo no YouTube]
40. **Tutorial: Controle de Versão de Software com Git** - [Vídeo no YouTube]
41. **release-please-action - GitHub Marketplace** - https://github.com/marketplace/actions/release-please-action

## 3. Engenharia de Prompts e Cicatrizes
### Tentativa 1
- Prompt:
Compare o Git Flow e o GitHub Flow em tabela (ideia, branches, release, complexidade)
- Resposta (resumo):
* **Git Flow**: Recomendado para aplicações distribuídas, sistemas legados ou produtos que exigem controle estrito e manutenção de múltiplas versões em paralelo.
* **GitHub Flow**: Ideal para aplicações web, SaaS e microsserviços onde o objetivo é realizar implantações frequentes e contínuas em produção.
- Referências usadas pela IA:
https://wingify.com/blog/git-branching-strategies/
https://dev.to/acestus/trunk-based-development-vs-git-flow-2kb5
- O que não funcionou:
Nada crítico nesta rodada. A resposta atendeu ao pedido: [citou fontes / veio no formato pedido / ficou utilizável no miniguia].
- Ajuste feito:
Nenhum ajuste necessário. Mantive o prompt como modelo reutilizável.

### Tentativa 2
- Prompt: Gerae um glossário de 8 termos do versionamento
- Resposta (resumo):
1. **Estrutura Básica**:
   * **Commit**: O registro fixo (*snapshot*) de um conjunto de alterações no histórico.
   * **Branch**: A ramificação para isolar o desenvolvimento de funcionalidades ou correções.

2. **Fluxo Colaborativo**:
   * **Pull Request (PR)**: O mecanismo do GitHub para propor, revisar e testar alterações antes da integração.
   * **Merge (e Squash & Merge)**: A união de ramificações, condensando múltiplos commits em um histórico limpo.

3. **Operações Avançadas**:
   * **Cherry-Pick**: A cópia seletiva de um commit específico para outra *branch* (essencial em *backports*).
   * **Git Stash**: O armazenamento temporário de alterações em rascunho para limpar a área de trabalho.

4. **Lançamento e Automação**:
   * **Tag e SemVer**: O direcionamento de marcadores fixos de versão baseados no padrão `MAJOR.MINOR.PATCH`.
   * **Conventional Commits**: A padronização das mensagens de commit que permite a automação de *releases* e *changelogs*.
- Referências usadas pela IA: Conteúdo alinhado às fontes principais (2.1); não detalhei cada citação do NotebookLM.
- O que não funcionou: Trouxe uma lista muito grante e completa
- Ajuste feito: Fiz uma solicitação para resumir

## 4. Miniguia de Estudo

### Resumos estruturados

#### Comparação estruturada entre o Git Flow e o GitHub Flow
| Critério de Análise | Git Flow | GitHub Flow |
| :--- | :--- | :--- |
| **Ideia Central** | Modelo rígido e altamente estruturado para gerenciar desenvolvimento paralelo e ciclos formais de lançamento por versões. | Modelo enxuto e ágil focado em integração e entrega contínuas (CI/CD). |
| **Branches** | **2 Permanentes**: `main` e `develop`.<br>**3 Temporárias**: `feature/*`, `release/*` e `hotfix/*`. | **1 Permanente**: `main` (sempre implantável).<br>**1 Temporária**: `feature/*` ou `bugfix/*` de curta duração. |
| **Release** | Promoção planejada via branch `release/*`, mesclada simultaneamente na `main` (com tag de versão) e na `develop`. | Implantação direta em produção a partir da `main` logo após a aprovação e mesclagem do Pull Request. |
| **Complexidade** | **Elevada**: Alto overhead de gestão de branches e risco frequente de conflitos complexos (*merge hell*) devido ao isolamento prolongado. | **Baixa**: Fluxo simples, pouca sobrecarga operacional e ciclos rápidos de feedback. |

#### Estratégias de Ramificação (Branching Strategies)

* **GitFlow**: Modelo estritamente estruturado composto por duas ramificações permanentes (`main` e `develop`) e três temporárias (`feature/*`, `release/*` e `hotfix/*`). Oferece alto isolamento para produtos com versões formais de lançamento, mas apresenta maior complexidade operacional e risco de conflitos de mesclagem (*merge hell*) em integrações prolongadas.
* **GitHub Flow**: Fluxo enxuto projetado para entrega contínua, onde apenas a branch `main` permanece em estado implantável. Novas funcionalidades ou correções são desenvolvidas em branches temporárias de curta duração e integradas diretamente à `main` por meio de **Pull Requests (PRs)**.
* **Trunk-Based Development (TBD)**: Prática ágil onde todos os desenvolvedores integram alterações na branch principal (`main` ou *trunk*) com frequência diária ou múltipla por dia. Depende do uso de **Feature Flags** (chaves de funcionalidade) para ocultar códigos incompletos em produção, reduzindo drasticamente conflitos e acelerando a esteira de CI/CD.

---

#### Comandos e Operações do Git

* **Gerenciamento de Estado (`git stash`)**: Permite salvar temporariamente modificações não concluídas no diretório de trabalho em uma pilha oculta, deixando a área de trabalho limpa para alternar de branch sem a necessidade de criar commits rascunhados.
* **Transporte Seletivo (`git cherry-pick`)**: Copia e reaplica um ou mais commits específicos de uma branch para outra sem importar todo o histórico adjacente.
* **Estratégias de Integração**:
  * **Merge**: Preserva o histórico completo de ramificação e intersecção de branches.
  * **Squash and Merge**: Consolida múltiplos commits intermediários de um PR em um único commit limpo na branch principal, mantendo o histórico linear e auditável.
  * **Rebase**: Move a base de uma branch para o topo da branch de destino, reescrevendo o histórico para criar uma linha do tempo estritamente linear.
* **Marcadores de Lançamento (Tags)**: Referências fixas vinculadas a um commit específico do histórico que sinalizam marcos ou versões oficiais de software.

#### Automação do Ciclo de Vida e Governança no GitHub

* **Versionamento Semântico (SemVer)**: Estrutura numéricas `MAJOR.MINOR.PATCH` onde o incremento do **Patch** sinaliza correções de falhas, o **Minor** adiciona funcionalidades retrocompatíveis e o **Major** introduz alterações incompatíveis.
* **Conventional Commits**: Convenção sintática para mensagens de commit (utilizando prefixos como `fix:`, `feat:`, `feat!:` / `BREAKING CHANGE:`) que torna o histórico interpretável por ferramentas automatizadas.
* **Automação de Lançamentos (Release Please)**: Ação automatizada do GitHub Actions que analisa o histórico de commits padronizados na `main`, atualiza o arquivo `CHANGELOG.md`, incrementa versões em arquivos de manifesto e cria/atualiza requisições de lançamento (*Release PRs*) de forma autônoma.
* **Governança e Branch Protection Rules**: Imposição de políticas no GitHub que bloqueiam commits diretos na branch principal, exigindo revisões obrigatórias por pares (*code review*) e aprovação prévia em verificações de CI/CD.
* **Backporting de Correções**: Processo automatizado que utiliza rótulos em PRs para propagar e aplicar correções de falhas da branch principal para branches de suporte dedicadas a versões legadas mantidas em produção.


### Glossário

#### 1. **Commit**
É o registro de um ponto na história do projeto (um *snapshot* ou instantâneo dos arquivos) que consolida as alterações realizadas na cópia de trabalho. Cada commit armazena um identificador único (*hash* SHA), o autor, a data e uma mensagem explicativa sobre as modificações feitas.

#### 2. **Branch (Ramificação)**
É um ponteiro móvel que aponta para um commit no histórico, permitindo isolar o desenvolvimento de uma funcionalidade ou correção em um ambiente separado sem afetar a linha principal do código. As ramificações garantem que modificações em andamento não desestabilizem a aplicação principal.

#### 3. **Pull Request (PR)**
É o mecanismo focal de colaboração em plataformas como o GitHub. Ele representa uma solicitação formal para mesclar o código de uma *branch* temporária na *branch* principal, servindo como ambiente para revisão de código por pares (*code review*), discussões técnicas e execução de testes automatizados via CI/CD.

#### 4. **Merge (e Squash & Merge)**
* **Merge**: Operação que une o histórico de alterações de uma *branch* em outra.
* **Squash and Merge**: Estratégia de mesclagem que junta múltiplos commits intermediários e de rascunho de um PR em um único commit limpo e padronizado na *branch* principal. Isso evita poluição no histórico e facilita o cálculo automatizado de versões.

#### 5. **Cherry-Pick**
É o comando que permite copiar e aplicar seletivamente um commit específico de uma *branch* para outra sem trazer todo o histórico adjacente. É fundamental em estratégias de *backporting* para aplicar correções de falhas de segurança (*hotfixes*) em versões legadas.

#### 6. **Git Stash**
É uma área de armazenamento temporário (uma pilha em rascunho) onde o desenvolvedor salva instantaneamente as alterações não concluídas do seu diretório de trabalho. Permite deixar a área de trabalho limpa para alternar de *branch* ou realizar tarefas urgentes sem a necessidade de criar um commit incompleto.

#### 7. **Tag e Versionamento Semântico (SemVer)**
* **Tag**: Um marcador fixo atribuído a um commit específico do histórico que não muda ao longo do tempo (diferente das *branches*), sendo usado geralmente para sinalizar o lançamento de uma versão oficial.
* **SemVer**: Padrão numérico `MAJOR.MINOR.PATCH` onde **Patch** indica correção de bugs, **Minor** novas funcionalidades retrocompatíveis e **Major** mudanças incompatíveis.

#### 8. **Conventional Commits**
Convenção e sintaxe padronizada para redação das mensagens de commit (utilizando prefixos como `feat:`, `fix:`, `feat!:`). Esse padrão torna o histórico inteligível para humanos e máquinas, permitindo que automações (como o *Release Please*) calculem o próximo número do SemVer e gerem o arquivo `CHANGELOG.md` automaticamente.


### Prompts reutilizáveis
1. Como usar o Backport Action?
2. Explique o Cherry-Pick na prática
3. O que é o Git Reflog?
4. Como automatizar o Release Please?
