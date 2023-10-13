### TEMPLATE

**Description**

**Syntax**
```text
```

**Example**
```text
```

**Availability:** 
&nbsp;&nbsp;:fas fa-check-square: Basic Plan
&nbsp;&nbsp;:fas fa-check-square: Standard Plan
&nbsp;&nbsp;:fas fa-check-square: Professional Plan  

**Roles Permission:**
&nbsp;&nbsp;:fas fa-check-circle: Owner
&nbsp;&nbsp;:fas fa-circle: Admin
&nbsp;&nbsp;:fas fa-circle: User

**Cost of Credit Points:** &nbsp;&nbsp;Free

--------------------------------------------------------------------------------

### list-practitioners

**Description**

List practitioners from the linked Cliniko account and the mapping status with the Slack users.

**Syntax**
```text
list-practitioners
```

**Example**
```text
# List active practitioners only.
list-practitioners

# List all practitioners including inactive ones.
list-practitioners all
```

**Availability:** 
&nbsp;&nbsp;:fas fa-check-square: Basic Plan
&nbsp;&nbsp;:fas fa-check-square: Standard Plan
&nbsp;&nbsp;:fas fa-check-square: Professional Plan  

**Roles Permission:**
&nbsp;&nbsp;:fas fa-check-circle: Owner
&nbsp;&nbsp;:fas fa-check-circle: Admin
&nbsp;&nbsp;:fas fa-check-circle: User

**Cost of Credit Points:** &nbsp;&nbsp;Free

--------------------------------------------------------------------------------

### map-practitioner

**Description**

Map practitioner with specific Slack user, or clear the mapping.

This is typically an one-time setup for a practitioner.  Once it's mapped, the connection
will be unchanged even practitioner name is changed or Slack name is changed.
You may run `list-practitioners` first to get the full list of practitioners and then
map those not yet mapped.


>[!TIP]
>It's strongly suggested to have Owner/Admin to execute this command in a public channel (eg. #general)
so that the mapping is transparent to the practitioner and acknowledge the mapping completion.

**Syntax**
```text
map-practitioner auto

map-practitioner <practitioner name>=<Slack user>

map-practitioner <practitioner name>=
```

**Example**
```text
# Auto map the practitioners who had not yet been mapped.
map-practitioner auto

# Map practitioner Izabella Solomon and Jackie Newman (names on Cliniko) to their Slack names.
map-practitioner Izabella Solomon = @Bella, Jackie Newman = @Jackie 

# You may also send the command in a multi-line message to make it clearer.
map-practitioner
Izabella Solomon = @Bella, 
Jackie Newman = @Jackie 

# Clear mapping of practitioner Jackie Newman.
map-practitioner Jackie Newman=
```

**Availability:** 
&nbsp;&nbsp;:fas fa-check-square: Basic Plan
&nbsp;&nbsp;:fas fa-check-square: Standard Plan
&nbsp;&nbsp;:fas fa-check-square: Professional Plan  

**Roles Permission:**
&nbsp;&nbsp;:fas fa-check-circle: Owner
&nbsp;&nbsp;:fas fa-check-circle: Admin
&nbsp;&nbsp;:fas fa-circle: User

**Cost of Credit Points:** &nbsp;&nbsp;Free

--------------------------------------------------------------------------------

### show-focus

**Description**

Display the focused practitioners and metrics of the current channel.

_**Clinic Bees**_ is using Slack channel to manage performance of specific practitioners and key metrics,
so that the management and actions are focused.

This command could be called in a channel only.

**Syntax**
```text
show-focus
```

**Availability:** 
&nbsp;&nbsp;:fas fa-check-square: Basic Plan
&nbsp;&nbsp;:fas fa-check-square: Standard Plan
&nbsp;&nbsp;:fas fa-check-square: Professional Plan  

**Roles Permission:**
&nbsp;&nbsp;:fas fa-check-circle: Owner
&nbsp;&nbsp;:fas fa-check-circle: Admin
&nbsp;&nbsp;:fas fa-check-circle: User

**Cost of Credit Points:** &nbsp;&nbsp;Free

--------------------------------------------------------------------------------

### add-focus

**Description**

Add the practitioners and/or metrics to be focused in the current channel.

The syntax of command is very flexible, you could use practitioner's name, mapped user or some
statements as "All Practitioners", "All Active Practitioners", "All Inactive Practitioners", etc.
to specify the practitioners to be focused.

