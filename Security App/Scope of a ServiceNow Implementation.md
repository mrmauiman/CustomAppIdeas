# Scope of a ServiceNow Implementaion
As seen on the [[Current  Workflows]] page, there is a lot of unecessary bulk to the workflows of hospital security.  This is a result of adopting new technologies overtime and not modernizing the entirety of the workflow.  However, not everything should be implemented as a standard feature in a hospital security app in ServiceNow because a lot of what was mentioned in [[Current  Workflows]] is hospital specific.  For example, Mary Washington Security is the only hospital security I know of that handles the morgue for the hospital.

## What should be implemented?
Below is a list of standard features I believe would fit into a general hospital security app:
- D.A.R.
- Opportunity patient tracker
- Bolo tracker
- C-Cure type application
	- Employee access manager
	- Alarm tracker
	- Remote control of hospital facilities (e.g. doors)
- Schedule
- Time off requests
- Daily briefing generater
- Lost and Found
- Tracker creator

## What groups should exist?
Assuming most hospital security teams are constructed similarly I believe the basic roles that should exist are:
- Chief
- Site Supervisor
- Shift Supervisor
- Security Officer

## Group permissions
### Chief
They should be able to access everything.  This is essentially the admin.

### Site Supervisor
They should be able to access everthing that has to do with their site.
- Promote/demote officers
- Set schedule for all shifts

### Shift Supervisor
They should be able to manage all officers on their shift.
- Set schedule for their shift.
- Access any supervisor specific tasks (MWHC example: morgue book)

### Security Officer
They should be able to access all applications except for the ones specified in the other groups.