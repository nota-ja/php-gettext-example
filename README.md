# PHP gettext example

## Prerequisites

* GNU gettext
  * `sudo apt-get install gettext` (Debian / Ubuntu)

## Deployment to Cloud Foundry

```
for d in locale/*/LC_MESSAGES/; do msgfmt $d/messages.po -o $d/messages.mo; done
cf push <APP-NAME>
```
