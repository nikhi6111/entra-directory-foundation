# VDR Directory Foundation

## Project Overview

This lab documents a practice Microsoft Entra ID directory for the fictional company VDR.

## Audit Evidence

### User changes

![VDR user audit log showing successful creation and earlier failed imports](screenshots/audit-users.png)

The log records the activity, timestamp, target account, status, and initiating administrator. Earlier bulk creation attempts failed because the initial passwords contained usernames. After correcting the passwords, the user creation events succeeded.
