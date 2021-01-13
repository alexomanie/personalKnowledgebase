# App Service

## key features

- Multiple languages and frameworks _(ASP .NET, ASP .NET Core, Java, Ruby, Node.js, PHP, or Python)_
- Managed production environment
- Containerization and Docker
- Global scale with high availability
- Connections to SaaS platforms and on-premises data
- Security and compliance
- API and mobile features
- Serverless code

## Limitations

- App Service on Linux is not supported on Shared pricing tier.
- You can't mix Windows and Linux apps in the same App Service plan.
- Within the same resource group, you can't mix Windows and Linux apps in the same region.
- The Azure portal shows only features that currently work for Linux apps. As features are enabled, they're activated on the portal.
- When deployed to built-in images, your code and content are allocated a storage volume for web content, backed by Azure Storage. The disk latency of this volume is higher and more variable than the latency of the container filesystem. Apps that require heavy read-only access to content files may benefit from the custom container option, which places files in the container filesystem instead of on the content volume.
