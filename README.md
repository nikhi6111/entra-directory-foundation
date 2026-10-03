# VDR Directory Foundation

## Project Overview

This lab documents a practice Microsoft Entra ID directory for the fictional company VDR.

## Audit Evidence

### User changes

![VDR user audit log showing successful creation and earlier failed imports](screenshots/audit-users.png)

The log records the activity, timestamp, target account, status, and initiating administrator. Earlier bulk creation attempts failed because the initial passwords contained usernames. After correcting the passwords, the user creation events succeeded.

### Group changes

![VDR group audit log showing group creation, owner assignment, and membership changes](screenshots/audit-groups.png)

Successful Core Directory events include Add group, Add owner to group, and Add member to group. The screenshot also contains an earlier owner-assignment failure and a group deletion event, preserving the visible audit history.

## New-Hire Exercise

I created Avery Thompson as an IT Analyst reporting to
Jordan Lee, then added Avery to SEC-Dept-IT.

VDR now has 16 company users plus my administrator account.
SEC-Dept-IT has 11 members.

## Hypothetical Access Comparison

Suppose IT employees need four applications: a ticketing
system, asset inventory, monitoring dashboard, and internal
knowledge base.

With group-based assignments, those applications could each
be assigned once to SEC-Dept-IT: four application assignments.
A new hire would need an account and one group membership.

With individual assignments, each of the 11 IT employees
would need four grants: 44 application assignments.
A new hire would need an account and four separate grants.

This is a design comparison. I have not assigned application
access to these groups in this lab.
