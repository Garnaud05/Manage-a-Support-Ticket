# Help Desk Lab: Ticket Escalation & New User PC Setup (osTicket)

## Scenario
On my first day as an IT Support Technician, my manager assigned two practice tickets in the company help desk system (osTicket). The mission: learn the company's support procedures and clear the day's unresolved tickets.

## Tools Used
- **osTicket**: ticketing system (tickets, tasks, knowledge base)
- **Windows 10**: domain-joined PC (Active Directory)
- **Mozilla Firefox**, **LibreOffice**, **Mozilla Thunderbird**

## Skills Demonstrated
Ticket ownership and assignment, task creation, knowledge base research, ticket escalation, professional ticket communication, user account verification, software validation, email client configuration.

---

## Part 1: Ticket #721285 (Helpdesk escalation procedures)

**Request:** Take ownership of the ticket, create a task to review the FAQs, then escalate the ticket to the Level 2 team. Leave the task open for review.

### Step 1: Log in and review the queue
I signed in to the osTicket agent portal and opened the Tickets queue, which held three unassigned high-priority tickets.

![Windows login screen](images/Screenshot__1441_.png)
![osTicket agent login](images/Screenshot__1443_.png)
![Open ticket queue showing 3 high-priority tickets](images/Screenshot__1444_.png)

### Step 2: Take ownership and create a task
I claimed ticket #721285 and created a task to identify FAQ categories and topics, assigned to myself under the Support department.

![Ticket #721285 assigned to me](images/Screenshot__1448_.png)
![Creating the task](images/Screenshot__1449_.png)

### Step 3: Review the knowledge base
In the Knowledge Base, I read the **Ticket escalation** FAQ. Key takeaways:
- Escalate by assigning the ticket to the **Level 2 Support** team.
- Tickets that should normally be escalated:
  - Incidents where personal or company confidential data could have been breached
  - Suspected malware that can't be identified or removed with Windows Defender
  - Requests that require Domain Administrator privileges
  - Requests for new software or hardware

![Ticket escalation FAQ](images/Screenshot__1451_.png)

### Step 4: Update the task
I posted an update summarizing what I learned about escalation routes and scope, and left the task open as instructed.

![Task update posted](images/Screenshot__1453_.png)

### Step 5: Escalate to Level 2 Support
I confirmed the ticket was assigned to me (My Tickets > Assigned to Me), then reassigned it to the **Level 2 Support** team.

![My Tickets queue](images/Screenshot__1454_.png)
![Reassigning the ticket to Level 2 Support](images/Screenshot__1456_.png)

### Step 6: Reply to the requester
I replied on the ticket so the requester knew the outcome: *"I've reviewed the FAQs and escalated it to the level 2 support team for completion."*

![Ticket reply](images/Screenshot__1457_.png)

---

## Part 2: Ticket #211913 (Set up PC for Kei)

**Request:** Verify the PC is configured correctly for Kei's account. Log on as Kei, launch LibreOffice and Firefox, confirm the account can browse www.515support.com, then add Kei's email account (kei@structureality.com) in Thunderbird.

### Step 1: Claim the ticket
I read the requirements and used **Claim** to assign the ticket to myself.

![Ticket #211913 details](images/Screenshot__1460_.png)
![Claiming the ticket](images/Screenshot__1461_.png)

### Step 2: Log in as Kei
On the PC, I signed in with Kei's domain account (ad.structureality.com).

![Domain login as Kei](images/Screenshot__1462_.png)

### Step 3: Verify applications
- **LibreOffice** launched successfully.
- **Firefox** and **Thunderbird** shortcuts were on Kei's desktop.
- **Firefox** loaded **www.515support.com**, confirming Kei's account has web access.

![LibreOffice start center](images/Screenshot__1465_.png)
![Kei's desktop with Firefox, LibreOffice, Thunderbird](images/Screenshot__1468_.png)
![515support.com loading in Firefox](images/Screenshot__1475_.png)

### Step 4: Set up email in Thunderbird
I launched Thunderbird and entered Kei's name, email address, and password in Account Setup. Thunderbird detected the server settings automatically (IMAP incoming, SMTP outgoing, mail.structureality.com). The ticket noted that the mail protocols aren't secured yet, so I clicked through the "no encryption" warning as expected.

![Thunderbird account setup (blank)](images/Screenshot__1469_.png)
![Name and email entered](images/Screenshot__1470_.png)
![Password entered](images/Screenshot__1471_.png)
![Configuration found automatically](images/Screenshot__1472_.png)
![Account successfully created](images/Screenshot__1474_.png)

### Step 5: Document the work on the ticket
Back in osTicket, I replied with a summary: Kei's sign-in works, LibreOffice and Firefox launch, 515support.com is reachable, and the Thunderbird account is configured.

![Reply summarizing the work](images/Screenshot__1476_.png)

### Step 6: Close the ticket
With everything verified and documented, I set the ticket status to **Closed**.

![Closing ticket #211913](images/Screenshot__1477_.png)

---

## Results
- Researched and correctly **escalated** a ticket following documented procedure
- Created and updated a **task** and left it open as instructed
- Verified a user's domain login, application launches, and web access
- Configured a **company email account** in Thunderbird
- Documented findings on the ticket and **closed** it once everything was verified

## What I Learned
- Follow documented procedures; the knowledge base is the first stop before escalating.
- Escalation criteria (data breach, unresolved malware, admin-level access, new hardware or software) determine when a ticket leaves Level 1.
- Clear ticket updates keep requesters and teammates informed and leave a record of the work.
- Logging in as the user catches setup problems before they turn into support calls.
