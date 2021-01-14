# App Service Plan

- defines a set of compute resources for a web app to run
- One or more apps can be configured to run on the same computing resources (or in the same App Service plan)

Each App Service plan defines:

- Region (West US, East US, etc.)
- Number of VM instances
- Size of VM instances (Small, Medium, Large)
- [Pricing tier](#pricing-tier) (Free, Shared, Basic, Standard, Premium, PremiumV2, PremiumV3, Isolated)

  > App Service Free and Shared (preview) hosting plans are base tiers that run on the same Azure virtual machines as other App Service apps. Some apps might belong to other customers. These tiers are intended to be used only for development and testing purposes.

## Pricing tier

### Shared compute:

Free and Shared, the two base tiers, runs an app on the same Azure VM as other App Service apps, including apps of other customers. These tiers allocate CPU quotas to each app that runs on the shared resources, and **the resources cannot scale out**.

### Dedicated compute:

The Basic, Standard, Premium, PremiumV2, and PremiumV3 tiers run apps on dedicated Azure VMs. Only apps in the same App Service plan share the same compute resources. The higher the tier, the more VM instances are available to you for scale-out.

### Isolated:

This tier runs dedicated Azure VMs on dedicated Azure Virtual Networks. It provides network isolation on top of compute isolation to your apps. It provides the maximum scale-out capabilities.
