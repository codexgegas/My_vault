# Azure Active Directory 
Azure AD manages different types of identities: users, service principals, managed identities, and devices. In this unit, we consider each type of Azure AD identity.

## User 
- A user identity is a representation of something that's managed by Azure AD.
-  Employees and guests are represented as users in Azure AD.
-  If you have several users with the same access needs, you can create a group. You use groups to give access permissions to all members of the group, instead of having to assign access rights individually.
---
*There are two types of managed identities: system-assigned and user-assigned.*

**System-assigned**. Some Azure services allow you to enable a managed identity directly on a service instance. When you enable a system-assigned managed identity, an identity is created in Azure AD that's tied to the lifecycle of that service instance. When the resource is deleted, Azure automatically deletes the identity for you. By design, only that Azure resource can use this identity to request tokens from Azure AD.

**User-assigned**. You may also create a managed identity as a standalone Azure resource. A user-assigned managed identity is assigned to one or more instances of an Azure service. You can create a user-assigned managed identity and assign it to one or more instances of an Azure service. With user-assigned managed identities, the identity is managed separately from the resources that use it.

---
## Device
A device is a piece of hardware, such as mobile devices, laptops, servers, or printer. Device identities can be set up in different ways in Azure AD, to determine properties such as who owns the device. Managing devices in Azure AD allows an organization to protect its assets by using tools such as Microsoft Intune to ensure standards for security and compliance. Azure AD also enables single sign-on to devices, apps, and services from anywhere through these devices.

There are multiple options for getting devices into Azure AD:

-   **Azure AD registered devices** can be Windows 10, iOS, Android, or macOS devices. Devices that are Azure AD registered are typically owned personally, rather than by the organization. They're signed in with a personal Microsoft account or another local account.
-   **Azure AD joined** devices exist only in the cloud. Azure AD joined devices are owned by an organization and signed in with their account. Users sign in to their devices with their Azure AD or synced Active Directory work or school accounts. You can configure Azure AD joined devices for all Windows 10 devices (except Windows 10 Home).
-   **Hybrid Azure AD joined devices** can be Windows 7, 8.1, or 10, or Windows Server 2008, or newer. Devices that are hybrid Azure AD joined are owned by an organization and signed in with an Active Directory Domain Services account belonging to that organization. They exist in the cloud and on-premises.
---

# Types of external Identities

Azure AD External Identities is a set of capabilities that enable organizations to allow access to external users, such as customers or partners. Your customers, partners, and other guest users can "bring their own identities" to sign in.

There are two different Azure AD External Identities: B2B and B2C.

-   B2B collaboration allows you to share your apps and resources with external users.
-   B2C is an identity management solution for consumer and customer facing apps.