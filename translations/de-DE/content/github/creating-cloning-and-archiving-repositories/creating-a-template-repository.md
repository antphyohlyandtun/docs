---
title: Eine Repository-Vorlage erstellen
intro: 'Du kannst ein vorhandenes Repository zu einer Vorlage machen, sodass Du wie auch andere Personen neue Repositorys mit derselben Verzeichnisstruktur{% if currentVersion == "free-pro-team@latest" or currentVersion == "github-ae@latest" or currentVersion ver_gt "enterprise-server@2.20" %}, Branches{% endif %} und Dateien generieren können.'
permissions: Anyone with admin permissions to a repository can make the repository a template.
redirect_from:
  - /articles/creating-a-template-repository
versions:
  free-pro-team: '*'
  enterprise-server: '*'
  github-ae: '*'
topics:
  - Repositories
---

{% note %}

**Note**: Your template repository cannot include files stored using {% data variables.large_files.product_name_short %}.

{% endnote %}

Um eine Repository-Vorlage zu erstellen, musst Du ein Repository erstellen und es anschließend zu einer Vorlage machen. Weitere Informationen zum Erstellen eines Repositorys findest Du unter „[Ein neues Repository erstellen](/articles/creating-a-new-repository).“

After you make your repository a template, anyone with access to the repository can generate a new repository with the same directory structure and files as your default branch.{% if currentVersion == "free-pro-team@latest" or currentVersion == "github-ae@latest" or currentVersion ver_gt "enterprise-server@2.20" %} They can also choose to include all the other branches in your repository. Branches created from a template have unrelated histories, so you cannot create pull requests or merge between the branches.{% endif %} For more information, see "[Creating a repository from a template](/articles/creating-a-repository-from-a-template)."

{% data reusables.repositories.navigate-to-repo %}
{% data reusables.repositories.sidebar-settings %}
1. Wähle **Template repository** (Repository-Vorlage) aus. ![Kontrollkästchen zum Umwandeln eines Repositorys in eine Vorlage](/assets/images/help/repository/template-repository-checkbox.png)
