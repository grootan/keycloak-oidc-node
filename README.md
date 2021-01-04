# Keycloak - Authorization Flow using Express

## About

This repository includes an express example app that displays the numerous Authorization Flows in OpenID Connect. This is a Node.js Express app that uses Keycloak to protect the /authorizedRoute route, Login and user setup are controlled by keycloak. The default route / is unprotected. The /logout route clears the keycloak session

## Instructions

1. Clone/Download the Repository.
2. Extract the zip or navigate to the home directory.
3. You can customize the details relevant to the OIDC in the ```./keycloak.json``` file
4. Make sure that you replace the keycloak-tenant-id with your TenantID and keycloak-client-id with your ClientID.
5. Modify {hostname} to align your keycloak domain.
6. RUN `npm install`
7. After installation of NPM packages, RUN `npm run start`
8. By default this node app will run in port `3000`
9. Finally, go to the browser and start `http://localhost:3000`

## Approach to work with the implicit flow

1. Click on "Login" button
2. You will be redirected to the user authentication screen of "Keycloak".
3. Complete all the authentication steps
4. Depending on the response type you configured, you will receive a token.

## What can I use these for

OpenID Connect is a perfect way to incorporate user authentication to your application, where you are relying on another party to handle user identity.

In this situation, Keycloak handles the identity of the users, allowing it faster to get up and running.

## Single Sign On (SSO)

By integrating OpenID Connect via Keycloak, you are building a session that can be used to single sign-on from your custom app to other applications that your users can access via the Keycloak portal.

If you have any queries / you notice any issues don't hesitate to raise issue.
