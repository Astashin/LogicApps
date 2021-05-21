
#### Set of Logic Apps working together to automate user sync between Azure AD tenants.
- B2B Invitation worker – reads user information from source and invites to destination tenant. Saves data for attribute syncing
- Attribute sync worker – performs synchronization of user object attributes from source to destination tenant
- Main workflow – triggered by scheduler and starts two sync workers above. Writes logging information to storage table

Full description is in this blog articles:
1. [Overview](https://blog.astashin.com/blog/Bring-em-all-in-p5/)
2. [Low-level design](https://blog.astashin.com/blog/Bring-em-all-in-p6/)
