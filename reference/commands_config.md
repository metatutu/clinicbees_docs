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
map-practitioner Izabella Solomon=@Bella, Jackie Newman=@Jackie 

# You may also send the command in a multi-line message to make it clearer.
map-practitioner
Izabella Solomon=@Bella, 
Jackie Newman=@Jackie 

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

### list-practitioners

**Description**

List all practitioners from the linked Cliniko account and the mapping status with the Slack users.

**Syntax**
```text
list-practitioners
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

### focus-practitioners

**Syntax**
```text
channel-practitioners <Slack user 1>,<Slack user 2>...
```

--------------------------------------------------------------------------------

### focus-metrics

**Syntax**
```text
channel-focus <metric 1>,<metric 2>...
```

### show-focus