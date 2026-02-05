# Permission Mapping

This sections shows a simple, non-tabular CRUD mapping that you can use to understand what each role is allowed to do in the system. It works alongside [summary.md](summary.md) and the role deep dives. For each module, you'll see which operations that are allowed for each role. If a permission has limits, a short note explains the scope of the restriction is added.

---

## Mapping

---

- **Membership Management**
  - **Write permissions**
    - Administrator
    - Clerk
  - **Read permissions**
    - All user roles

- **Core Accounting**
  - **Write permissions**
    - Administrator
    - Accountant
  - **Read permissions**
    - All user roles

- **Contributions**
  - **Write permissions**
    - Administrator
    - Accountant
    - Clerk: restriced to tagging only
  - **Read permissions**
    - All user roles

- **Projects**
  - **Write permissions**
    - Administrator
    - Accountant: restricted to finance-scope
    - Clerk: restricted to tagging contributions to projects
  - **Read permissions**
    - All user roles

- **Assets**
  - **Write permissions**
    - Administrator
    - Accountant
  - **Read permissions**
    - All user roles

- **Attendance**
  - **Write permissions**
    - Administrator
    - Clerk
  - **Read permissions**
    - All user roles

- **Reporting**
  - **Write permissions**
    - Administrator
    - Accountant
  - **Read Permissions**
    - All user roles
