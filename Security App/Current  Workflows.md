# Current Workflows
**[[Scope of a ServiceNow Implementation | Scope of Security App]]**
## D.A.R.
This is an application for the dispatcher to log information about what all officers are doing.  Examples of uses:
- Log when officers do patrols
- Log when officers took breaks
- Log what occured during a call
- Log if a system was reported as malfunctioning

## EPIC
This is an application to keep track of what patients are currently admitted.  For security use, it informs officers which rooms have custodials and which rooms are private.

It is unlikely you could integrate this into ServiceNow since this is a hospital wide program and officers use it for such a small usecase.  There is also no way to integrate EPIC with an external service.

However, we could integrate the custodial tracking into it's own custom tracker since every custodial must be escorted in by a security officer, so we could setup an automation to add a custodial to a custodials tracker when ever there is a custodial escort in the D.A.R. implementation

>**Note:** After some googling I found an API called QIE.  However, It's not something you can just implement due to the nature of the data it gives access to.

## C-CURE
This is an application that tracks all hospital personnel.  It tracks what doors employees access and any alarms that are triggered in the hospital.  Examples of uses:
- Disable/enable employee badges
- Open any door in the hospital remotely
- Alert the dispatcher of any alarms (fire, tamper, hugs, etc.)

## Excel Spreadsheets
Most information security needs to keep track of is kept in Excel Spreadsheets and could be implemented into databases and forms on ServiceNow.  Examples of things kept in Excel:
- Lost and Found
- Daily Briefing
- Bolos
- Officer on call list
- Schedule
- etc.

## Various Physical Forms
Many things are still tracked with physical records that could be easily integrated into digital forms.  Examples of physical records:
- Morgue book
- Item lones (keys, pagers, temperary badges)
- Time off requests
- etc.