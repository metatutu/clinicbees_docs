### my-account

**Description**

Get the status of the account, so that owner could know the account subscription status and
remaining credit points in the account.

This command can be called by the Owner role only.  And it could be called with **bees** directly only.

**Syntax**
```text
my-account
```

**Availability:** 
&nbsp;&nbsp;:far fa-check-square: Basic Plan
&nbsp;&nbsp;:far fa-check-square: Standard Plan
&nbsp;&nbsp;:far fa-check-square: Professional Plan  

**Roles Permission:**
&nbsp;&nbsp;:far fa-check-circle: Owner
&nbsp;&nbsp;:far fa-circle: Admin
&nbsp;&nbsp;:far fa-circle: User

**Call Place:**
&nbsp;&nbsp;:fas fa-check-circle: Direct Message (to _**bees**_)
&nbsp;&nbsp;:fas fa-circle: Public channels

**Cost of Credit Points:** &nbsp;&nbsp;Free

--------------------------------------------------------------------------------

### install-cliniko

**Description**

Install Cliniko API key, so that system could prepare performance data from Cliniko.

>[!TIP]
>Please take reference to [Cliniko's article](https://help.cliniko.com/en/articles/1023957-generate-a-cliniko-api-key)
to obtain a valid Cliniko API key. 

This command can be called by the Owner role only and it could be called only once when system is initialized.

Once the Cliniko API key is installed, it will take 2-8 hours to prepare performance data from linked Cliniko account
before users could access it.

**Syntax**
```text
install-cliniko <Cliniko API key>
```

**Example**
```text
install-cliniko MS********czMDExMDYxMDM3NjQ0LVA2NDhlM2ViQ05xd2ZIOHd4dFNyMTRuaU5h********-***
```

**Availability:** 
&nbsp;&nbsp;:far fa-check-square: Basic Plan
&nbsp;&nbsp;:far fa-check-square: Standard Plan
&nbsp;&nbsp;:far fa-check-square: Professional Plan  

**Roles Permission:**
&nbsp;&nbsp;:far fa-check-circle: Owner
&nbsp;&nbsp;:far fa-circle: Admin
&nbsp;&nbsp;:far fa-circle: User

**Call Place:**
&nbsp;&nbsp;:fas fa-check-circle: Direct Message (to _**bees**_)
&nbsp;&nbsp;:fas fa-circle: Public channels

**Cost of Credit Points:** &nbsp;&nbsp;Free

--------------------------------------------------------------------------------

### health-check

Run a system diagnostics to check the system status.

>[!NOTE]
>This health check is depending on the command handling module up running.
>If there is no response even reaction on the command you sent, please contact customer support to get help.

**Syntax**
```text
health-check
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

### list-users

**Description**

List users and their roles.

**Syntax**
```text
list-users
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

### assign-admin

**Description**

Assign Admin role to one or multiple Slack users.

**Syntax**
```text
assign-admin <Slack users>
```

**Example**
```text
assign-admin @Dennis @Anna
```

**Availability:** 
&nbsp;&nbsp;:far fa-check-square: Basic Plan
&nbsp;&nbsp;:far fa-check-square: Standard Plan
&nbsp;&nbsp;:far fa-check-square: Professional Plan  

**Roles Permission:**
&nbsp;&nbsp;:far fa-check-circle: Owner
&nbsp;&nbsp;:far fa-circle: Admin
&nbsp;&nbsp;:far fa-circle: User

**Call Place:**
&nbsp;&nbsp;:fas fa-check-circle: Direct Message (to _**bees**_)
&nbsp;&nbsp;:fas fa-check-circle: Public channels

**Cost of Credit Points:** &nbsp;&nbsp;Free

--------------------------------------------------------------------------------

### revoke-admin

**Description**

Revoke Admin role from one or multiple Slack users.

**Syntax**
```text
revoke-admin <Slack users>
```

**Example**
```text
revoke-admin @Dennis @Anna
```

**Availability:** 
&nbsp;&nbsp;:far fa-check-square: Basic Plan
&nbsp;&nbsp;:far fa-check-square: Standard Plan
&nbsp;&nbsp;:far fa-check-square: Professional Plan  

**Roles Permission:**
&nbsp;&nbsp;:far fa-check-circle: Owner
&nbsp;&nbsp;:far fa-circle: Admin
&nbsp;&nbsp;:far fa-circle: User

**Call Place:**
&nbsp;&nbsp;:fas fa-check-circle: Direct Message (to _**bees**_)
&nbsp;&nbsp;:fas fa-check-circle: Public channels

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

--------------------------------------------------------------------------------
