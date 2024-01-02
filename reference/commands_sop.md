### assign-sop

**Description**


Create a SOP and assign the SOP to one or multiple users.  _**Clinic Bees**_ will help to follow up
the execution of the SOP.

You could describe the SOP in message and the message will be kept as is and it becomes the "home"
of the SOP for reference.  Assignee will be kept reminded on compliance of the SOP in their daily
work.

You may add or remove assignees according to the instruction after you successfully executed this
command or close the SOP if it's no longer needed.

>[!NOTE] 
>This commend could be called in public channel only to make sure all assignees will be able to access
it.  And it could be called by Owner or Admin only.

**Syntax**
```text
assign-sop <SOP description>
```

**Example**
```text
assign-sop
NDIS Practice Standards
https://www.ndiscommission.gov.au/providers/registered-ndis-providers/provider-obligations-and-requirements/ndis-practice-standards
@Bella @Hedi
```

**Availability:** 
&nbsp;&nbsp;:far fa-check-square: Basic Plan
&nbsp;&nbsp;:far fa-check-square: Standard Plan
&nbsp;&nbsp;:far fa-check-square: Professional Plan  

**Roles Permission:**
&nbsp;&nbsp;:far fa-check-circle: Owner
&nbsp;&nbsp;:far fa-check-circle: Admin
&nbsp;&nbsp;:far fa-circle: User

**Call Place:**
&nbsp;&nbsp;:fas fa-circle: Direct Message (to _**bees**_)
&nbsp;&nbsp;:fas fa-check-circle: Public channels

**Cost of Credit Points:** &nbsp;&nbsp;Free

--------------------------------------------------------------------------------

### my-sop

**Description**

List all the open SOP assigned or created.

**Syntax**
```text
my-sop
```

**Availability:** 
&nbsp;&nbsp;:far fa-check-square: Basic Plan
&nbsp;&nbsp;:far fa-check-square: Standard Plan
&nbsp;&nbsp;:far fa-check-square: Professional Plan  

**Roles Permission:**
&nbsp;&nbsp;:far fa-check-circle: Owner
&nbsp;&nbsp;:far fa-check-circle: Admin
&nbsp;&nbsp;:far fa-check-circle: User

**Call Place:**
&nbsp;&nbsp;:fas fa-check-circle: Direct Message (to _**bees**_)
&nbsp;&nbsp;:fas fa-check-circle: Public channels

**Cost of Credit Points:** &nbsp;&nbsp;Free

--------------------------------------------------------------------------------

### cancel-sop

**Description**

Cancel a SOP with specific ref id.
It's typically to be used to handle some case that a SOP was not smoothly removed
when it's deleted but it's still assigned to some user.  For example, the user who
created the SOP is deleted from Slack.
This command could be called by Owner or Admin only.

**Syntax**
```text
cancel-sop <ref id>
```
**Example**
```text
cancel-sop 9
```

**Availability:** 
&nbsp;&nbsp;:far fa-check-square: Basic Plan
&nbsp;&nbsp;:far fa-check-square: Standard Plan
&nbsp;&nbsp;:far fa-check-square: Professional Plan  

**Roles Permission:**
&nbsp;&nbsp;:far fa-check-circle: Owner
&nbsp;&nbsp;:far fa-check-circle: Admin
&nbsp;&nbsp;:far fa-circle: User

**Call Place:**
&nbsp;&nbsp;:fas fa-check-circle: Direct Message (to _**bees**_)
&nbsp;&nbsp;:fas fa-check-circle: Public channels

**Cost of Credit Points:** &nbsp;&nbsp;Free
