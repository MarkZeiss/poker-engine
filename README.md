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
- [Bonuses](#bonuses): Set up promotional bonuses for users.
- [Affiliate Program](#affiliate): Implement an affiliate marketing program.
- [Mailing Lists](#mailing): Manage email communication with users.
- [Agency Program](#agent): Create and manage agent accounts.
- [Cashier Settings](#cashier): Configure payment and withdrawal options.
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

2. [User Profile](#user-profile):

- [Personal Information](#profile): Update and manage user profile details.
- [Password](#password): Change and reset user passwords.
- [Bonuses](#user-bonuses): View and redeem available bonuses.
- [Affiliate Program](#user-affiliate): Access and manage affiliate program details.
- [Agent Program](#user-agent): View and track agent program information.
- [Avatar](#avatar): Customize user profile avatars.
- [Game Settings](#user-game): Adjust user-specific game settings.
- [Account Settings](#user-settings): Manage general account settings.

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

### <a name="bonuses"></a> Bonuses

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



### <a name="cashier"></a> Cashier Settings



### <a name="payment"></a> Payment Systems



### <a name="cryptocurrencies"></a> Cryptocurrencies



### <a name="coupons"></a> Coupons



### <a name="transactions"></a> Transactions



### <a name="server"></a> Server Settings



### <a name="general"></a> General Settings



### <a name="game"></a> Game Settings



### <a name="templates"></a> Mailing List Settings



### <a name="addons"></a> Addons



### <a name="languages"></a> Language Settings



### <a name="signup"></a> Registration Settings



### <a name="navigation"></a> Navigation Settings



### <a name="processes"></a> Process Management



### <a name="configuration"></a> Configuration



### <a name="editor"></a> Page Editor



### <a name="messages"></a> Messages



### <a name="updates"></a> Updates



### <a name="panel"></a> Admin Panel Settings



## <a name="user-profile"></a> User Profile



### <a name="profile"></a> Personal Information



### <a name="password"></a> Password



### <a name="user-bonuses"></a> Bonuses



### <a name="user-affiliate"></a> Affiliate Program



### <a name="user-agent"></a> Agent Program



### <a name="avatar"></a> Avatar



### <a name="user-game"></a> Game Settings



### <a name="user-settings"></a> Account Settings



##  <a name="lobby"></a> Lobby
