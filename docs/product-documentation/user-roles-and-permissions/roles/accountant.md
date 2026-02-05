# Accountant

The accountant is responsible for financial integrity: posting transactions and producing financial reports for leadership and auditors.They escalate anomalies and higher order operations to [accountant](administrator.md)

---

- **Limit**
  - **Maximum accounts**: 1 primary account per instance. 1 optional deputy (this should be approved by admin first)

- **Purpose & Accountability**
  - Ensures accurate financial records and reporting. Accountable to the Admin and church governance.

- **Write permissions(Modules)**
  - Core Accounting
  - Contributions
  - Projects
  - Assets
  - Reporting

- **Responsibilities**
  - Post and categorize financial transactions
  - Allocate contributions to funds/projects. Handle adjustments based on approval rules
  - Produce financial statements, exports and ad-hoc reports for auditors and leadership.
  - Validate bulk financial imports and co-ordinate validation with admin before applying.

- **Acceptance Criteria**
  - Accountant can create, update and reconcile financial transactions.
  - Attempts to perform admin-only governance actions are blocked and logged.
  - Financial exports include audit metadata(requester, reason, timestamp) and are recorded.
