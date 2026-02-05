# Viewer

Viewers are read-only reviewers(auditors, trustees or members) who inspect and view records. They do not have permissions to modify data.

---

- **Limit**
  - **Maximum accounts**: unlimited accounts per instance

- **Purpose & Accountability**
  - No specific purpose

- **Write permissions**
  - No write permissions

- **Responsibilities**
  - Viewers do not have responsibilities

- **Acceptance Criteria**
  - Viewer can access permitted read views. Write attemps are blocked or ignored.
  - Exports succeed only with explicit export permission from admin or higher order role
  - Tests to confirm viewers cannot perform write operations.
