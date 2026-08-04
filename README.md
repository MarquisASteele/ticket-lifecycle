<p align="center">
    <img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Ticket Lifecycle Guide</h1>

This guide demonstrates the complete lifecycle of support tickets within osTicket by simulating real-world help desk scenarios. It covers ticket creation, prioritization, escalation, department routing, Service Level Agreements (SLAs), ticket ownership, and resolution from both the end-user and help desk perspectives.

<h2>Tools and Technologies Used</h2>

- **Microsoft Azure** (Virtual Machines/Compute)
- **Remote Desktop Connection**
- **osTicket**

<h2>Operating System Used</h2>

- **Windows 10 Pro** (21H2)

<h2>Objectives</h2>

- Create support tickets as an end user.
- Review ticket properties as a Help Desk Agent.
- Configure ticket priority, department, SLA, and ownership.
- Escalate tickets to the appropriate departments.
- Resolve tickets following a realistic help desk workflow.
- Observe how role-based permissions affect ticket visibility.
- Understand how ticket communication and documentation function in a production environment.

---

<h2>Lab Preparation</h2>

Before working through the ticket scenarios, prepare the environment by making the following changes.

- Change the **SysAdmins** department to a **Top-Level Department**.
- Delete the **Maintenance** department (do not archive it).

---

<h2>Ticket Scenario 1 – Online Banking System Outage</h2>

### End User

Create a ticket with the following issue:

> **Entire mobile/online banking system is down.**

<p>
<<img width="3024" height="1964" alt="image" src="https://github.com/user-attachments/assets/d668f39b-ac91-4f74-ac88-c6c01bf422c7" />
>
</p>

### Help Desk Agent (John)

Open the ticket and review the following properties:

- Priority
- Department
- SLA
- Assigned To

<p>
<!-- Insert Screenshot -->
</p>

Update the ticket with the following properties:

- **SLA:** SEV-A (1 Hour, 24/7)
- **Department:** Online Banking

<p>
<!-- Insert Screenshot -->
</p>

Attempt to access the ticket again as **John**.

Observe whether the ticket can still be viewed or modified after it has been escalated.

<p>
<!-- Insert Screenshot -->
</p>

### Help Desk Agent (Jane)

Log in as **Jane**, who belongs to the Online Banking department, and work the ticket through completion.

<p>
<!-- Insert Screenshot -->
</p>

---

<h2>Ticket Scenario 2 – Adobe Upgrade Request</h2>

### End User

Create a ticket with the following issue:

> **Accounting department needs Adobe upgrade, broken.**

<p>
<!-- Insert Screenshot -->
</p>

### Help Desk Agent (John)

Review the ticket properties.

- Priority
- Department
- SLA
- Assigned To

Assign the following properties:

- **SLA:** SEV-B (4 Hours, 24/7)
- **Department:** Support

<p>
<!-- Insert Screenshot -->
</p>

Work the ticket through completion as **John**.

<p>
<!-- Insert Screenshot -->
</p>

---

<h2>Ticket Scenario 3 – CFO Laptop Failure</h2>

### End User

Create a ticket with the following issue:

> **CFO's laptop will no longer turn on.**

<p>
<!-- Insert Screenshot -->
</p>

### Help Desk Agent (John)

Review the ticket properties.

- Priority
- Department
- SLA
- Assigned To

Assign the following properties:

- **SLA:** SEV-B (4 Hours, 24/7)
- **Department:** Support

<p>
<!-- Insert Screenshot -->
</p>

Resolve the ticket as **John**.

<p>
<!-- Insert Screenshot -->
</p>

---

<h2>Permission and Escalation Demonstration</h2>

Assign all tickets a **SEV-A** priority and move the **System Administrators** ticket last.

Observe that the escalated ticket is no longer accessible because of departmental permissions.

<p>
<!-- Insert Screenshot -->
</p>

Switch to the **Admin Panel** and grant your account **View Access** to the **System Administrators** department.

Return to the **Agent Panel** and reopen the ticket.

Notice that the ticket is now visible, but your permissions may still prevent you from modifying it.

<p>
<!-- Insert Screenshot -->
</p>

This demonstrates how role-based access control (RBAC) limits ticket visibility and editing privileges based on department membership and assigned permissions.

---

<h2>Email Notifications</h2>

Most enterprise ticketing systems include email integration.

Whenever a ticket is updated, assigned, or resolved, the requester typically receives an email notification containing the latest activity. Users can often reply directly to these emails, and their responses are automatically appended to the existing ticket, maintaining a complete communication history.

---

<h2>Ticket Intake in a Real Help Desk Environment</h2>

Support requests are received through many different channels, including:

- Phone calls
- Email
- Web portals
- Chat applications
- Walk-up requests
- Internal messaging platforms

Although technicians may occasionally resolve issues immediately, organizations generally require that every support request be documented with a ticket.

Creating tickets for all work performed provides:

- Accurate documentation
- Historical troubleshooting records
- SLA tracking
- Performance metrics
- Workload reporting
- Audit accountability

Proper documentation ensures issues can be tracked from creation through resolution while providing valuable operational metrics for the IT organization.

---

<h2>Skills Demonstrated</h2>

- Help Desk Ticket Management
- Ticket Lifecycle Management
- Incident Prioritization
- Service Level Agreement (SLA) Administration
- Department Routing
- Ticket Escalation
- Role-Based Access Control (RBAC)
- User and Agent Communication
- Incident Documentation
- IT Service Management (ITSM)
- Technical Documentation

---

<h2>Conclusion</h2>

This lab demonstrates the complete lifecycle of support tickets within osTicket, from initial ticket creation to final resolution. By working through multiple incident scenarios, configuring ticket properties, escalating requests between departments, and resolving issues based on priority and access permissions, this project provides practical experience with the workflows commonly used in enterprise IT service desks.

Repeating these exercises helps reinforce ticket management concepts, strengthens troubleshooting intuition, and builds the technical foundation required for entry-level Help Desk and IT Support roles.
