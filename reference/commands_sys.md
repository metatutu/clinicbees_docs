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
&nbsp;&nbsp;:fas fa-check-square: Basic Plan
&nbsp;&nbsp;:fas fa-check-square: Standard Plan
&nbsp;&nbsp;:fas fa-check-square: Professional Plan  

**Roles Permission:**
&nbsp;&nbsp;:fas fa-check-circle: Owner
&nbsp;&nbsp;:fas fa-circle: Admin
&nbsp;&nbsp;:fas fa-circle: User

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
&nbsp;&nbsp;:fas fa-check-square: Basic Plan
&nbsp;&nbsp;:fas fa-check-square: Standard Plan
&nbsp;&nbsp;:fas fa-check-square: Professional Plan  

**Roles Permission:**
&nbsp;&nbsp;:fas fa-check-circle: Owner
&nbsp;&nbsp;:fas fa-check-circle: Admin
&nbsp;&nbsp;:fas fa-check-circle: User

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
&nbsp;&nbsp;:fas fa-check-square: Basic Plan
&nbsp;&nbsp;:fas fa-check-square: Standard Plan
&nbsp;&nbsp;:fas fa-check-square: Professional Plan  

**Roles Permission:**
&nbsp;&nbsp;:fas fa-check-circle: Owner
&nbsp;&nbsp;:fas fa-check-circle: Admin
&nbsp;&nbsp;:fas fa-check-circle: User


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
&nbsp;&nbsp;:fas fa-check-square: Basic Plan
&nbsp;&nbsp;:fas fa-check-square: Standard Plan
&nbsp;&nbsp;:fas fa-check-square: Professional Plan  

**Roles Permission:**
&nbsp;&nbsp;:fas fa-check-circle: Owner
&nbsp;&nbsp;:fas fa-circle: Admin
&nbsp;&nbsp;:fas fa-circle: User

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
&nbsp;&nbsp;:fas fa-check-square: Basic Plan
&nbsp;&nbsp;:fas fa-check-square: Standard Plan
&nbsp;&nbsp;:fas fa-check-square: Professional Plan  

**Roles Permission:**
&nbsp;&nbsp;:fas fa-check-circle: Owner
&nbsp;&nbsp;:fas fa-circle: Admin
&nbsp;&nbsp;:fas fa-circle: User

**Cost of Credit Points:** &nbsp;&nbsp;Free

--------------------------------------------------------------------------------