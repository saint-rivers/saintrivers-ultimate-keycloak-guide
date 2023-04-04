# Ultimate Keycloak Guide

## Building the custom keycloak theme

The Keycloakify starter project can be found here:

<https://github.com/keycloakify/keycloakify-starter>

Run the commands below to build the React App to Freemarker and a JAR file.

```bash
cd keycloakify-starter
npm run build-keycloak-theme
```

I think the new Quarkus version of Keycloak (17 or higher) allows building of Freemarker to jar files for theme customization in Keycloak UI.

Several helpful readme files can be found in `/opt/keycloak/**` with suggestions on what can be done.

The built jar files can be uploaded to the `/opt/keycloak/providers` and it will be built in the Keycloak Dockerfile.

## Updating the Keycloak Login UI

Using Keycloakify, the starting point of the configuration can be found in the file specified below.

`keycloakify-starter/src/keycloak-theme/login/KcApp.tsx`

The main styles will be stored in the `css` file in the same directory.

`keycloakify-starter/src/keycloak-theme/login/KcApp.css`