The metrics should be listed with their correct ids.

This command could be called in a channel only.
It could be called by Owner or Admin, but not general users.

**Syntax**
```text
add-focus <practitioners> <metrics>
```

**Example**
```text
# add Jackie Newman and Izabella Solomon as focused practitioners and ia_arrived as focused metric
add-focus Jackie Newman @Bella ia_arrived

# add all active practitioners as focused practitioners and focus on ia_arrived and ia_revenue metrics
add-focus ia_arrived, ia_revenue from all active practitioners
```

**Availability:** 
&nbsp;&nbsp;:fas fa-check-square: Basic Plan
&nbsp;&nbsp;:fas fa-check-square: Standard Plan
&nbsp;&nbsp;:fas fa-check-square: Professional Plan  

**Roles Permission:**
&nbsp;&nbsp;:fas fa-check-circle: Owner
&nbsp;&nbsp;:fas fa-check-circle: Admin
&nbsp;&nbsp;:fas fa-circle: User

**Cost of Credit Points:** &nbsp;&nbsp;Free

--------------------------------------------------------------------------------

### remove-focus

**Description**

Remove the practitioners and/or metrics to be focused in the current channel.

It's taking reveresed action of `add-focus` with the same syntax and rules.

This command could be called in a channel only.
It could be called by Owner or Admin, but not general users.

**Syntax**
```text
remove-focus <practitioners> <metrics>
```

**Example**
```text
# remove Jackie Newman and Izabella Solomon from focused practitioners and ia_arrived from focused metrics
remove-focus Jackie Newman @Bella ia_arrived

# remove all inactive practitioners from focused practitioners
remove-focus all inactive practitioners
```

**Availability:** 
&nbsp;&nbsp;:fas fa-check-square: Basic Plan
&nbsp;&nbsp;:fas fa-check-square: Standard Plan
&nbsp;&nbsp;:fas fa-check-square: Professional Plan  

**Roles Permission:**
&nbsp;&nbsp;:fas fa-check-circle: Owner
&nbsp;&nbsp;:fas fa-check-circle: Admin
&nbsp;&nbsp;:fas fa-circle: User

**Cost of Credit Points:** &nbsp;&nbsp;Free

--------------------------------------------------------------------------------

### assign-task

**Description**

Create a task and assign task to one or multiple users.  _**Clinic Bees**_ will help to follow up the
execution of the task assignment with each individuals.

You could describe the task in whatever you'd like.  The message you sent will be kept as is, and
it will become the "home" of this task.  When task assignee fininshed the task, they need to reply
"Done" to close the action.  The timestamp of their reply will help to track the task execution.

You may also cancel the task by replying it with "Cancel".  You may also remind those not yet
taken action by replying "Remind", and we will tag the right users for attention.

The first line in task description will be used for summary of the task to be listed in individual's
task list.

>[!NOTE] 
>This commend could be called in public channel only to make sure all assignees will be able to access
it.

**Syntax**
```text
assign-task <task description>
```

**Example**
```text
assign-task
Please take the training course.
@Bella @Hedi
```

**Availability:** 
&nbsp;&nbsp;:fas fa-check-square: Basic Plan
&nbsp;&nbsp;:fas fa-check-square: Standard Plan
&nbsp;&nbsp;:fas fa-check-square: Professional Plan  

**Roles Permission:**
&nbsp;&nbsp;:fas fa-check-circle: Owner
&nbsp;&nbsp;:fas fa-check-circle: Admin
&nbsp;&nbsp;:fas fa-check-circle: User

**Cost of Credit Points:** &nbsp;&nbsp;Free

--------------------------------------------------------------------------------

### my-tasks

**Description**

List all the open tasks assigned or created.

**Syntax**
```text
my-tasks
```

**Availability:** 
&nbsp;&nbsp;:fas fa-check-square: Basic Plan
&nbsp;&nbsp;:fas fa-check-square: Standard Plan
&nbsp;&nbsp;:fas fa-check-square: Professional Plan  

**Roles Permission:**
&nbsp;&nbsp;:fas fa-check-circle: Owner
&nbsp;&nbsp;:fas fa-check-circle: Admin
&nbsp;&nbsp;:fas fa-check-circle: User

**Cost of Credit Points:** &nbsp;&nbsp;Free
