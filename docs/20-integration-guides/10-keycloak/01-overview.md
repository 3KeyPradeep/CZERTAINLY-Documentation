# Overview

This integration guide describes how to integrate platform with [Keycloak](https://www.keycloak.org/) as an authentication server.

CZERTAINLY access control decouples the identification, authentication, and authorization process. It provides flexible configuration of [Externalized Authentication](../../concept-design/architecture/access-control/externalized-authentication).

:::info Access Control
To get more information about the identification, authentication, and authorization process, refer to [Access Control](../../concept-design/architecture/access-control/overview).
:::

## Keycloak

Keycloak is an open source identity and access management solution. It provides a single place to manage all your users and applications. It can be used to secure applications and services with little to no code. It also support single sign-on and other advanced features like multi-factor authentication or risk-based authentication.

Enterprise grade authentication can be achieved by integrating Keycloak with CZERTAINLY.

:::caution Keycloak installation
This integration guide assumes that you have already installed and configured Keycloak. For more information, refer to [Keycloak documentation](https://www.keycloak.org/documentation.html).
:::

## Integration

The following steps should be done to integrate Keycloak with CZERTAINLY:

| #     | Reference                                                     | Short description                                                |
|-------|---------------------------------------------------------------|------------------------------------------------------------------|
| **1** | [Create Realm and Client](create-realm)                       | Create and configure new Keycloak Realm and Client               |
| **2** | [Configure OIDC](configure-oidc)                              | Configure OIDC client that can connect to Keycloak OIDC provider |
| **3** | [Create User and Login](create-user-login)                    | Create new Keycloak User for CZERTAINLY and login                |
| **3** | **(Optional)** [Add CZERTAINLY Theme](czertainly-theme) | Add CZERTAINLY custom theme to Keycloak and realm                |

## Identity providers

Keycloak supports multiple identity providers.
You can configure identity providers together with appropriate attribute mapping to allow users to login to CZERTAINLY with their existing accounts.

For more information, refer to [Identity Providers](https://www.keycloak.org/docs/latest/server_admin/#_identity_broker) in the Keycloak documentation.