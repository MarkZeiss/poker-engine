# Poker-Engine v3 documentation
This documentation is the official documentation for Poker-Engine v3

*English version*

This comprehensive documentation provides detailed information on all the customization options available in the poker-engine v3 software. The software can be found directly at [poker-engine.com](https://poker-engine.com), and a demo version is also available at [demo.poker-engine.com](https://demo.poker-engine.com).

The different categories under which the customizations are organized include:

1. [Admin Panel](#admin-panel):

- [Tables](#tables): Configure and manage poker tables.
- [Tournaments](#tournaments): Set up and run poker tournaments.
- [Styles](#styles): Customize the visual appearance of the software.
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
**Renewal period**: Choose one of the available values, such as Every day, to create the tournament at the same time each day.\
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


### <a name="styles"></a> Styles



### <a name="users"></a> User Management



### <a name="groups"></a> Groups



### <a name="bonuses"></a> Bonuses



### <a name="affiliate"></a> Affiliate Program



### <a name="mailing"></a> Mailing Lists



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
