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
&nbsp;&nbsp;:far fa-check-square: Basic Plan
&nbsp;&nbsp;:far fa-check-square: Standard Plan
&nbsp;&nbsp;:far fa-check-square: Professional Plan  

**Roles Permission:**
&nbsp;&nbsp;:far fa-check-circle: Owner
&nbsp;&nbsp;:far fa-check-circle: Admin
&nbsp;&nbsp;:far fa-check-circle: User

**Call Place:**
&nbsp;&nbsp;:fas fa-circle: Direct Message (to _**bees**_)
&nbsp;&nbsp;:fas fa-check-circle: Public channels

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

### show-performance

**Description**

Get the report of focused practitioners and metrics in the current channel and
show the performance in specified period with group option.

The period is essentially specified with a start date and end date in ISO 8601 form as YYYY-MM-DD.
For example, "2022-01-01 to 2022-12-31".  However, we supports much wider ways to specify the period
with the semi-natural language system.  For example, you may use "last 4 weeks", "last 12 months",
"year to date", "YTD", etc.  You could explore it by yourself to figure out the most comfortable
expression you like.

For group option, it supports `daily`, `weekly`, `monthly`, `quartterly` or `yearly`.
It will group data based on your preference specified in the command.

>[!NOTE]
The content of report is focusing on focused practitioners and metrics.  However, depends on plan
(for example, Professional plan could be with more analysis and smart content) and actual data 
(for example, if focused practitioners are not comparable, so related content could be hidden),
there could be with some slight difference.

**Syntax**
```text
show-performance <period> <group option>
```

**Example**
```text
# report of focused practitioners/metrics in current channel with data of full year 2022 grouped by week
show-performance 
Please provide weekly report between 2022-01-01 and 2022-12-31. 

# monthly report of year to date
show-performance
Monthly report of YTD.

# quarterly report of last 3 years
show-performance
Quarterly report of last 3 years.

# daily report of current month up to date
show-performance Daily report of MTD.
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
&nbsp;&nbsp;:fas fa-circle: Direct Message (to _**bees**_)
&nbsp;&nbsp;:fas fa-check-circle: Public channels

**Cost of Credit Points:** &nbsp;&nbsp;:fas fa-cart-shopping: 5 credit points

--------------------------------------------------------------------------------

### good-morning

**Description**

Get the daily preview report of a practitioner.
Daily preview report provides the overview of appointments and tasks of the day as
well as the hints and SOP to support individual to complete work.

>[!NOTE]
We strongly suggest to have practitioners to call command to query their own daily report
by themselves.  If you have to call command by Admin, make sure it's called in the channel
and the practitioner is in the channel focus, so that the query is transparent.

**Syntax**
```text
good-morning
```

**Example**
```text
# typically, practitioner query own report of the day
good-morning

# optionally, could specify practitioner and/or date
good-morning @Bella 2023-12-12
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

**Cost of Credit Points:** &nbsp;&nbsp;:fas fa-cart-shopping: 1 credit point

--------------------------------------------------------------------------------

### good-night

**Description**

Get the daily review report of a practitioner.
Daily review report provides the summary of appointments completed with hints.

>[!NOTE]
We strongly suggest to have practitioners to call command to query their own daily report
by themselves.  If you have to call command by Admin, make sure it's called in the channel
and the practitioner is in the channel focus, so that the query is transparent.

**Syntax**
```text
good-night
```

**Example**
```text
# typically, practitioner query own report of the day
good-night

# optionally, could specify practitioner and/or date
good-night @Bella 2023-12-12
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

**Cost of Credit Points:** &nbsp;&nbsp;:fas fa-cart-shopping: 1 credit point
