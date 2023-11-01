## Slack Configuration


This is the procedure on how to create _**Clinic Bees**_ app on your Slack workspace,
so that the app could work on your workspace.

This has to be done by the **Primary Workspace Owner** of your Slack workspace according
to Slack's rule.  It will take about 15 minutes to complete all the steps if you follow
up the instructions carefully.


### Step 1. Create new app

>[!TIP]
It requires few steps to go to **Your Apps** page on Slack as described below.  However, there is a shortcut
by opening the URL https://api.slack.com/apps/ and then you could start from the 4th step directly.

1. Open **Customize Workspace** in Slack.
![1](images/yourapps-1.png)

2. Click **ACCOUNT/Configure apps** from the left sidebar.
![2](images/yourapps-2.png)

3. Click **Build** on the top menu.
![3](images/yourapps-3.png)

4. Now you are on **Your Apps** page.  Click **Create New App**.
![4](images/yourapps-4.png)

5. Select **From an app manifest** from the configuration options.
![5](images/newapp-1.png)

6. Select the **workspace** where you want to install _Clinic Bees_, so that you and your team could work with _Clinic Bees_.
![6](images/newapp-2.png)

7. Copy and paste below content of app manifest in **YAML** box.

>[!NOTE]
As there is some default content in the box when opening the page, please clear them first and input content below completely.

```text
display_information:
  name: bees
features:
  bot_user:
    display_name: bees
    always_online: false
oauth_config:
  scopes:
    bot:
      - channels:history
      - chat:write
      - chat:write.public
      - files:write
      - groups:history
      - im:history
      - mpim:history
      - reactions:write
      - users:read
      - files:read
settings:
  event_subscriptions:
    bot_events:
      - message.channels
      - message.groups
      - message.im
      - message.mpim
  interactivity:
    is_enabled: true
  org_deploy_enabled: false
  socket_mode_enabled: true
  token_rotation_enabled: false
```
![7](images/newapp-3.png)

8. Simply click **Create**, the app will be created immediately.
![8](images/newapp-4.png)


### Step 2. Create App token

>[!TIP]
App token is one of 2 tokens Clinic Bees needs to get so that it could work with your workspace.

1. Click **Settings/Basic Information** from the left sidebar.
![1](images/apptoken-1.png)

2. Scroll down the page to **App-Level Tokens**, click **Generate Token and Scopes**.
![2](images/apptoken-2.png)

3. Input **Token Name** and add the **Scope**, then click **Generate**.

```text
Token Name: clinicbees
Scope: connections:write (you may select from the list by clicking Add Scope)
```
![3](images/apptoken-3.png)


4. Copy and save the token, and click **Done** to close the window.

>[!NOTE]
The app token is typically as "xapp-...".  Please record the token safely. 

![4](images/apptoken-4.png)

### Step 3. Customize the app icon

>[!TIP]
Actually you may take this step whenever you'd like.  However, the settings of **Display Information** is right below
the **App-Level Token**, so you may consider to set it up now.

Simply upload the icon image and set it up according to Slack's instruction.
![0](images/changeicon-1.png)

You may use **Clinic Bees** default logo as below after you saved it before you upload it to Slack.
![0](images/clinicbees_slack_logo.png)

### Step 4. Enable direct message

1. Click **Features/App Home** from the left sidebar.

2. Scroll down the page to **Your App's Presence in Slack**, turn on **Always Show My Bot as Online**.
![1](images/apphome-1.png)

3. Scroll down the page to **Show Tabs**, check **Allow users to send Slash commands and messages from the message tab**.
![2](images/apphome-2.png)

>[!TIP]
If Slack user would still not be able to send message directly to **bees** with below message on Slack client app, simply restart the Slack client app.
![3](images/apphome-3.png)

### Step 5. Create OAuth token

>[!TIP]
OAuth token is one of 2 tokens Clinic Bees needs to get so that it could work with your workspace.

1. Click **Features/OAuth & Permissions** from the left sidebar, and then click **Install to Workspace** in
section of **OAuth Tokens for Your Workspace**.

![1](images/oauthtoken-1.png)

2. Click **Allow** to grant the permissions to the app.

![2](images/oauthtoken-2.png)

3. Copy and save the token.

>[!NOTE]
The OAuth token is typically as "xoxb-...".  Please record the token safely. 

![3](images/oauthtoken-3.png)

### Congratulations!

Congratulations!  Now, you have your Slack workspace configured.

Please provide the app token (xapp-...) and OAuth token (xoxb-...) to _**Clinic Bees**_ team per requested.

Upon your payment of initial setup fee and first month's service fee received, we will configure the **Clinic Bees**
app for your workspace shortly, and then you could start chatting with **@bees**.
