# Keycloak - Authorization Flow using Express

## About

This repo contains express example app that demonstrate the various OpenId Connect's Authorization flows. This is a Node.js Express app that uses Keycloak to protect the /authorizedRoute route, Login and user setup are controlled by keycloak. The default route / is unprotected. The /logout route clears the keycloak session.

## Instructions

1. Clone/Download the Repository.
2. Extract or GOTO home folder.
3. You can configure your OIDC related information in ```./keycloak.json``` file
4. Make sure you replace `keycloak-tenant-id` with your TenantID and `keycloak-client-id` with your ClientID.
5. Change `{hostname}` to match keycloak host.
6. RUN `npm install`
7. After installation of NPM packages, RUN `npm run start`
8. By default this node app will run port `3000`
9. Finally go to browser and launch `http://localhost:3000`

## Approach to work with the implicit flow

1. Click on "login" button
2. You will be redirected to "Keycloak" user authentication screen
3. Complete all authentication steps
4. You will receive Token based on the response type which you configured

## What can I use these for

OpenId Connect is a great way to add user authentication to your application where you are depending on another party to manage the user identities.

In this case Keycloak will manage the identity of your users making it faster to get up and running.

## Single Sign On (SSO)

By implementing OpenId Connect via Keycloak you are creating a session which can be used to single sign on from your custom app into other apps that your users may have access to via the Keycloak portal

If you have any queries / you notice any issues don't hesitate to raise issue.
