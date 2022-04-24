# Guide sur le fonctionnement de cette communauté open source

Découvrez ci-dessous comment vous pouvez rejoindre un projet existant ou développer le vôtre.

## Une seule règle dans cette communauté

Nous ne sommes pas inquiets si vous cassez ce dépôt. C'est un terrain de jeu et nous vous encourageons à échouer souvent. Utilisez ce dépôt comme un terrain d'entraînement et prenez plaisir à contribuer aux projets que vous réalisez avec les autres étudiants. De nombreux étudiants ont acquis une expérience réelle du "travail en équipe" en travaillant sur ces projets.

## Un petit guide pour commencer

1. Consultez l'article [Qu'est-ce que Git & GitHub ?](Commandes_git.pdf).

2. Sur la [page GitHub de ce dépôt](https://github.com/digifab-dev/demarrer-avec-git), cliquez sur le bouton "Fork".

   ![Fork](https://help.github.com/assets/images/help/repository/fork_button.jpg)

3. Clonez _votre dépôt forké_ sur votre ordinateur :

   ![UI du code](https://docs.github.com/assets/images/help/repository/code-button.png)

    Par exemple, exécutez cette commande dans votre terminal :

    ```bash
    git clone https://github.com/<votre-pseudo-github>/demarrer-avec-git.git
    ```

    **Remplacez \<votre-pseudo-github\>**

    Pour en savoir plus sur le [forking](https://help.github.com/en/github/getting-started-with-github/fork-a-repo) et le [clonage d'un repo](https://docs.github.com/en/github/creating-cloning-and-archiving-repositories/cloning-a-repository).

4. Accédez au répertoire du projet :

    ```bash
    cd demarrer-avec-git
    ```

5. Avant d'apporter des modifications, [maintenez votre fork en phase](https://www.freecodecamp.org/news/how-to-sync-your-fork-with-the-original-git-repository/) pour éviter les conflits de fusion :

    ```bash
    git remote add upstream https://github.com/digifab-dev/demarrer-avec-git.git
    git pull upstream main
    ```

    Si vous rencontrez un **merge conflict**, vous devez résoudre le conflit. Il existe de nombreux guides en ligne, vous pouvez aussi essayer celui de [opensource.com](https://opensource.com/article/20/4/git-merge-conflict).

6. Après avoir ajouté le upstream et vérifié que tous les fichiers sont à jour, nous allons maintenant faire une nouvelle branche avant de modifier tout fichier. Il y a deux façons de faire :

    ```bash
    git checkout -b <nom-de-branche>
    ```

    ```bash
    git branch <nom-de-branche>
    git switch <nom-de-branche>
    ```

7. Sur votre ordinateur, ouvrez votre éditeur de texte, et ajoutez votre nom au fichier `CONTRIBUTORS.md`.

8. Ajoutez les changements avec `git add`, `git commit` ([écrire un bon message de commit](https://chris.beams.io/posts/git-commit/), si possible) :

    ```bash
    git add CONTRIBUTORS.md
    git commit -m "Ajout de <votre-pseudo-github>"
    ```

    **Remplacez \<votre-pseudo-github\>**

9. Poussez vos changements _vers votre dépôt_ :

    ```bash
    git push origin <nom-de-branche> 
    ```

10. Allez sur la page GitHub de _votre fork_, et faites une pull request :

    ![pull request](https://help.github.com/assets/images/help/pull_requests/choose-base-and-compare-branches.png)

    Pour en savoir plus sur les pull requests, consultez la [page d'aide de GitHub](https://help.github.com/en/github/collaborating-with-issues-and-pull-requests/creating-a-pull-request).

11. Attendez que l'un des mainteneurs fusionne votre demande de modification. S'il y a des conflits, vous recevrez une notification.

12. Rejoignez un projet et commencez à contribuer ou à former vos propres groupes d'applications. Soyez audacieux et prenez plaisir à développer des projets ensemble ! [Consultez ce guide](https://github.com/digifab-dev/demarrer-avec-git/blob/main/Pour_bien_démarrer.md) pour plus d'informations sur la sélection d'un projet.

13. Pour voir l'icône Digifab dans votre profil GitHub, [inscrivez-vous ici](https://digifab-github.herokuapp.com/) puis [suivez ces étapes](https://help.github.com/articles/publicizing-or-hiding-organization-membership/) (vous devez effectuer les étapes 1 et 2 pour que cela fonctionne).

## Anatomie d'un projet open source

Chaque communauté open source est différente.

Passer des années sur un projet open source signifie que vous avez appris à connaître _un_ projet open source. Passez à un autre projet et vous découvrirez que le vocabulaire, les normes et les styles de communication sont complètement différents.

Cela dit, de nombreux projets open source suivent une structure organisationnelle similaire. Comprendre les différents rôles de la communauté et le processus global vous aidera à vous orienter rapidement vers un nouveau projet.

Un projet open source typique comprend les types de personnes suivants :

**Author** : La personne ou l'organisation qui a conçu le projet.

**Owner** : La ou les personnes qui ont la propriété administrative de l'organisation ou du dépôt (ce n'est pas toujours la même chose que l'auteur original).

**Maintainers** : Les contributeurs qui sont responsables de la vision et de la gestion des aspects organisationnels du projet (peuvent également être les auteurs ou les propriétaires du projet).

**Contributors** : Toute personne qui a contribué au projet.

**Membres de la communauté** : Les personnes qui utilisent le projet. Ils peuvent être actifs dans les conversations ou exprimer leur opinion sur la direction du projet.

Les grands projets peuvent également avoir des sous-comités ou des groupes de travail axés sur différentes tâches, telles que l'outillage, le triage, la modération de la communauté et l'organisation d'événements. Pour trouver ces informations, consultez la page "équipe" du site Web d'un projet ou le dépôt de la documentation sur la gouvernance.

Un projet possède également une documentation. Ces fichiers sont généralement répertoriés à la racine du dépôt.

**LICENSE** : Par définition, chaque projet open source doit avoir une licence open source. Si le projet n'a pas de licence, il n'est pas open source.

**README** : Le README est le manuel d'instruction qui accueille les nouveaux membres de la communauté dans le projet. Il explique pourquoi le projet est utile et comment le démarrer.

**CONTRIBUTING** : Alors que les README aident les usagers à utiliser le projet, les docs de contribution aident les usagers à contribuer au projet. Elle explique quels types de contributions sont nécessaires et comment le processus fonctionne. Bien que tous les projets ne disposent pas d'un fichier CONTRIBUTING, sa présence indique qu'il s'agit d'un projet accueillant pour les contributions.

**CODE_OF_CONDUCT** : Le code de conduite fixe les règles de base du comportement des participants associés et contribue à faciliter un environnement convivial et accueillant. Bien que tous les projets ne disposent pas d'un fichier CODE_OF_CONDUCT, sa présence indique qu'il s'agit d'un projet accueillant auquel contribuer.

**Autre documentation** : Il peut y avoir une documentation supplémentaire, comme des tutoriels, des instructions ou des politiques de gouvernance, en particulier pour les projets plus importants.

Enfin, les projets open source utilisent les outils suivants pour organiser la discussion. La lecture des archives vous donnera une bonne idée de la façon dont la communauté pense et travaille.

**Issue tracker** : Où les participants discutent des problèmes liés au projet.

**Pull requests** : Où les participants discutent et examinent les changements en cours.

**Forums de discussion ou listes de diffusion** : Certains projets peuvent utiliser ces canaux pour des sujets de conversation (par exemple, "Comment puis-je..." ou "Que pensez-vous de..." au lieu de rapports de bogues ou de demandes de fonctionnalités). D'autres utilisent le gestionnaire des incidents pour toutes les conversations.

**Canal de discussion synchrone** : Certains projets utilisent des canaux de discussion (tels que Discord ou IRC) pour les conversations informelles, la collaboration et les échanges rapides.
