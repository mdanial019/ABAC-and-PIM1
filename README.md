# ABAC-and-PIM1
Hands-on lab implementing least-privilege, scope-aware access control in Microsoft Entra ID — moving from permanent, tenant-wide role assignments to custom roles, Administrative Unit-bound delegation, and time-boxed PIM activation, with every change traced through the audit log.
What this lab covers
🧩 Built a least-privilege custom role from scratch, scoped to a single explicit permission (microsoft.directory/agentIdentities/appRoleAssignedTo/update) instead of reusing an over-privileged built-in role.
🏢 Created an Administrative Unit and delegated a built-in role (Groups Administrator) scoped only to that unit — restricting a user's admin rights to a defined object boundary rather than the entire directory.
⏱️ Converted a permanent PIM assignment into a time-bound, justification-required active assignment, replacing standing privileged access with just-in-time, business-justified activation.
⚖️ Directly contrasted two delegation models for the same privilege — a permanent, tenant-wide role grant vs. an Administrative Unit-scoped grant — to illustrate blast-radius reduction in practice.
🔍 Verified every change end-to-end via Entra ID audit logs, tracing custom role creation, scoped role assignment, and PIM add/remove/process events with full timestamps.
📝 Noted where Entra ID directory roles differ from true Azure-style ABAC — custom roles and Administrative Units are the native equivalents for permission- and object-scope restriction, since Entra ID directory roles don't support Azure resource RBAC's attribute-based conditions.
Why it matters

Standing, tenant-wide privileged access is one of the most common findings in real-world identity security reviews. This lab demonstrates the practical alternative: scoping what a role can do (custom roles), scoping where it applies (Administrative Units), and scoping when it's active (PIM) — the core toolkit for privileged access management (PAM) in an enterprise Entra ID tenant.

Skills demonstrated

Microsoft Entra ID · Custom RBAC Roles · Administrative Units · Privileged Identity Management (PIM) · Least-Privilege Design · Just-in-Time Access · Audit Log Analysis · Privileged Access Governance
