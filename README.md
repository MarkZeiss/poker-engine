# Poker-Engine v3 documentation
This documentation is the official documentation for Poker-Engine v3

*English version*

This comprehensive documentation provides detailed information on all the customization options available in the poker-engine v3 software. The software can be found directly at [poker-engine.com](https://poker-engine.com), and a demo version is also available at [demo.poker-engine.com](https://demo.poker-engine.com).

The different categories under which the customizations are organized include:

1. [Admin Panel](#admin-panel):

- [Tables](#tables): Configure and manage poker tables.
- [Tournaments](#tournaments): Set up and run poker tournaments.
- [Styles](#styles): Customize the appearance of the game tables.
- [User Management](#users): Manage user accounts and permissions.
- [Groups](#groups): Organize users into groups for easier management.
- [Bonuses](#admin-bonuses): Set up promotional bonuses for users.
- [Affiliate Program](#affiliate): Implement an affiliate marketing program.
- [Mailing Lists](#mailing): Manage email communication with users.
- [Agency Program](#agent): Create and manage agent accounts.
- [Cashier Settings](#admin-cashier): Configure payment and withdrawal options.
- [Payment Systems](#payment): Integrate different payment gateways.
- [Cryptocurrencies](#cryptocurrencies): Support digital currencies for transactions.
- [Coupons](#coupons): Create and manage promotional coupons.
- [Transactions](#transactions): Track and manage user transactions.
- [Server Settings](#server): Configure server-related settings.
- [General Settings](#general): Set up essential software configurations.
- [Game Settings](#game): Customize various aspects of the poker game.
- [Mailing List Settings](#templates): Configure email communication settings.
- [Addons](#addons): Enhance the software with additional features.
- [Language Settings](#languages): Customize the language used in the software.
- [Registration Settings](#signup): Set up user registration options.
- [Navigation Settings](#navigation): Customize the software's navigation menu.
- [Process Management](#processes): Manage background processes and tasks.
- [Configuration](#configuration): Access and modify system configurations.
- [Page Editor](#editor): Edit and customize the software's web pages.
- [Messages](#messages): Manage system messages and notifications.
- [Updates](#updates): Keep the software up to date with the latest version.
- [Admin Panel Settings](#panel): Configure the admin panel itself.

2. [User](#user):

- [User Profile](#user-profile): Update and manage user profile details.
- [User Details](#user-details): Personal Details.
- [Password](#user-password): Change and reset user passwords.
- [Bonuses](#user-bonuses): View and redeem available bonuses.
- [Affiliate Program](#user-affiliate): Access and manage affiliate program details.
- [Agent Program](#user-agent): View and track agent program information.
- [User Settings](#user-settings): Manage general account settings.

3. [Lobby](#lobby): Access the poker lobby interface.

By referring to this documentation, customers can gain a comprehensive understanding of the poker-engine v3 software and effectively tailor it to their specific needs and preferences.

## <a name="admin-panel"></a> Admin Panel

### <a name="tables"></a> Tables

To create, edit, and delete game tables, go to the `Games` > `Tables` section in the admin panel.

To create a new table, click on the `New table` tab.

**Game**: By default, the game is set to Texas Hold'em.

**Table name**: The table name is displayed in the list of tables and in the lobby.

**Table mode**: Choose between real money or virtual chips.

**Table type**: Select between Public or Private. If you choose Private, an additional field for password entry will appear. Private tables are not displayed in the lobby, but the corresponding icon will appear in the list of tables in the admin panel. To play at a private table, players need to click on "Playing with friends" in the lobby, then select "Join the game," enter the table name, and password.

**Minimum buy-in**: Set the minimum buy-in for the table. You can choose from the provided options or specify your own amount, to do this click on the `choose another` link below the list of options.

**Maximum buy-in**: Determine the maximum buy-in for the table. Choose from the provided options or specify your own amount, to do this click on the `choose another` link below the list of options.

**Small blind**: Set the small blind for the table. Choose from the provided options or specify your own amount, to do this click on the `choose another` link below the list of options.

**Big blind**: Determine the big blind for the table. By default, it is set to twice the small blind. Choose from the provided options or specify your own amount, to do this click on the `choose another` link below the list of options.

**Number of players**: Select the number of players the table will accommodate. Options include 9, 6, 4, and 2.

**Rake**: Enter the percentage of winnings that will be charged as a commission at the table. Enter 0 if no commission is to be charged. Use a dot to separate decimal numbers.

\
Click the `Tables` tab to view the list of tables.

Use the search bar to find specific game tables.

The list of tables can be sorted by clicking on the column names. Sort options include *Table Name*, *Players*, *Table Mode* (Cash, Virtual Chips, Tournament), *Buy-in*, and *Bets* (Small Blind/Big Blind).

On the right side of each table, there are icons representing possible actions.

**Pause game**: Pause the game at the table. Players will hear a sound indicating the table has been paused, and the word "paused" will appear in the upper left corner of the table. No action can be taken during a pause.

**Open table**: Open the table in a new tab in debug mode. This allows you to view all cards in the current hand and perform additional actions such as disconnecting a player (click on the desired player to open the action menu). You can also take actions on behalf of any player before their turn. To increase a player's stack, click on your login in the top right corner and select `Increase the stack`.

**Add bot**: Add a pre-created bot to the table. They can be created in the [user management](#users) section. Select the bot and specify its initial stack, regardless of the table settings.

**Delete bot**: Remove a bot from the table. You can also disconnect the bot in debug mode.

**Set the cards for the next hand**: Open a window to set the board cards and individual cards for each player. Click `OK`, and these cards will be dealt in the next hand. This allows you to test complex combinations or split pots.

**Disable bot actions**: Prevent bots at the table from performing any actions.\
**Enable bot actions**: Allow bots at the table to resume their usual actions.

**Table history**: Open the detailed history of the table, including player actions, administrator actions, and stack changes.

**Stop the table**: Disable play at the table and remove it from the lobby. Note that this action can only be taken when there are no players at the table. If players are present, a corresponding message will be displayed.\
**Run the table**: Make the table available again and display it in the lobby.

**Delete the table**: The table will be deleted after a delay of 1-2 seconds. Note that this action is not possible while players are at the table.

**Edit the table**: Open the page to modify the table parameters. It is not recommended to make changes during the game process.

Click on the `Table history` icon to view the complete history of the table, including player actions, administrator actions, and stack changes. You can update the history at any time by clicking the `Refresh data` button. The history includes columns for *Event* (description of the event), *Game number* (unique hand number when the event occurred), *Value* (event value, such as numerical values or text descriptions), *User* (the player associated with the event or empty value), and *Time* (the timestamp of the event).


### <a name="tournaments"></a> Tournaments

To manage game tournaments, access the `Games` > `Tournaments` section in the admin panel.

Creating a New Tournament\
To create a new tournament, click on the `New tournament` tab.

**Game**: The default game is Texas Hold'em.

**Tournament name**: The name of the tournament will be displayed in the list of tournaments and in the lobby.

**Private tournament**: If selected, a password field will appear. Participants will need to enter this password to join the tournament.

**Game currency**: Choose between *USD* or *Tournament Tickets* as the currency required for participation.

**Buy-in**: Specify the buy-in amount from the provided list or enter your own value by clicking on `choose another`. You can also choose not to charge a buy-in by setting it to 0.

**Rake**: This is the commission for participating in the tournament. It will be added to the buy-in and is not included in the prize pool. Set the rake to 0 if you do not want to charge a commission.

**Number of chips**: Determine the number of chips each player will start with in the tournament, as well as during rebuy or re-entry.

**Level time**: This is the duration in seconds, e.g. 300 seconds (5 minutes), after which the ante, small blind, and big blind increase.

**Ante**: Mandatory bid at the beginning of each hand. Select from the list or enter a custom value.

**Ante grow**: After the specified interval in *Level time*, the ante will increase by the specified value or multiply by the specified value (indicate "x" before the value).

**Start small blind**:  Choose the value of the initial small blind or enter a custom value.

**Start big blind**: Choose the value of the initial big blind or enter a custom value.

**Blind grow**: After the interval specified in *Level time*, the small and big blinds will increase by the specified value or multiply by the specified value (indicate "x" before the value).

**Number of Players**: Determine the number of participants at each table. Options include 9, 6, 4, or 2 players.

**Minimum players**: Specify the minimum number of registered participants required to start the tournament. Bots are also counted.

**Maximum players**: Set the maximum number of participants allowed in the tournament, including bots.

**Allow Sitout**: Enabling this option allows players to save their seat at the table without actively participating in the game.

**Tournament start**: Set the exact time and date for the tournament to start. Players will be seated approximately 1 minute before the tournament begins.

**Late registration**: Specify the duration of late registration from the start of the tournament in seconds.

**Renewal of the tournament**: This option allows for automatic recreation of the tournament. The available options include: *Disable*, *Interval after completion*, and *Renewal period*.\
**Interval after completion**: The tournament will be recreated after a certain period of time at the end of the previous tournament. The value is specified in seconds, e.g. 86400 (24 hours). This setting remains in effect until the tournament is manually removed.\
**Time to register**: Specify the time allowed for registration in a tournament after it is automatically created. The value is specified in seconds, e.g. 3600 (1 hour).\
**Renewal period**: Choose one of the available values, such as *Every day*, to create the tournament at the same time each day.\
**Time to register**: Specify the time allowed for registration in the tournament. Since the tournament is created in advance, this value determines the registration time. The value is specified in seconds, e.g. 1800 (30 minutes).

**Allow Rebuy**: Rebuy allows a player who has lost all their chips to buy another stack of chips and continue playing at the same table without leaving their seat.\
**First interval**: Set the duration in seconds from the start of the tournament during which players can rebuy. For example, 3600 (1 hour) allows rebuys within the first hour.\
**Number of possible rebuys**: Determine the maximum number of rebuys allowed during the specified first interval. Set to 0 for no limit.\
**Second interval**: Set the duration in seconds after the first interval during which players can rebuy. For example, 300 (5 minutes) allows rebuys for 5 minutes following the end of the first interval.\
**Number of possible rebuys (2)**: Specify the maximum number of rebuys allowed during the specified second interval. Set to 0 for no limit.\
**Standby time**: If a player does not rebuy within this time, they will no longer participate in the tournament and their seat will become vacant. Specify the duration in seconds, e.g. 300 (5 minutes).

**Allow Re-entry**: Re-entry allows a player who has lost all their chips to leave the table and pay to re-enter the tournament as a new player. They will receive a full starting stack of chips and be assigned to a random seat.\
**Re-entry interval**: The re-entry interval specifies the time period, measured in seconds, during which players can re-enter the game. For example, a re-entry interval of 1800 means players can re-enter within 30 minutes after the tournament starts.\
**Number of possible re-entries**: Players are allowed to make a certain number of re-entries within the specified time interval. Set to 0 for no limit.

**The prize fund**: There are two types of prize funds available:\
*Fixed Prize Fund*: In this option, a predetermined amount is allocated as the prize fund. This amount is then divided among the winners of the tournament.\
*Accounting for Players*: The total amount of all players' contributions (buy-in) is divided among the winners of the tournament.\
**The amount of the prize fund**: When selecting the *Fixed Prize Fund* option, the amount of the prize fund is indicated.

Placement Prizes: Indicate the percentage of the prize pool for each placement in the tournament. For example:

**1st place**: Percentage of the prize pool allocated for the winner.\
**2nd place**: Percentage of the prize pool allocated for the second-place winner.\
**3rd place**: Percentage of the prize pool allocated for the third-place winner.\
**...**\
**15th place**: Percentage of the prize pool allocated for the fifteenth-place winner.

> Once the tournament begins, tables will be promptly created and players will be seated one minute prior to the start time. A notification will be displayed in the lobby, alerting users about the tournament kick-off, and they will be swiftly moved to their designated tables. These newly created tables can be easily accessed by navigating to `Game` > `Tables`, where they will be listed as tables in *Tournament* mode, denoted by their format *Tournament name {table#n}*.
> 
> Experience the excitement of competitive poker at your fingertips!

\
To view the list of tournaments, click on the `Tournaments` tab.

To find specific tournaments, use the search bar.

You can sort the list of tournaments by clicking on the column names. The available sort options are *Tournament Name*, *Players*, *Buy-in*, *Start time*, and *Status* (Registration / Running / Completed / Canceled).

On the right side of each tournament, you will find icons representing possible actions.

**Add bot**:  This allows you to add a pre-created bot to the table. Bots can be created in the [user management](#users) section. Once added, the bot's username will be visible to users in the list of registered players.

**Delete bot**: You can cancel the participation of a specific bot in the tournament by clicking on this icon.

**Edit tournament**: Clicking on this icon will open the page where you can modify the tournament parameters. If any changes are made, registered users will immediately receive an email notifying them of the changes.

**Remove tournament**: You cannot delete a tournament if there are players at least on one table.

**Game results**: Tournaments with the status *Completed* and *Running* always allow you to view the results of the game. Clicking on this icon will open a new page with the list of players and their results.

### <a name="styles"></a> Styles

To edit the table logo and add a new table style, go to the `Games` > `Styles` section in the admin panel.

The `Styles` tab displays all available table styles. One style is available by default. To change the table logo, click on the *Change the logo* icon next to the desired style.

Next, you can choose between *Text* or *Image* options.

If you select *Text*, you can enter the text that will appear on the game table.

You can also choose the desired color for the text using the color selection tool.

Specify the font size of the displayed table text (from 7 to 42) using the size option.

Click the `Save` button to apply the changes, and you will immediately see the new table image.

If you select *Image*, you can upload an image from your computer in PNG format. Once uploaded, it will appear in the list of available images below.

In the list of available images, there are two icons in front of each image.

Clicking on the icon allows you to change the table logo. A confirmation dialog box will appear, and you can select *Yes* or *Cancel* to proceed. When you save the changes, the table image will immediately be updated with the new logo.

You can permanently remove an uploaded image from the list of available logos by clicking on the *Delete the image* icon. Deleting an image will not delete or modify an existing table logo.

\
Clicking on the `My style` tab allows you to load a new table style.

The table style should be a zip archive containing the following files:

- *style.conf.php* - style configuration
- *cards* folder
- *css* folder
- *images* folder
- *sounds* folder

An example of a configuration file is shown below:

> Table6x\
> 6\
> preview.png\
> table.css\
> table_origin.jpg

- The first line is the name of the style, which will be displayed in the list of styles.
- The second line is the maximum number of players for which the table is designed (9, 6, 4, or 2).
- The third line is the name of the image with the table preview, which should be in the *images* folder.
- The fourth line is the name of the table style CSS file, which should be in the *css* folder.
- The fifth line is the name of the image of the table itself, which should be in the *images* folder.

The table image should not include the table logo. The table preview is a thumbnail image of the original table image, approximately 700x530 pixels in size. In the style archive, add a very small preview image (approximately 280x212 pixels) with the name *{preview_name}_thumb.{preview_extension}*, to be displayed in the style list. For example, if the preview image is *my_preview.jpg*, then the thumbnail image should be *my_preview_thumb.jpg*.

Styles are loaded into the `../Games/Styles` folder. After loading, to activate a style, open the list of styles and click on the *Activate* icon next to the new style. The main style is located in the `../Games/Styles/table9x` folder. You can use the necessary material from this folder as a basis for creating your new style. In many cases, you may only need a new table image, as all other elements can be copied from the default style folder.


### <a name="users"></a> User Management

To manage users, including creating, editing, and deleting them, follow these steps

1. Go to the admin panel and navigate to the `Users` > `Managing` section.
2. To create a new user, click on the `New` tab.
3. Enter the following details for the user:

**Username**: Enter the username for the game account. You can use English letters, numbers, and the underscore symbol.

**Password**: Set a password for the account.

**Group**: Select the user group from the options available. You can create new groups in the [group management](#groups) section.

**Balance**: Set the initial balance for the user's account or leave it at 0.

**Virtual Account Balance**: Set the initial balance for the user's virtual currency account or leave it at 0.

**E-mail**: Provide the user's email address.

4. Click on `Additional information` to access additional fields for entering data.
- Here, you can specify the user's *Name*, *Last Name*, *Avatar*, *Gender*, *Birthday*, *Phone number*, *Zip code*, *Address*, *Country* and *City*.
5. You can also define the following parameters:

**Bot**: Indicate whether the account being created is a bot. Bots can be attached to the game at any time.

**Designated Agent**: Assign an agent for the user. The designated agent will profit from that player according to the agent program settings.

**Agent**: Determine whether the user is an agent. Agents can be assigned to other players and have special profit conditions.

6. Once all the fields are filled in, click on the `Create an Account` button.

\
To view the list of users, follow these steps

1. Click on the `Users` tab.
2. To search for specific users, use the search bar.
3. You can sort the list of users by clicking on the column names. The available options for sorting include *Username*, *Balance*, *Group*, *Rank*, *Email*, *Creation date*, and *IP address*. *Email* and *IP address* will be hidden if you do not have sufficient authorization.

On the right side of each user in the list, you will find icons representing different actions you can take:

**Approve Registration**: If your [registration settings](#signup) require email confirmation or manual approval, and the user has not confirmed their registration, you can confirm the account by clicking this icon.

**Confirm Email Address**: Click this icon to manually confirm the user's email address. An email address is marked as unconfirmed if it has been changed in the profile settings. Confirming an email address ensures that it is valid and can be used to receive email messages. 

**Operations History**: Click on this icon to view all user balance activities.

**Edit the Profile**: Click on this icon to edit the user's account details.

**Block the Account**: Click on this icon to ban the account. The user will not be able to log in or perform any actions.\
**Unlock the account**: Click on this icon to make the account available for login again.

**Remove the Player**: Click on this icon to delete the account, along with all related information such as statistics and uploaded avatars.

> Additionally, if you click on the `Operations History` icon, you can choose to view specific information such as *Referral Accruals*, *Bonuses*, *Deposits*, *Withdrawals*, *Internal Transfers*, *Cash Tables*, and *Tournaments*. By default, all operations are selected, and you can update the history by clicking the `Refresh Data` button.

### <a name="groups"></a> Groups

To manage user groups, such as creating, editing, and deleting them, navigate to the `Users` > `Groups` section in the admin panel.

Creating a new group is as simple as clicking on the `New Group` tab.

Here are the details you need to provide to create a group:

**Group name**: Enter a name for the group.

**Access rights**: Define the access rights for users belonging to this group.

The following access rights can be assigned:

> *a* - User can perform all actions and access the admin panel.\
*a1* - User can manage tables and tournaments within the admin panel.\
*b* - User is allowed restricted access to the admin panel. They cannot use the code editor, modify or customize the cashier, send letters, or perform actions on users and groups.\
*c* - User can use the moderator panel.\
*d* - User can log in to their account and perform actions on it.\
*e* - User can log in to their account but cannot edit or change settings.\
*f* - User can log in to their account but cannot perform any actions.

\
To view the list of groups, click on the `Groups` tab.

The list of groups can be sorted by clicking on the column names such as *Name*, *Access rights*, and *Users*.

Each group in the list has icons on the right side representing possible actions.

You can perform the following actions on a group:

**Group settings**: Click to edit the settings of the group.

**Delete the group**: Removes the selected group.

### <a name="admin-bonuses"></a> Bonuses

To access and manage bonuses and view the history of bonus accruals, go to the `Users` > `Bonuses` section in the admin panel.

To create a new bonus, click on the `New` tab.

Here are the details you need to provide when creating a bonus:

**Bonus description**: Enter a description for the bonus.

**Bonus event**: Select the event for which the bonus will be credited. The available options are:
- *When replenishing an account*: the bonus will be credited with each deposit to the internal account.
- *At the first replenishment*: the bonus will be credited only on the first deposit to the internal account.
- *After the first authorization*: the bonus will be credited only after authorization of a newly created account.

**Bonus Type**: Choose the type of bonus to be credited. This can be:
- *Virtual money*
- *USD* - default currency
- *Tournament tickets*

**Bonus amount**: Specify the exact number. If the bonus is determined by a percentage of the deposit amount, add the % symbol. To indicate decimal numbers, use a dot.

**Start date**: Enter the exact date and time when the bonus offer will be activated.

**Expiration date**: Choose the end date after which the bonus will no longer be valid.

\
Click the `Bonuses` tab to view the list of created bonuses.

You can use the search bar to find a specific bonus.

The list of bonuses can be sorted by clicking on the column names. The available sorting options include *Bonus description*, *Bonus event*, *Bonus Type*, *Amount*, and *Validity*.

On the right side of each bonus, there are icons representing possible actions.

**Stop**: Terminate the bonus offer.

**Edit**: Modify the parameters of the bonus offer.

**Delete**: Remove the bonus offer.

\
Click on the `History` tab to view the history of bonus accruals.

You can use the search bar to find the specific username to which the bonus was credited.

The list of accruals history can be sorted by clicking on the column names. The available sorting options include *Bonus name*, *Username*, *Bonus Type*, *Balance before accrual*, *Balance after accrual*, and *Accrual time*.

### <a name="affiliate"></a> Affiliate Program

Poker-Engine offers an integrated affiliate program that allows registered users to earn rewards for referring new players. Each user receives a unique referral link with a login, which, when clicked and used for registration, assigns a referrer to the new player. The referrer then receives a reward based on the deposits made by the player registered through their link. This reward can be a percentage of the deposit or a fixed amount. Additionally, the affiliate program provides the flexibility of creating multiple referral levels, which makes it even more attractive. If your referral successfully registers someone through their unique affiliate link, both you and the referrer will start receiving rewards for the deposits of the invited players.

To access and manage referral levels and view the statistics of affiliate accruals, navigate to the `Users` > `Affiliate Program` section in the admin panel.

To create a new referral level, click on the `Referral levels` tab and then click the `Add level` button. A window will appear where you can enter the reward size by specifying the amount of remuneration. If the amount is defined as a percentage of the deposit, include the % symbol. For decimal numbers, use a dot as the separator. Click the `Ok` button to add the new level to the list of referral levels. The level number is automatically assigned based on the number of existing levels and cannot be changed. You can create multiple levels and modify the reward for any level at any time. To change the reward, click on the `Change` icon next to the desired level. To delete a level, simply click on `Delete`.

To view reward statistics, switch to the `Statistics` tab. You can use the search bar to find specific usernames and see which rewards have been credited to them. The list of statistics can be sorted by clicking on column names such as *User*, *Referral*, *Level*, *Reward*, and *Accrual time*.

### <a name="mailing"></a> Mailing Lists

To check the status of sent emails and create a new mailing, navigate to the `Users` > `Mailing` section.

To create a new mailing, follow these steps:

**Mailing template**: Select a mailing template that has been created in the [mailing list settings](#templates).

**Recipients**: Choose recipients based on available parameters or manually specify them.

**Generate coupons**: Select yes or no to automatically generate coupons. These coupons will be visible in the [coupon list](#coupons). Use this option only if the mailing template supports coupon insertion into the template body.\
**Coupon currency**: Set the game currency that will be associated with the coupons.\
**Coupon value**: Determine the value for the coupons.\
**Coupon expiration date**: Specify the exact date and time for coupon expiration. Leave the field blank if no expiration date is needed.\
**Characters**: Define the number of symbols each coupon should contain. The default value is 10.

After completing the above steps, click on the `Send letters` button. A message displaying the estimated mailing time will appear. Confirm or cancel the mailing by clicking the respective buttons.

To check the current sending status, click on the `Mailing history` tab.

### <a name="agent"></a> Agency Program

The Poker-engine offers a built-in functionality for assigning and managing agents, which can be highly beneficial in promoting your online poker room. By assigning agents to players, you can provide them with a profit in their internal agent account based on the players' gameplay, including wins and losses. Agents have the ability to view statistics on their profits, analyze them, and transfer funds from their agent account to the balance of their assigned players. The administrator has the authority to view all agents and their statistics, as well as transfer funds from the agent account to the players assigned to the agents.

To effectively manage and configure the agent program, access the admin panel and navigate to `Users` > `Agent Program`.

In the `Settings` tab, you can configure the general settings of the agent program.

**Profit of agents**: Enable or disable this feature. If enabled, user agents will have special profit terms applied.

**Profit percentage**: Specify the percentage of profit. Agents assigned to players will earn a profit based on the table rake. No profit will be accrued if the rake is 0.

**Accrual mode**: Choose when the profit should be credited to agents. Options include *When winning and when losing*, *Only in case of winning*, and *Only on loss*.

Save your changes by clicking the `Save` button.

\
To manage agents, navigate to the `List of agents` tab.

The list of agents can be sorted by clicking on the column names. Sorting options include *Username*, *Profit percentage*, *Agent balance*, *Assign* (the user who assigned the agent), *Assigned time*, and *Users* (the number of users assigned to the agent).

On the right side of each agent, there are icons representing various actions.

Clicking on *Change settings* allows you to modify the settings for the agent account. In the appearing window, you can edit the *Account balance* by adjusting the balance of the user's agent account, and choose the *Profit mode* between *Follow the general rule* or *Specify manually*. If you select *Specify manually*, an additional option called *Profit percentage* will appear, allowing you to enter a specific profit percentage for this agent. Agents assigned to players will earn a profit if these players win, depending on the rake amount. No profit will be accrued if the rake is 0. Click the `OK` button to save the changes.

Clicking on *List of users* will display the statistics of the assigned users.

The list of users can be sorted by clicking on the column names. Sorting options include *Username* and *Profit*.

On the right side of each user, there are icons representing various actions.

Clicking *Send funds* opens the Amount entry window. Here, you can enter the amount to be transferred from the agent's account to the selected user's balance. The total available for sending will be equal to the amount in the agent's account.

Clicking on *Detailing* allows you to view a detailed history of agent rewards from the user.

The list of rewards can be sorted by clicking on the column names, including *Table ID*, *Rake*, *Amount*, and *Time*.

### <a name="admin-cashier"></a> Cashier Settings

To access the cashier settings, navigate to the administrator panel and click on `Cashier` > `Settings`.

Currency Settings:

- Click on the `Currency` tab to configure currency settings.
- **Currency code**: This code represents the main currency and is displayed when selecting a currency. The default currency code is USD.
- **Currency symbol**: The currency symbol is displayed next to the numeric value of the currency (e.g., user balance, buy-in, blinds). The default currency symbol is $.

Verification Settings:

- Click on the `Verification` tab to configure verification settings.
- **Deposit limit 1**: Set the deposit limit for users who have not yet passed verification. Use 0 for no limit. Decimal numbers should be separated by a dot.
- **Deposit limit 2**: Set the deposit limit for users who have passed verification. Use 0 for no limit. Decimal numbers should be separated by a dot.
- **Minimum amount for withdrawal**: Set the minimum amount required for a user to request a withdrawal. Use 0 to disable this option.
- **Commission for withdrawal**: Specify the percentage of commission charged for withdrawing funds from the user's balance. Use 0 for no commission.
- **Restrictions on withdrawal 1**: Set a withdrawal limit for users who have not passed verification. Use 0 for no limit.
- **Restrictions on withdrawal 2**: Set a withdrawal limit for users who have passed verification. Use 0 for no limit.
- **Transfers**: Enable the ability to send funds to other users, even if the user has not passed verification.

Remember to click on the `Save` button to save your changes.

### <a name="payment"></a> Payment Systems

To set up payment systems, navigate to the `Cashier` section and click on `Payment Systems`.

To configure payment systems for withdrawals, go to the `Withdrawal` tab. Here, you can enable or disable specific payment systems and configure API keys for certain systems. All withdrawal requests will be displayed in the [messages](#messages) section.

To set up payment systems for depositing funds, click on the `Deposit` tab. Here, you can enable or disable different payment systems, configure secret keys for signing, and add wallet addresses to accept funds. All payments will be automatically credited to the user's internal account.

We currently support a variety of payment systems and gateways, including Paypal, Payeer, Coinpayments, and others. We are continuously adding new payment options based on our customers' requests.

Don't forget to click on the `Save` button to ensure that your changes take effect.

### <a name="cryptocurrencies"></a> Cryptocurrencies

Introducing Cryptocurrencies with Poker-Engine: Simplify and Streamline Payments on Your Website

With Poker-Engine, you can seamlessly accept cryptocurrencies on your website, eliminating the need for third-party integration. All you need is your wallet address to start accepting funds. Our payment processing module will automatically reconcile the balance on your wallet and credit the payments. To optimize server resources, our module doesn't require node loading. Instead, you can easily check your wallet balance by accessing the *API url*.

Our cryptocurrency interface not only facilitates payment processing but also offers additional features to enhance your experience. You can now configure Blockchain and Cryptocurrency settings, as well as customize rate updates effortlessly. Simply navigate to `Cashier` > `Cryptocurrencies` to access these functionalities.

\
To configure rate updates, go to the `Settings` tab.

**Price URL**: This is the URL that provides the data needed to update the cryptocurrency price. By default, it uses the Coingecko API: https://api.coingecko.com/api/v3/coins/markets?vs_currency=usd&ids=%ids&order=market_cap_desc&sparkline=false. If you plan to change the address to another service, ensure that the data accepts identifiers via GET parameters. For example, you can use ids=%ids, where %ids will be replaced with ids=ethereum,tether (a comma-separated list of all active cryptocurrencies). Currency identifiers can be customized when adding a cryptocurrency.

**Price hold**: Specify the duration for which the price value should be retained after the user specifies the desired top-up amount. This value is indicated in seconds. For example, setting it to 300 means the price will be held for 5 minutes.

\
To manage blockchains, click on the `Blockchains` tab.

To add a new blockchain, click on the `Add blockchain` button.

In the window that appears, enter the following parameters:

**Name**: This is the name that will be displayed when users choose a blockchain, such as *Ethereum Mainnet*.

**Blockchain ID**: This is the identifier for the blockchain (a number, e.g. *42* for *Kovan Test Network*).

**API URL**: Enter the URL that retrieves a list of transactions by address. Please ensure you use an API key to increase the rate limit.

**API URL (TOKEN)**: Enter the URL that retrieves a list of transactions by the contract address. Again, use an API key for a higher rate limit.

**API2 URL**: Enter the URL that returns the last block from the blockchain. Remember to use an API key for a higher rate limit.

Click the `OK` button.

The new blockchain will now appear in the list of blockchains. To edit its parameters, click on the *Blockchain parameters* icon. To delete it, click on *Delete blockchain*.

\
To add a new cryptocurrency to your platform, click on the `Add cryptocurrency` tab. 

**Type**: By default, it is set as an *Ethereum-based* currency.

**Method name**: This is the name of the deposit method, which will also be used in the cashier to allow users to select a payment method. For example, you can set it as "Ethereum" or "USDT (erc20)".

**Deposit address**: This is the address where users will send their funds. It is recommended to create a separate address for each cryptocurrency.

**Token**: If enabled, users will need to send funds using the contract address.\
**Contract address**: If you are using a token as a method of receiving funds, you need to provide the contract address.\
**Token decimals**: Specify the number of decimal places for the token.\
**Burning coins**: This mode accounts for a double transfer in each user's transaction, with one transfer being burned.\
**Burning percentage**: In the burning coins mode, specify the percentage value to be burned. This percentage will also be deducted from the total deposit amount.

**Confirmations**: Set the number of confirmations in the network required for funds to be credited.

**Price**: Choose either *Manually* or *Automatically* for price updates.\
**Price value**: If you have selected *Manually* for price updates, enter the price in US dollars.\
**Price ID**: If you have selected *Automatically* for price updates, provide the identifier that will fetch the current value of the cryptocurrency price. For example, "tether".

**Maximum random value**: This value is used to create a unique payment amount. A random value between 0 and the specified maximum value will be added to the final payment amount. The default value is 999. For example, if a user wants to add 1 USDT to their balance, the system will generate a random number (e.g. 125) and create an account with a total amount of 1.000125 USDT (taking into account the *token decimals* for the currency). The additional amount is a small fee for creating a unique payment. A too large value will increase the payment amount, while a too low value may increase the time taken to create the payment.

**Symbol**: Specify the symbol for the cryptocurrency, e.g. ETH.

**Blockchain**: Select the appropriate blockchain from the list.

**Allow withdrawals**: By selecting this option, users will have the authority to conveniently initiate withdrawal requests through this method.\
**Withdrawal method name**: In this field, you can precisely indicate the name associated with the withdrawal method. This designated name will be prominently showcased in the cashier section as an accessible choice for users.

Once you've entered the necessary details, click the `Add` button to complete the process.

\
Managing your cryptocurrencies is made easy with our intuitive user interface. By clicking on the `List of cryptocurrencies` tab, you can view and sort your cryptocurrency list by various criteria, such as *Name* and *Cryptocurrency price*. Each cryptocurrency is accompanied by icons representing different actions.

To activate a payment method, simply click on the **Activate method** icon. Conversely, to deactivate a payment method, click on the **Deactivate method** icon. If you need to make any changes to the parameters of a specific cryptocurrency, click on the **Configure cryptocurrency** icon. And if, for any reason, you want to remove a cryptocurrency from your platform, click on the **Remove cryptocurrency** icon.

With Poker-Engine's integrated cryptocurrency support, you can enhance your website's payment capabilities, offering your users a seamless and secure experience.

### <a name="coupons"></a> Coupons

Our software offers an enhanced coupon support feature that greatly improves its functionality. With this feature, you can create and manage different types of coupons, such as USD or virtual chips. Coupons can also have expiration dates and can be automatically generated when creating custom [mailings](#mailing).

To access the coupon management section, go to `Cashier` > `Coupons`.

In the `Settings` tab, you have the option to enable or disable coupon support according to your preference.

\
To add a new coupon, click on the `Add` tab.

**Game coupon**: When adding a game coupon, enter the gaming coupon code (e.g., L99MQ).

**Currency**: Select the game currency that corresponds to this coupon.

**Nominal**: Set the nominal value for the gaming coupon. If the value includes decimal numbers, use a dot as the separator.

**Expires**: Specify the expiration date and time for the coupon, or leave the field blank if there is no expiration date.

Click the `Add` button to create the coupon.

\
To view the list of coupons, navigate to the `Coupons` tab.

You can use the search bar to quickly find specific coupons.

The list of coupons can be sorted by clicking on the column names. Sorting options include *Coupon*, *Nominal*, and *Redeemed* (showing who redeemed the coupon and when).

If needed, you can delete a coupon by clicking on the corresponding icon.

### <a name="transactions"></a> Transactions

To ensure accurate and reliable record-keeping of all online cashier transactions, our system diligently saves and documents every payment processed, including coupon redemptions and balance-related transactions. Accessing this vital information is easy; simply navigate to the `Cashier` > `Payments` section.

When reviewing the transactions, the *User* column offers a convenient way to click on a player's login and access a detailed user page containing essential user information. In the *Action* column, you will find specific details regarding each transaction, including whether it was a deposit, withdrawal, or internal transfer. Additionally, it will indicate the payment amount and the payment method utilized (cryptocurrency payment, credit card payment, or any other form of payment). The current status of the payment can also be viewed.

Moreover, the *Date* column presents the exact date and time when the payment was initiated, providing a clear understanding of the transaction timeline. With our comprehensive payment history feature, we guarantee transparency and accountability, as it meticulously tracks every financial transaction conducted by the online cashier.

### <a name="server"></a> Server Settings

To configure the server settings, navigate to the administrator panel and go to `Settings` > `Server`. These settings are initially set during software installation and can be modified in the configuration file located in the `Config` directory. However, it is advisable to make changes through the administrator panel and only edit the file as a last resort. Changing settings via the panel will automatically restart certain [processes](#processes), such as the *gameserver*, which is vital.

The **Site URL** parameter enables you to alter the domain if it has been changed or was previously unspecified. Ensure that you enter the correct value, as any mistake will necessitate manual editing of the configuration file.

**Script path** refers to the full path of the script folder. If the path is incorrect, manual editing of the configuration file and restarting all processes will be required.

The **Site e-mail** is used for receiving notifications and as the technical support address for users.

The **Site name** is the name displayed in the site pages' titles.

Select the appropriate time zone for the site under the **Time** section.

Once the necessary changes have been made, click `Save` to confirm them. Keep in mind that if the changes require restarting the game server, the saving process may take some time.

### <a name="general"></a> General Settings

To customize the external display of site features, avatars, and lobby background tune, navigate to the `Settings` > `General` section.

\
To customize avatars, go to the `Avatars` tab.

Here, you can choose whether to allow users to upload their own images from their computers as avatars. By default, this option is disabled. You can also choose which avatars are available for users to select from the default avatars set. Click on an avatar image to set it as the default avatar for new user registrations.

To upload a new avatar from your computer, click the *file selection box*. Hold down the "SHIFT" key to select multiple images, or press "CTRL" to select images individually. Image names must only contain Latin letters and numbers. Click the `Upload files` button.

Remember to click the `Save` button after making any changes.

\
To customize the lobby background tune, go to the `Melodies` tab. This tune plays on loop whenever a user accesses the lobby page.

Enable or disable the background melody as desired.

Select a tune from the provided list. There is a player on the right side for your convenience in previewing the tunes.

To upload a new tune from your computer, click on the *file selection area*. Hold down the "SHIFT" key to select multiple files, or press "CTRL" to select files individually. Please ensure that the melody name consists only of Latin letters and numbers.

After making any changes, save them by pressing the `Save` button.

\
To edit the display of other site features, click on the `Site` tab.

**Site description**: Enter a description of the site that will be visible to search engines.

**Keywords**: Enter phrases and words that users typically search for on search engines. These keywords are important for site promotion. Separate them with commas.

**Cashier**: Disable this feature if you want to make the online cashier unavailable to users.

**Play for money**: Disable this feature if you don't want cash tables for real money to be visible in the lobby.

**Tournaments**: Disable this feature if you don't want to create tournaments or have them visible in the lobby. Tournament tickets will also be hidden.

Click the `Save` button after making any changes.

### <a name="game"></a> Game Settings

The entire gameplay relies on specific parameters. To modify them, navigate to `Settings` > `Game`.

**IP Check**: Enabling this option prohibits players using the same IP address from playing at the same table.

**Move Time**: This is the duration within which a player must make their move. Otherwise, an automatic fold/check will occur. Time is specified in seconds.

**Player Timeout**: If a player fails to take any action within this time period, they will go into sitout mode. Time is specified in seconds.

**Showdown Timer**: During the announcement of winners, players will see all the cards of other players for a specified period of time. Time is specified in seconds.

**Timeout for Absent Players**: If a player is disconnected and does not return to the table within the specified time period, they will go into sitout mode. Time is specified in seconds.

**Sitout Timer**: This is the duration players spend on the exit page of the table. Time is specified in seconds. You can edit this page using the built-in [editor](#editor).

**Virtual Money Replenishment**: The number of virtual chips credited to a user's account each time they log in. This can only happen once every 24 hours. Use a decimal number with a dot as the separator. Set to 0 to disable this option.

**Rake**: The commission charged as a percentage on each winning. Set to 0 for no commission. Use a decimal number with a dot as the separator.

**Bot's Move**: The time it takes for a bot to make its move, specified in seconds. You can set two values separated by a comma to create a random duration within a range. For example, "2,7" will result in bot moves between 2 to 7 seconds.

**Play with Friends**: Specify who can create private tables. Options include "All Users", "Verified Users Only", or "Nobody"

**Chat**: Enable or disable the ability for players to send chat messages.

**Preflop Rake**: This function allows you to enable or disable rake after players fold preflop.

**Chips Symbol**: The symbol displayed before the numerical value of bets on the table. Leave empty for no symbol, use $ as the default.

**Tournament Currency Symbol**: The symbol displayed next to the numeric value when playing in tournaments. Leave empty for no symbol.

**Tournament Currency Chips Symbol**: The symbol displayed before the numerical value of bets on the table when playing in tournaments. Leave empty for no symbol.

Click the `Save` button to save your changes.

### <a name="templates"></a> Mailing List Settings

Navigate to `Settings` > `Email Templates` to manage your email templates and configure your email delivery preferences.

\
Access the `Settings` tab to adjust email delivery settings:

**SMTP Server Usage**: Choose 'Yes' to enable or 'No' to disable the use of an SMTP server for email dispatch.

**SMTP Server**: Input the address of your SMTP server.

**SMTP Port**: Enter the port number your SMTP server uses.

**SMTP Encryption**: Select the encryption method (SSL, TLS, or NONE) for your SMTP server.

**SMTP Authentication Required**: Choose 'Yes' if your SMTP server requires authentication, or 'No' if it does not.\
**SMTP Username**: Provide the username for SMTP server authentication.\
**SMTP Password**: Provide the password for SMTP server authentication.

**From Email Address**: Enter the email address that will be used as the sender, such as no-reply@example.com.

**From Name**: Enter the sender's name that recipients will see, such as "Poker Room Support."

**Fallback on Failure**: Toggle 'Yes' to enable or 'No' to disable fallback to a built-in mail function if SMTP delivery fails.

Remember to click the `Save` button to apply your new email settings.

\
To view and manage your email templates, select the `Templates` tab. Each template will have options to *Preview*, *Edit*, or *Delete*. Select *Preview* to review the template in a new tab.

\
To create a new email template, click the `Create Template` button.

**Template Subject Name**: Enter a name that will be used in the email's subject line.

**Filename**: Leave this field empty to have the filename generated automatically.

**Email Body Content**: Compose the text that will be sent to users. You may include HTML, language tags, and system variables.

Click on `List of System Variables` to view all available variables. Click on a variable to insert it directly into your email content. Press F11 on your keyboard to switch to full-screen mode while editing.

Don't forget to click the `Save` button to preserve your new template.

### <a name="addons"></a> Addons Management

To enhance the functionality of your Poker Room, navigate to `Settings` > `Addons`. Currently, only official addons provided by us can be uploaded due to security and compatibility reasons. Custom addons can be developed upon request.

**Installed Addons**: Lists all the currently installed addons. By default, a captcha addon is pre-installed for security during user registration.

**Captcha Settings**: To enable or disable the captcha feature, click the toggle switch next to the corresponding addon.

**Addon Requests**: If you require additional functionality, you can request custom addon development. Contact our support team for more details on this service.

**Managing Addons**: Each addon comes with a set of actions. You can view addon details, configure settings, or remove an addon if it is no longer needed.

Remember to review any changes made to addon configurations by clicking the `Save` button.

### <a name="languages"></a> Language Management

To cater to a global audience, manage your language settings by navigating to `Settings` > `Languages`. Here, you can add new languages or manage existing ones to customize the user experience for players from different regions.

\
**Adding a New Language**

Click on the `New` tab to upload a new language pack.

**Language Name**: Specify the language (e.g., Bulgarian).

**Language Code**: A brief identifier for the language (e.g., "bg").

**Language File**: Upload the corresponding language file. Ensure the filename corresponds with the language code (e.g., 'bg.php').

**Flag Icon**: Upload the country flag icon in png, gif, jpg, or jpeg format. The filename should match the language code (e.g., 'bg.png').

Click the `Add` button to include the new language in your Poker Room.

\
**Manage Existing Languages**

Use the `Add Text` button to insert new phrases into the language pack. In the modal, enter the translation text into the provided field. HTML tags are permitted. Choose `Confirm` to save or `Cancel` to discard changes. Upon confirmation, you will receive a phrase ID for use in the platform's content.

The `Languages` tab displays all available languages. On the right side of each language, there are icons representing possible actions.

**Activate/Deactivate**: Toggle a language's availability on the platform.

**Edit**: Modify translations within a language pack.
- To edit a phrase, simply click on it in the edit view. This action will display the phrase's unique ID, which can be utilized to reference the phrase throughout your content.
Use `Save Changes` to apply modifications or `Cancel` to revert.
Utilize the search functionality (Ctrl+F) in your browser to quickly locate specific phrases for editing.

**Remove**: Delete a language pack from the system.

### <a name="signup"></a> Registration Settings

To access and configure the signup settings, navigate to the `Settings` section and select `Registration`.

**Account Approval Method**:  This setting allows you to specify the method for approving new registered accounts, such as *Email Address Confirmation*, *Administrator Approval*, *Email Address Confirmation and Administrator Approval*, or *Not Required*.

**Email Address Requirement**: Enabling this option will prompt users to provide their email address during the registration process.

**Date of Birth Requirement**: Enabling this option will require users to provide their date of birth during registration.\
**Minimum Age for Registration**: Specify the minimum age in years, e.g., 18, to restrict registration to users above a certain age.

After making any changes, remember to click the `Save` button to apply the updated settings.

### <a name="navigation"></a> Navigation Settings

To manage the site navigation, navigate to `Settings` > `Navigation`.

The navigation menu consists of two sections, namely `Top of the site` and `Bottom of the site`. Both sections display a list of menu items that are sorted based on their position number. On the right side of each item, there are icons representing possible actions: *Activate/Deactivate* menu item, *Edit*, *Delete*, *Move Down*, and *Move Up*.

To add a new menu item, click on the `Add item` button available on each tab. This action will open a modal window where you can specify the parameters for the new item.

In the modal window, you can set the following parameters:

**Type**: Select the type of the menu item. You can choose between *Link* (a normal hyperlink) or *Code* (a stand-alone code, such as an image).

**Name**: Enter the name of the menu item or use a language variable.

**Link**: Provide the link to the desired page. For example, you can enter "mylink" to link to a specific page.

**Target**: Define the target behavior when the link is clicked. Options include opening the link in a new tab or performing the transition on the current tab.

**Parent**: Select the parent menu item, if applicable. The parent item will become an expandable list containing the selected sub-item.

**Code**: Use this field to insert any HTML tags or code, such as an image with a hyperlink to a banner.

**Access**: Set the accessibility of the menu item. You can choose between `guest` (accessible to guests), `user` (accessible to registered users), or `for all` (accessible to all users).

Once you have specified the desired parameters, click `Ok` to save the new menu item. If you decide not to add a new item, click `Cancel` to exit the modal window without making any changes.

### <a name="processes"></a> Server Process Management

To oversee server operations and review system logs, navigate to `Processes` > `Management`.

The game server orchestrates gameplay at the tables, organizes tournaments, and conducts various background tasks such as updating player statistics, synchronizing chat and hand histories, among others. In this section, you'll find information on the following:

**Server Status**: Displays the current status of the game server. You can see whether it's active or offline. While the server is offline, users will not be able to connect to the tables, and their browser client will automatically attempt to refresh the connection until the server becomes active again.

**Process ID (PID)**: Shows the unique identifier for the main server process.

**Server Control**:
  - **Start Server**: Boot up the game server to allow users to connect and play.
  - **Stop Server**: Gracefully shut down the server, ensuring all data is saved before going offline. During this time, players will not be able to establish new connections.
  - **Restart Server**: Perform a complete stop and restart of the server. This may be necessary for updates or troubleshooting.

\
**Log Management**

**Log Files List**: A directory of all system logs, each corresponding to a specific task or process. Logs can be sorted by `Log Name` or `Log Size` to facilitate easier management and review.

**View Log**: Inspect the detailed records within a log file to diagnose problems or perform audits.

**Clear Log**: Reset the log file to clear old entries and free up space.

**Log Storage**: Access the folder containing all log files by clicking on the underlined directory name.

\
By maintaining a well-managed server environment, you ensure a reliable and smooth experience for your users. Regular monitoring and management of these processes help prevent downtime and maintain the integrity of your online poker room software.

### <a name="configuration"></a> Server Configuration

Navigate to `Processes` > `Server Configuration` to tailor the game server settings to your needs. The game server is powered by OpenSwoole, which guarantees high performance and scalability for your online poker platform.

**Server IP Address**: Specify the IP address for the WebSocket server. The default value is `0.0.0.0`, which makes the server accessible on all network interfaces.

**Server Port**: Define the port number for the WebSocket server to listen to incoming connections.

**Connection Protocol**: Choose the communication protocol: `ws` for WebSocket or `wss` for WebSocket Secure. Note: Use `wss` if your site operates over HTTPS.\
**SSL Certificate File**: If using `wss`, upload or provide the path to the SSL certificate file. Ensure that the file and its directory have the appropriate permissions.\
**SSL Certificate Key File**: Similar to the certificate file, upload or specify the path to the SSL certificate key file, checking that permissions are set correctly.

**Maximum Number of Requests**: Define the threshold for the number of requests a connection can make before being reset. This serves as a protective measure against potential abuse and ensures fair resource distribution among users. For instance, setting this to `1000` means that after 1000 requests, the connection's request count will be reset.

**Connection Limit**: Determine the maximum number of concurrent connections the server can manage. Attempts to connect beyond this threshold will be denied, preserving server stability.

**Process Owner**: Specify the system user under which server processes will run. This helps in managing permissions and maintaining security.

**Process Group**: Designate the system group for server processes to further refine access control and process management.

Following these configurations, your game server will be optimized for security, performance, and reliability, providing an exceptional gaming experience for your players.

### <a name="editor"></a> Page Editor

The `Page Editor` is an essential tool for administrators to manage and customize the website's pages. This section provides robust features for editing page identifiers, content, and visibility settings, ensuring that the site maintains a professional appearance and user-friendly navigation.

The main features of the `Page Editor` are organized into a user-friendly table with the following columns:

**URL Slug** - Represents the unique address for each page, which is used in the website's URL (e.g., "support" for www.example.com/support).

**Description** - Provides a concise summary of the page's purpose or its content, aiding in quick identification and management.

**Visibility** - Specifies the audience for each page: whether it's available to all visitors (public), only to guests (non-registered users), or exclusively to registered users (private).

Next to each page entry, icons are available for quick actions:

**Toggle Visibility** - Enable or disable the page's visibility with a single click.

**Open in New Tab** - Preview the page as it would appear to the site's visitors.

**Edit** - Modify the page's content, style, or visibility settings.

**Delete** - Remove the page from the website.

\
Below the list of pages, there is a dedicated section for managing the site's aesthetics through CSS styles. This section presents a list of CSS styles, each accompanied by its style name and icons for edit and delete actions. This functionality allows for the modification of visual elements to enhance the user experience.

\
**Creating a New Page**

To add a new page to your site, click the `Create New Page` button and provide the details in the following fields:

**Entry Type**: Choose the kind of entry you are adding: *Web Page*, *Content Block*, or *CSS Style Sheet*.

If *Web Page*:\
**Page Identifier**: Assign a unique identifier that users will use to navigate to the page (e.g., "support").\
**Visibility Level**: Set the page's accessibility to public, guests only, or registered users only.

If *Content Block*:\
**Associated Page**: Specify the identifier of the related page for organizational purposes (e.g., "support").\
**Content Identifier**: Set a unique name that corresponds to the content block.

**Page Title**: Enter the title for your page or content block. You can utilize language variables for multilingual support.

**Content**: Insert the actual content for your page, which can include text, HTML markup, JavaScript code, etc. Use this to craft the desired look and feel for your new page.

For a more immersive editing experience, press F11 on your keyboard to switch to full-screen mode while editing. Ensure all changes are saved by clicking the `Save` button, or navigate back to the list of pages using the `Page List` button.

### <a name="messages"></a> Messages Center

The Messages Center is a hub for all communication-related activities within the admin panel of the online poker room software. It provides a comprehensive overview of all the incoming verification and withdrawal requests, as well as direct messages from the site's visitors through the feedback form.

\
**Navigating the Messages Center**

- **Inbox**: This section contains all incoming messages, verification requests, and withdrawal requests. Each type of message is marked with a distinct icon for easy identification.
- **Sent Items**: This area displays all messages that have been sent out by the admin. It is useful for tracking previous correspondences.
- **Compose**: Use this feature to create and send messages to individual users or multiple recipients.

\
**Managing Messages**

- **Sorting**: Messages can be organized by *Sender*, *Content*, *Category* (such as general messages, verification, or withdrawal requests), and *Date*. This enables easy retrieval of past correspondences.
- **User Information**: By clicking on the sender's name, you are directed to the [User Management](#users) section where you can view detailed information about the user.
- **Action Icons**: Each message is accompanied by icons that allow you to *View*, *Delete*, or *Select* the message for batch actions.
- **Batch Deletion**: Select multiple messages and click on the deletion icon at the top of the list to remove them all at once.

\
**Message Details**

- **General Messages**: When opening a general message, sender details are displayed, and you have the option to respond directly.
- **Verification Requests**: These messages come with attachments that can be reviewed before clicking on the `Verify` button or responding to the user's message.
- **Withdrawal Requests**: Details of the request and the chosen withdrawal method are shown. You can action the request by clicking `Approve`, `Deny`, or `Message User`. For Coinpayments methods, funds are transferred automatically upon approval. For other methods, marking the request as 'Paid' is a manual confirmation of transaction completion.

\
**Sending Messages**

- **Individual Messaging**: To send a message to a specific user, simply enter their username or email address.
- **Group Messaging**: For broader communication, specify multiple recipients by separating their identifiers with commas.

By utilizing the Messages Center effectively, administrators can ensure smooth and efficient communication with users, which is an essential aspect of managing an online poker room.

### <a name="updates"></a> Software Update Management

Managing updates is crucial to ensure that your online poker room software has the latest features, security patches, and performance improvements. The `Updates` section of the admin panel provides a comprehensive set of tools to help administrators maintain the software efficiently.

**Version Check and Update Indicator**\
When logging into the administrator panel, the version installed on your server is checked against the actual one. If they are different, the `Updates` button will flash orange, indicating that a new update is available. If the installed version is up to date, the button will stay green.

**File Integrity and Update Process**\
Even if the version of the installed software is up to date, you may still need to update accidentally changed or deleted files. To facilitate this, go to the `Updates` section and wait for the files to be checked.

**Caution Regarding Engine File Modifications**\
We do not recommend making any changes to the engine files. The update process only ignores the modified style files and those files that have been edited with the [Page Editor](#editor). For all other cases, after an update, you will have to manually check for differences. Free utilities can assist you with this; for example, WinMerge is a useful tool for Windows users.

**Disclaimer**\
Please note that we do not guarantee smooth operation when making changes to the engine files. In case of any problems, our support will be limited until the original files are restored.

**Checking for Updates**\
Upon accessing the `Updates` section, the system will automatically check for available updates. This process may take a few minutes, depending on the number of files that require scanning. A summary is presented with the following information:
- **Files to Update**: Number of existing files that have new versions available.
- **Files to Delete**: Number of outdated files that should be removed.
- **New Files**: Number of new files to be added.
- **New Tables**: Number of new database tables to be created.
- **Tables to Update**: Number of database tables that require updates.

You can click on `Details` to see a list of affected files or tables, including their names and paths.

**Backup and Changelog**\
Before applying any updates, it is recommended to create a backup of your current setup. You can do this by clicking on `Backup` next to the list of affected files. The backup will be stored in the `Backup` section for later retrieval.

Beneath the update summary, you will find the `Changelog`. This section provides detailed descriptions of the changes included in the latest version. Always clear your browser cache after an update to ensure that all changes take effect.

**Applying Updates**\
To initiate an update, simply click the `Update` button. If the update process requires a restart of the game server, be prepared for a brief downtime, typically lasting no more than one to two minutes. After the update is complete, verify that the game server is active in the [Process Management](#processes) section. If the server is not running, manually start it and review the log files for any issues.

**Backup Management**\
In the `Backup` submenu, administrators can manage their backups with the following options:
- **Create Backup**: To archive the current state of all software files.
- **Download**: To save a backup archive to your local machine.
- **Extract Files**: To restore files from a backup, replacing the current software folder contents.
- **Delete Backup**: To remove a backup file from the server.

**Note**
- Always create a backup before applying updates, especially if you have made custom modifications to the software.
- It is possible to preview new updates on our demo site before applying them to your live environment.

### <a name="panel"></a> Administrator Panel Configuration

Click on the profile icon in the upper right corner to access the Administrator Panel Configuration menu, where you can personalize the settings to improve your management experience and panel security.

#### Enhanced Security Verification
By enabling the `Enhanced Security Verification` feature, you will add an additional layer of protection to the admin panel. Each time you log in, you will be prompted to upload a pre-generated verification code from your computer. To generate a new code, switch the toggle to `On` and click `Generate Verification Code`. Follow this by clicking `Download Verification File`, which contains the code necessary for future logins.

#### Automatic Updates
The `Automatic Updates` feature streamlines the process of keeping your software up-to-date. When this is enabled, the system will automatically check for and download the latest updates upon logging into the panel. This ensures that you are always running the most current version of the software, with all the newest features and security enhancements.

#### Tooltip Display Preferences
With `Tooltip Display Preferences`, you have control over the display of helpful tooltips throughout the admin panel. Toggling this option off will disable pop-up tooltips that appear when you hover over informational icons (marked with a question mark). This can declutter the interface if you are already familiar with the panel's functionality.

#### Panel Configuration Options
- **Enhanced Security Verification**: Increase the security of your admin access with an additional verification step.
- **Automatic Updates**: Keep your software current with automated checks and downloads of new updates.
- **Tooltip Display Preferences**: Choose whether to display explanatory tooltips for a cleaner admin panel interface.

After adjusting these settings to your preference, be sure to click the `Save Changes` button to apply your changes. 

**Note**: It is highly recommended to preview new software updates on our demo site before applying them to your live environment. This allows you to familiarize yourself with the updates and ensure compatibility with your existing setup.

## <a name="user"></a> User

### <a name="user-profile"></a> User Profile Management

The User Profile section is your personal command center for managing your information and customizing your poker room experience. Here, you have the autonomy to adjust your settings and preferences, which empowers you with the ability to tailor your gaming environment to your liking.

For a comprehensive view of your performance, navigate to the `Profile` section on the main site. You'll find a detailed dashboard featuring your game statistics, including win rates, number of games played, and various other metrics that can help you refine your poker strategy.

#### <a name="user-details"></a> Personal Details

In the `Personal Details` tab, members have the ability to review and update their personal information, ensuring all details are up-to-date and accurate for a seamless online gaming experience.

To edit your information:

1. Navigate to the `Personal Details` tab within the `Profile` section.
2. Click on the `Edit` button to modify your details.
3. You can update your *First Name*, *Last Name*, *Phone Number*, *ZIP Code*, *Address*, *Country*, and *City*.
4. To ensure the security of your account, changes to sensitive information like email addresses are subject to email verification. Follow the link sent by our system to confirm any changes.
5. Note: Your login and date of birth are permanent and cannot be changed once set.

Rest assured, your personal information is held in the strictest confidence. It is not displayed to third parties and is solely used for account verification and administrative purposes.

Remember to click the `Save Changes` button after making any modifications to ensure your profile is updated accordingly.

#### <a name="user-password"></a> Password Management

For optimal security, we recommend our users to regularly update their passwords. Our platform provides an easy and secure process for password management.

To update your password:

1. Select the `Password` tab in your profile section.
2. Enter your current password in the provided field.
3. Input your new password into the `New Password` field and confirm it by entering it again in the `Confirm New Password` field.
4. Click on the `Save` button to apply the changes.

**Password Requirements:**
- Must be at least 8 characters in length.
- Should include a mix of upper and lower case letters.
- Incorporate at least one number and one special character for added security.

**Note:** Our system encrypts all passwords, ensuring that your information remains private and secure. Once your password is set, it is not visible to anyone, including our staff.

In case you have forgotten your password, simply click on the `Forgot Password` link when logging in and follow the instructions to reset it. A secure password reset link will be sent to your registered email address within a few minutes. Please check your spam folder if you do not see it in your inbox. Follow the link to create a new password and regain access to your account.

#### <a name="user-bonuses"></a> Bonuses

Stay engaged and get rewarded! Our platform appreciates your loyalty and offers a variety of bonuses to enhance your gaming experience. Navigate to the `Bonuses` tab in your account to explore the rewards available to you.

- **Bonus History**: Review a detailed log of bonuses credited to your account. Sort the list by *Bonus Name*, *Bonus Type* (such as Tournament Tickets, USD, Virtual Chips), *Amount*, and *Date of Crediting*. Keep track of your rewards and plan your next move.

- **Total Bonus Tally**: Easily view the sum of all bonuses credited to your account at a glance. This total reflects your accumulated rewards, giving you an insight into the value you've gained from playing with us.

- **Exclusive Offers**: Look out for exclusive bonus offers that pop up from time to time. These special promotions are designed to provide an extra boost to your gameplay.

**Creating Bonuses**: Bonuses can be created and managed by administrators in the [Bonuses](#admin-bonuses) section of the admin panel. Tailor-made bonuses can be crafted to suit various events, achievements, and player milestones.

Remember, the more you play, the more you earn! Bonuses are our way of saying 'thank you' for your continued patronage. Ensure your profile is up to date to be eligible for all rewards and check back often to not miss out on any offers.

#### <a name="user-affiliate"></a> Affiliate Program

Maximize your earnings through our Affiliate Program by inviting new players to our platform. Access your personalized referral links and track the growth of your affiliate network.

- **Affiliate Dashboard**: Navigate to the **Affiliate Program** tab to monitor your referrals. Analyze the enrollment history, manage your unique affiliate links, and view your earnings broken down by *User*, *Referral Level*, *Reward*, and *Time*.

- **Earnings Overview**: Get a comprehensive view of your total earnings from all referrals. Our intuitive table format allows for easy organization and review of your affiliate income.

- **Customizable Settings**: Tailor the Affiliate Program to your preferences by visiting the [Affiliate Program Settings](#affiliate) in the admin panel. Adjust your strategy and optimize your earning potential with our flexible configuration options.

Join the program today and start benefiting from your network's success!

#### <a name="user-agent"></a> Agent Dashboard

As an authorized agent within our online poker room software, you will have exclusive access to the `Agent Dashboard`. This comprehensive interface is designed to provide you with a detailed overview and management capabilities for all your assigned players.

- **Earnings Summary**: At a glance, view the total profit generated from all players under your purview, as well as your current agent account balance. This summary is crucial for keeping track of your financial performance and planning your strategy.

- **Player Analysis**: By selecting `Details` next to a player's login, you can access in-depth statistics for individual players. This section presents a neatly organized table displaying information such as the *Table ID*, *Rake* contributed, *Winnings*, and *Accrual Time*. This data helps you to understand your players' activities and their contribution to your earnings.

- **Fund Management**: The `Transfer Funds` option allows you to support your players by sending funds directly to their accounts. Clicking this will prompt a secure dialog where you can specify the transfer amount, which must not exceed your available agent balance. This feature facilitates financial assistance and incentives for your players, encouraging loyalty and sustained play.

- **Adjustable Agent Preferences**: Fine-tune your agent operations by visiting the [Agent Settings](#agent) section within the admin panel. This area allows you to set up the commission rates, payment intervals, and other essential aspects that influence your revenue from the associated players.

These tools are designed to empower you as an agent, providing you with the resources needed to manage your players effectively and to maximize your earnings through strategic oversight.

### <a name="user-settings"></a> User Settings

Enhance your gaming experience with personalized settings tailored to your preferences. Dive into the `Settings` section on the main site to customize your gaming environment, avatar, and account details.

#### Avatar

Personalize your profile with a custom avatar. Your selected image will represent you at the gaming tables and within the player community.
Here is an avatar selection box where you can manage your avatars, accessible through [General Settings](#general).
If avatar upload is enabled in [General Settings](#general), you can upload your own custom avatar to further personalize your profile.

#### Game Settings

Tailor your poker experience by configuring your preferred game settings, including keyboard shortcuts for in-game actions like fold, call, and raise. Click on the `Game settings` tab. Here, you can set up Hot keys for *Call*, *Raise*, *Fold*, *Check*. To customize these, simply click against the desired action to call the input handler. It will prompt you to press any key on the keyboard, displaying the key name against the action. Complete the setup by clicking on the `Change` or `Cancel` button.

#### Account Settings

Click on `Account settings` tab.

- **IP Binding**: Enable this option to restrict login sessions to the current IP address for enhanced security, preventing unauthorized access from different locations. Once enabled, authorization will only be possible from the current IP address.

- **Top Ranking Display**: Opt to show your username in the player ranking list. This feature is enabled by default.

- **Detailed Game Statistics**: Choose to display detailed statistics about your gameplay. This option is available only when the Top Ranking Display is turned on. It is enabled by default.

- **Email Notifications**: Receive email notifications for any changes in your account. This feature is enabled by default.

Remember to click the `Save changes` button after making any adjustments to ensure that your preferences are updated.

##  <a name="lobby"></a> Poker Lobby Overview

The Poker Lobby serves as the gateway to all the action, providing players with an intuitive and feature-rich environment to enjoy their online poker experience. Each feature is designed to provide players with control and flexibility, ensuring a seamless and enjoyable poker experience from the moment they enter the lobby. Here's a closer look at the key features available within the Poker Lobby:

#### Main Tabs

Upon entering the lobby, players are greeted with two prominent tabs:

- **Tables**: This tab presents a curated list of all available poker tables, allowing players to quickly find a game that suits their preferences and skill level.
- **Private Games**: Formerly known as "Play with Friends", this tab lets players set up private tables for an exclusive poker session with invited friends.

#### Table Listings

*Real-Time Updates*

The Lobby dynamically updates with real-time information, ensuring that the status of tables and tournaments is always current. Players will never miss out on joining a new game or tournament due to outdated information.

Browse the left section of the lobby to find a neatly organized display of active tables. Here, you'll see essential details like stakes, number of players, and game type at a glance. Use our intuitive filters and sorting options to quickly locate the perfect table that matches your skill level and interests.

Choose between `Cash Games` or `Tournaments` using the tabs provided. A handy search bar lets you pinpoint tables by name, and sorting by various parameters means you're always just a click away from your preferred game. For administrators, disabling tournament participation in [General Settings](#general) will hide the Tournaments tab, streamlining the experience for your users.

To enhance user navigation and provide detailed insights, a dedicated section is situated on the right side of the screen. This area includes options such as `Play for Money` and `Play for Fun` (using Virtual Chips). By selecting either of these options, the table listings will be refreshed to align with your choice of play mode.

If you've recently competed in a tournament, you'll find a convenient link to the last tournament's results. Your balance is displayed prominently – real money players can track deposits and withdrawals, while fun players can monitor their virtual chip tally. Hover over your balance for a tooltip that reveals the bonus chips credited at login.

Beneath your balance, the `Tournament Tickets` section awaits. Click through to a modal window detailing your tournament ticket history and the current total. These tickets are your key to registering for upcoming tournaments or to join freerolls designated for ticket holders.

Selecting a table brings up information about occupied seats alongside a `Sit at the Table` button, inviting you to join the game. For tournaments, `Registration` and `More` buttons provide quick access to essential tournament details. Register with a click, or delve deeper into the tournament's specifics and see who else is in the running.

#### Cashier

Adjacent to the balance and tournament tickets, players will find a prominent `Cashier` button. One click unveils the cashier modal window, where players can perform a variety of financial transactions across different tabs, including *Deposit*, *Withdrawal*, *Transfer*, and *Transaction history*. Additionally, players can access the *Verification* tab for account security and compliance purposes. The time of the last visit to the cashier is also displayed for convenience. Notably, to maintain a high level of security, only one cashier window can be opened at a time.

The system is intuitive, automatically calculating the total amount to be credited or transferred to a player's account when they enter a deposit or withdrawal figure, factoring in all associated fees. The `Transfer` tab enables players to make internal transfers to other player accounts, provided their own account has this functionality. All account transactions are meticulously recorded under the `Transaction history` tab, sortable by *Information*, *Amount*, *Residue* (Balance after), *Status*, and *Date*.

For those who have completed the verification process, the verification tab becomes unavailable, ensuring a streamlined experience for verified users.

#### Inclusive Features: Play with Friends

*Create a New Game*

We've introduced the ability for players to host private tables, fostering a more personalized and exclusive gaming atmosphere. To create a private table, players simply provide a *Game name*, *Password*, specify the *Buy-in*, the *Maximum buy-in*, and select the *Number of seats* (options include 9, 6, 4, 2). Upon clicking the `Create` button, a confirmation message will appear, affirming the successful creation of the table. Players can then extend invitations to friends to join in on the private game.

*Join a Game*

Accessing a private table is straightforward. Players need only enter the *Game name* and *Password* before clicking the `Join` button to be part of the exclusive gameplay experience.

#### Real-Time Server Clock

We've strategically placed a real-time server clock beneath the bottom navigation bar to assist players in managing their play sessions and coordinating tournament participation.

\
We are committed to providing an unparalleled online poker experience, and these Lobby enhancements are just the beginning. Stay tuned for more updates as we continue to refine and improve our software.
