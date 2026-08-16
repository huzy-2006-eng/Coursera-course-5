Access Controls -
Security controls that manage access,authorization and accountability of information.

AAA FRAMEWORK.
Authentication.
Authorization.
Accounting.

#### Factors of authentication -
1. Knowlegde: Something the user knows. Ex- Password
2. Ownership: Something the user posseses. Ex- OTP
3. Characteristic: Something the way is. Ex-Biometrics.

# Single sign-on(SSO):
A technology that combines several different logins into one.
1. SSO improves the user experience by eliminating the number of usernames and passwords people have to remember.
2. Companies can lower costs by streamlining how they manage connected services.
3. SSO improves overall security by reducing the number of access points attackers can target.
4. This technology became available in the mid-1990s as a way to combat password fatigue, which refers to people’s tendency to reuse passwords across services. 

## How SSO works:
1. SSO solutions use trusted third-parties to prove that a user is who they claim to be. This is done through the exchange of encrypted access tokens between the identity provider and the service provider.
2. These access tokens are exchanged using two authentication protocols:

LDAP(Lightweight Directory Access Protocol)- mostly used to transmit information on-premises.
SAML(Security Assertion Markup Language)- mostly used to transmit information off-premises, like in the cloud.

## Limitations of SSO:
Usernames and passwords alone are not always the most secure way of protecting sensitive information. SSO provides useful benefits, but there’s still the risk associated with using one form of authentication. 


#### Multi-factor authentication(MFA):
A security measure which requires a user to verify their identity in two or more ways to access a system or network.

#### Separation of duties -
The principle that users should not be given levels of authorization that would allow them to misuse a system.

#### Basic auth-
The technology used to establish a user's request to access a server.

#### OAuth-
An open-standard authorization protocol that shares designated access between applications.

#### API token -
A small block of encrypted code that contains information about a user.

OAuth sends and receives access requests using API tokens by passing them from a server to a user's device.

#### Accounting -
It is the process of monitoring the access logs of a system.

#### Session - 
A sequence of network HTTP basic auth requests and responses associated with the same user.

#### Session ID -
A unique token that identifies a user and their device while accessing the system.

#### Session cookie-
A token that websites use to validate a session and determine how long that session should last.

#### Session hijacking -
An event when attackers obtain a legitimate user's session ID.

# Identity and Access Management (IAM)-
1. As organizations become more reliant on technology, regulatory agencies have put more pressure on them to demonstrate that they’re doing everything they can to prevent threats. **Identity and access management (IAM) is a collection of processes and technologies that helps organizations manage digital identities in their environment**. Both AAA and IAM systems are designed to authenticate users, determine their access privileges, and track their activities within a system.

2. Either model used by your organization is more than a single, clearly defined system. They each consist of a collection of security controls that ensure the right user is granted access to the right resources at the right time and for the right reasons. Each of those four factors is determined by your organization's policies and processes.

# User Provisioning:
1. User Provisioning is the process of creating and maintaining a user's digital identity.
2. For example,a college might create a new user account when a new instructor is hired.
The new account will be configured to provide access to instructor-only resources while they are teaching.

# Granting authorization:
1. Mandatory Access Control(MAC)-
MAC is the strictest of the three frameworks. Authorization in this model is based on a strict need-to-know basis. Access to information must be granted manually by a central authority or system administrator. 

For example, MAC is commonly applied in law enforcement, military, and other government agencies where users must request access through a chain of command. MAC is also known as non-discretionary control because access isn’t given at the discretion of the data owner.

2. Discretionary Access Control(DAC)-
DAC is typically applied when a data owner decides appropriate levels of access. One example of DAC is when the owner of a Google Drive folder shares editor, viewer, or commentor access with someone else.

3. Role-based Access Control(RBAC)-
RBAC is used when authorization is determined by a user's role within an organization. For example, a user in the marketing department may have access to user analytics but not network administration.

