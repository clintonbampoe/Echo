# Clerk

Clerk handle routine operational data entry: recording contributions, attendance and basic membership administration operations. They escalate anomalies and higher order operations to [accountant](accountant.md)

---

- **Limit**
  - **Maximum accounts**: 3 accounts per instance(default). Admin may configure

- **Purpose & Accountability**
  - Performs day-to-day operational data entry and basic member administration. accountable to Accontant and church governance.

- **Write permissions(Modules)**
  - Membership management
  - Contributions
  - Projects
  - Attendance

- **Responsibilities**
  - Record contributions and tag gifts to members, funds or projects
  - Record attendance for services and events and maintain basic attendance summaries
  - Update member data and group membership
  - Flag anomalies (mismatched deposits, duplicate records) and escalate to accountant or admin, if permission is denied

- **Acceptance Criteria**
  - Clerk can create and tag contributions.
  - UI hides or disables deposit finalization, reconciliation and other operations that require accountant permissions.
  - Clerk entries are recorded in audit logs with author, timestamp, entity and metadata (subject to change)
