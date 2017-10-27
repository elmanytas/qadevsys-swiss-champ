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

