# qadevsys-swiss-champ
Deploys al scrum team tools in a single instance.

The team need this essential tools:
* git
* chat
* automatization
* quality
* artifact repository
* project management

All those tools must have a Open Source license.

## Git
There are some valid alternatives but the better IMHO are Gitea/Gogs and Gitlab.

### Gitea
Gitea fits all requirements and does not have big hardware requirements so it could be a good choice when there is not enough RAM to run gitlab.

### Gitlab
Gitlab is a full stack software that includes mattermost (slack replacement), docker registry, continuos integration (in some use cases could be a good Jenkins replacement) and more.

But it needs more hardware, starting with 4GB RAM.

## Chat
Chat is included with gitlab as a slack replacement with mattermost.

## Jenkins
Is an automatization tool that will help you to do CI, CD, QA tasks, ...

## Sonar
Will measure the code quality.

## Nexus
It is an artifact repository.

## Taiga
It is a scrum tool that integrates with Gitea and Github (https://tree.taiga.io/support/integrations/webhooks/).

# Used resources
jmferrerm@serenity:~$ free
              total        used        free      shared  buff/cache   available
Memoria:    16317664    12681772      374456      691960     3261436     2402988
Swap:             0           0           0
jmferrerm@serenity:~$ docker stop gitlab
free -m
^C
jmferrerm@serenity:~$ free -m
              total        used        free      shared  buff/cache   available
Memoria:       15935        6813        5863         701        3258        7893
Swap:             0           0           0
jmferrerm@serenity:~$ docker stop nexus
^C
jmferrerm@serenity:~$ free -m
              total        used        free      shared  buff/cache   available
Memoria:       15935        6275        6394         701        3264        8431
Swap:             0           0           0
jmferrerm@serenity:~$ docker stop jenkins
^C
jmferrerm@serenity:~$ free -m
              total        used        free      shared  buff/cache   available
Memoria:       15935        4767        7897         700        3269        9940
Swap:             0           0           0
jmferrerm@serenity:~$ docker stop sonarqube
^C
jmferrerm@serenity:~$ free -m
              total        used        free      shared  buff/cache   available
Memoria:       15935        2872        9793         700        3269       11837
Swap:             0           0           0
jmferrerm@serenity:~$ docker stop postgresql
^C
jmferrerm@serenity:~$ free -m
              total        used        free      shared  buff/cache   available
Memoria:       15935        2868        9809         687        3256       11854
Swap:             0           0           0
jmferrerm@serenity:~$ docker stop nginx
^C
jmferrerm@serenity:~$ free -m
              total        used        free      shared  buff/cache   available
Memoria:       15935        2852        9821         687        3261       11870
Swap:             0           0           0
jmferrerm@serenity:~$
