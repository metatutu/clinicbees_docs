### install-cliniko

**Description**

Install Cliniko API key, so that system could access performance data from the Cliniko account.

>[!TIP]
>Please take reference to [Cliniko's article](https://help.cliniko.com/en/articles/1023957-generate-a-cliniko-api-key)
to obtain a valid Cliniko API key. 

This command can be called by the Owner role only and it could be called only once when system is initialized.

Once the Cliniko API key is installed, it will take 2-6 hours to pull data from linked Cliniko account
before users could access performance data.

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

Run a system diagnostics to see whether system is up running normally.

>[!NOTE]
>This health check is depending on the command responding system is still running.
If the command is not even responded including reactions, please call customer support to resolve
the issue.

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
&nbsp;&nbsp;:fas fa-circle: User

**Cost of Credit Points:** &nbsp;&nbsp;Free

--------------------------------------------------------------------------------

### list-users

**Description**

List all users and their roles.

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

--------------------------------------------------------------------------------

### assign-admin

**Description**

Assign Admin role to a Slack user.

**Syntax**
```text
assign-admin <Slack user>
```

**Example**
```text
assign-admin @Dennis
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

Revoke Admin role from a Slack user.

**Syntax**
```text
revoke-admin <Slack user>
```

**Example**
```text
revoke-admin @Dennis
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