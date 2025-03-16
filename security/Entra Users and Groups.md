# Entra Users and Groups 

https://learn.microsoft.com/en-ca/training/modules/configure-user-group-accounts/1-introduction

> Access to [[Azure]] resources is controlled through user accounts and identities that are defined in [[Microsoft Entra ID]]. Microsoft Entra ID supports group accounts to help you organize user accounts for easier administration.

### Three types of accounts 

[[Microsoft Entra ID]] supports three types of user accounts. The types indicate where the user is defined (in the cloud or on-premises), and whether the user is internal or external to your Microsoft Entra organization

### Cloud identity	

A user account with a cloud identity is ==defined only in Microsoft Entra ID==. This type of user account includes administrator accounts and users who are managed as part of your organization. A cloud identity can be for user accounts defined in your Microsoft Entra organization, and also for user accounts defined in an external Microsoft Entra instance. When a cloud identity is removed from the primary directory, the user account is deleted.

- A new user account must have a display name and an associated user account name. An example display name is Aran Sawyer-Miller and the associated user account name could be asawmill@contoso.com.

- Information and settings that describe a user are stored in the user account profile.

- The profile can have other settings like a user's job title, and their contact email address.

- A user with Global administrator or User administrator privileges can preset profile data in user accounts, such as the main phone number for the company.

- Non-admin users can set some of their own profile data, but they can't change their display name or account name.

#### Things to consider when managing cloud identity accounts

Considerations when managing user accounts. 

- Consider ==user profile data==. Allow users to set their profile information for their accounts, as needed. User profile data, including the user's picture, job, and contact information is optional. 

- Consider ==restore options for deleted accounts==. Include restore scenarios in your account management plan. Restore operations for a deleted account are available up to 30 days after an account is removed. 

- Consider ==gathered account data==. Collect sign-in and audit log information for user accounts. 

### Directory-synchronized identity

User accounts that have a directory-synchronized identity are defined ==in an on-premises Active Directory==. A synchronization activity occurs via [[Microsoft Entra Connect]] to bring these user accounts in to Azure. The source for these accounts is [[Windows Server Active Directory]].

### Guest user	

Guest user accounts are ==defined outside Azure==. Examples include user accounts from other cloud providers, and Microsoft accounts like an Xbox LIVE account. The source for guest user accounts is Invited user. Guest user accounts are useful when external vendors or contractors need access to your Azure resources.