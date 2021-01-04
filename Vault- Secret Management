# Intdouctionn to Secret Management

As apps become more complex in the way they use microservices, managing API keys and other secrets becomes more challenging as well. Microservices running in containers need to transfer secrets to allow them to communicate with each other. Each of those transfers, and each of the secrets being exchanged, needs to be secured properly for the entire system to remain secure.

**Hard-coding API keys and other secrets is definitely NOT an option.**  
Despite the obvious nature of the previous statement, a lot of developers still expose the credentials of their microservices or apps on GitHub. Fortunately, there are tools designed to make managing secrets easier.

# Why Secret Management

Passwords and keys are some of the most broadly used and important tools your organization has for authenticating applications and users and providing them with access to sensitive systems, services, and information. Because secrets have to be transmitted securely, secrets management must account for and mitigate the risks to these secrets, both in transit and at rest.

### Secrets can include:

- User or auto-generated passwords

- API and other application keys/credentials (including within containers)

- SSH Keys

- Database and other system-to-system passwords.

- Private certificates for secure communication, transmitting and receiving of data (TLS, SSL etc.)

- Private encryption keys for systems like PGP

- RSA and other one-time password devices

The Other reason being the very nature of cloud infrastructure. Machine-to-machine and container-to-container communications are made more seamless with tokens, API keys, and other secrets transferred in a secure way.
Secrets management also enables better management of microservices-based architecture.
Other focus areas are

- Audit Logs: Who requested credentials for which system at what point of time
- High Automation for changing/revoking and rolling secrets
- High Entropy passwords
# Introduction to Vault

`Vault` provides a unified interface to secret while maintaining tight access control and logging a comprehensive audit log. It is a tool that secures user applications and base to limit the surface space and attack time in a breach. It gives an API that allows access to secrets based on policies. Any user of the API needs to verify and only see the secrets they are authorized to view.

# Why Vault

| Current problems                                   | Vault's Goals                                                         |
| -------------------------------------------------- | --------------------------------------------------------------------- | --- | --- | --- |
| Secrets are everywhere.                            | Vault is the single source of truth for all secrets.                  |
| They are generally unencrypted.                    | Vault manages encryption (during transit and at rest) out of the box. |
| It's difficult to dynamically generate them.       | Secrets can be dynamically generated.                                 |
| It's even more difficult to lease and revoke them. | Secrets can be leased and revoked.                                    |
| There's no audit trail.                            | There's an audit trail for generating and using secrets.              |

https://www.vaultproject.io/docs/what-is-vault

### Key Feature of Vault

- Secure Storage
- Encryption
- Access Control Policies
- Dynamic Secrets
- Auditing
- Multiple Authentication
- Revocation

**Secure Storage**
We can store data as a Key-Value pair. These values are stored in encrypted form in persistent storage. So, gaining access to raw storage isn't enough to access your secrets.

**Encryption**
Vault has the ability to encrypt and decrypt data. It provides facilities to encrypt and store the encrypted data in any location without having to design their own encryption methods.

**Access Control Policies**
We can manage the access for the secrets or any other features of the vault. This is the most crucial feature for any secret storage system.

**Dynamic Secrets**
Vault can generate secrets whenever we want for any systems. For example, when an application needs to access an S3 bucket, it asks Vault for credentials, and the Vault will generate an AWS keypair with valid permissions on demand.

**Auditing**
We can audit all the request to the vault and we can keep the redundant logs files. This includes any request to Vault: successes, failures, configuration, data access, etc. Audit logs can be sent to the syslog, files, and more.

**Multiple Authentication**
We can talk with the vault via multiple methods of authentication. e.g. Vault possesses the ability to support tokens, username/password, GitHub, certificates, and more.

**Revocation**
Vault can revoke all secrets read by a specific user or all secrets of a specific type. Revocation assists in key rolling as well as locking down systems in the case of an intrusion.

| Current problems                                   | Vault's Goals                                                         |
|----------------------------------------------------|-----------------------------------------------------------------------|---|---|---|
| Secrets are everywhere.                            | Vault is the single source of truth for all secrets.                  |
| They are generally unencrypted.                    | Vault manages encryption (during transit and at rest) out of the box. |
| It's difficult to dynamically generate them.       | Secrets can be dynamically generated.                                 |
| It's even more difficult to lease and revoke them. | Secrets can be leased and revoked.                                    |
| There's no audit trail.                            | There's an audit trail for generating and using secrets.              |

# Secret Management with Vault

https://www.vaultproject.io/guides/secret-mgmt


# Why We Need Dynamic Secrets
https://www.hashicorp.com/blog/why-we-need-dynamic-secrets

### Best Pratices

https://citihub.com/insights/our-blog/implementing-secrets-management-using-hashicorp-vault-enterprise/



# how to setup Vault
