# kevinatkins.dev
Personal website built on Hugo using the Congo theme

## Theme Customization
* Site uses the congo theme. Docs for configuration can be found here: https://jpanther.github.io/congo/docs/

## Prerequesites
* Download Hugo from https://gohugo.io/installation/
* Azure CLI for deployment https://learn.microsoft.com/en-us/cli/azure/

## Building
* `hugo` to build
* `hugo server` and site will be served at localhost:1313 

## Deployment
Currently hosted on Azure Static Web Apps. SWA CLI has been the easiest to get up and running for deployment. Config is saved at swa-cli.config.json. 

**Setup SWA CLI**
* Download swa-cli using `npm install -g @azure/static-web-apps-cli`
* `az login` if you haven't already authenticated with Azure CLI

**Deploy**
* `swa deploy --env production` for production build
* `swa deploy --env preview` for beta build. Preview site is found at https://thankful-ground-015359a10-preview.centralus.4.azurestaticapps.net