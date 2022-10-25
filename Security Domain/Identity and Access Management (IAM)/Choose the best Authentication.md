Authentication (sometimes abbreviated AuthN) is the process of verifying who you are and making sure you are who you say you are. When logging on to a PC with a user name and password authentication happens. Below contain some of the industries commonly used authentication protocols.

- OpenID Connect (OIDC) is a simple identity layer on top of the OAuth 2.0 protocol, which allows computing clients to verify the identity of an end-user based on the authentication performed by an authorization server, as well as to obtain basic profile information about the end-user in an interoperable and REST-like manner. In technical terms, OpenID Connect specifies a RESTful HTTP API, using JSON as a data format. OpenID Connect allows a range of kinds of clients, including Web-based, mobile, and JavaScript clients, to request and receive information about authenticated sessions and end-users. The specification suite is extensible, supporting optional features such as encryption of identity data, discovery of OpenID Providers, and session management.
- SAML is an XML based framework used by business entities or partners to share the authentication, attribute, and entitlement information about an entity. SAML can be used in the following three scenarios:
- Single Sign On(SSO): SAML is specially used to solve the multidomain problem. For example, a user has an account with example1.com and example2.com, where these two are business partners. With a single sign on facility, the user has to login just once on the Web site and he will be able to access resources from both the Web sites. Sharing authentication information is fairly simple as SAML provides independent grammar and protocol to share information from one server domain to the other domain.
- Federated Identity: As maintaining identity information for each of the services that a user is subscribed to is a tedious process, SAML solves this problem by providing grammar to establish a identity known as federated identity. This is a shared name identifier used to refer to an end user or an entity who is using the services offered by various partners.
- Web Service Security: SAML also provides a facility to secure the Web services. This is done by using SAML assertion in the soap header to transmit the information which is not possible using other security formats.
- Web Services Federation (WS-Federation or WS-Fed) is part of the larger WS-Security framework and an extension to the functionality of WS-Trust. The features of WS-Federation can be used directly by SOAP applications and web services. WS-Fed is a protocol that can be used to negotiate the issuance of a token. You can use this protocol for your applications (such as a Windows Identity Foundation-based app) and for identity providers (such as Active Directory Federation Services).

### Enable Single Sign-On

In a mobile-first, cloud-first world, you want to enable single sign-on (SSO) to devices, apps, and services from anywhere so your users can be productive wherever and whenever. When you have multiple identity solutions to manage, this becomes an administrative problem not only for IT but also for users who have to remember multiple passwords. By using the same identity solution for all your apps and resources, you can achieve SSO. And your users can use the same set of credentials to sign in and access the resources that they need, whether the resources are located on-premises or in the cloud.

**Best Practices**

- Allow users to log in with a single ID to several related, but independent software systems.
- Leverage existing solutions for creating/managing user identities.
- Enforce session timeouts.
- Enable authentication request signing to make sure that all SAML responses, for example AQR, assertions, and logout responses, are signed.
- Make sure that none of your certificates are expired or revoked.
- Set excluded users to ensure that accounts and users are unable to log in or remain logged in.
- Always do exact matching of redirect URIs.
- Callback pages should not contain third party resources.

### Enforce Multi-Factor Authentication for Users

Multi-Factor Authentication is a method of authentication that requires the use of more than one verification method and adds a critical second layer of security to user sign-ins and transactions. Multi-Factor Authentication helps safeguard access to data and applications while meeting user demand for a simple sign-in process. It delivers strong authentication via a range of verification options: phone calls, text messages, or mobile app notifications or verification codes and third-party OAuth tokens.

Methods for authenticating people differ significantly from those for authenticating machines and programs, and this is because of the major differences in the capabilities of people versus computers. Computers are great at doing large calculations quickly and correctly, and they have large memories into which they can store and later retrieve Gigabytes of information. Humans do not. So we need to use different methods to authenticate people. In particular, the cryptographic protocols we have already discussed are not well suited if the principal being authenticated is a person (with all the associated limitations).

**Best Practices**

- Require multi factor authentication for all of your users.
- Microsoft recommends not using SMS as a second factor of authentication.
- Use MFA for Global Admins and other accounts with administrative privileges, even if you are not using it for the standard users.
- Use Microsoft Authenticator app on your smartphone for Global Admin accounts, because it is more secure than other verification options.