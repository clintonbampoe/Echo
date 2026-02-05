# Guidelines

This file offers a simple template and set of practical rules that help contributors define roles in a consistent way. The goal is to make role definitions easy to understand, straightforward to implement in code, and ready to connect with permission checks or UI controls later on.

---

## Core Rules

- **Least Privilege**: Give only the minimum permissions needed for the role to do its job.
- **Keep it small**: Prefer a minimal set of roles and simple responsibilities.
- **Be explicit**: State limits and restricitions clearly so devs can implement them without guessing.
- **Log everything**: All write actions must be auditable (actor, role, timestamp, entity, reason)
- **Make it extensible**: Design roles so adding a narrowly scoped role later is straightforward.

---

## Role Definition Template

For each role in the `roles` directory, include only the sections below. Keep each section concise, clear and straightforward.

- **Header**
  - Role name
- **Limit**
  - Maximum number of accounts allowed for this role per church instance.
- **Write Permissions**
  - List modules where the role has write access (exact module names). If permission is restricted, include the restriction inline. Keep each entry to one line.
- **Responsibilities**
  - List concise bullet points describing the day-to-day tasks(action-oriented, e.g, "Record contributions and tag to projects")
- **Acceptance Criteria**
  - Include concrete checks that show that the role is working as intended. Example: "Clerk can create contributions but cannot mark deposits cleared; attempts are blocked and logged"

---

## Permission Mapping Guidelines

To map permissions to a role, devs must follow this guideline...

- Navigate to the [permission-mapping.md](permission-mapping.md) file
- Find the permission you want to add to the role under the **Mapping** section.
- Under **Write permissions**, add the role that you want to have this permission.
- If there are restrictions to said permission, please describe the restriction inline (in full detail) next to the role.
- All roles by defualt have **Read permissions**--confirm before rollout.
- Refer to [permission-mapping.md](permission-mapping.md) for examples on how to implement this.
