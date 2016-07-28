# DatabaseMaker
A Minecraft plugin for Craftbukkit 1.9

##Description :
This complex plugin lets you create some databases, in game GUI, and use the Bukkit API's listeners to create your database with true permissions, with a single configuration file <name>.yml foundable with the config files of the plugin, in the folder "databases".

##Commands :
* /dbm or /databasemaker : Prints the help \n
* /dbm help : Prints the help.
* /dbm create <database> : Create a database, you need to set up the database before using it. If the server is stopped, the database will not be saved until you use /dbm <database> config save
* /dbm remove <database> : Removes a database, please note that you need the right permission to do this : databasemaker.<database>.conf, or databasemaker.*
* /dbm list : List all databases.
* /dbm <database> : Send information about a database.
* /dbm <database> add <item> <arguments> : Add an item.
* /dbm <database> edit <item> <arguments> : Edit an item.
* /dbm <database> remove <item> : Removes an item.
* /dbm <database> <item> : Print information about the item.
* /dbm <database> config : A complex command :
  * help : Print the help message of /dbm config.
  * value <type_of_value> <name> [type_of_value] [name] : Use this configuration args to set up what you want in your database. You can set   until 10 differents arguments for a database. Please note that if you use a "\" before your type of value, the value will not be       mandatory. If u use a "*" instead of the type of value, you will be able to use any type of value. For the differents types of         values,   see at the end of this README.
  * max <int Nb_of_max_items> : puts a limit for the database length. (Numbers of items). If you put 0, the database will not have a limit.
  * autoload <true/false> : Will the database automatically load with the plugin ? (Default value : "false")
  * save : Saves the database and the config. If you created a database without setting up values, type of values and max, you will not be   able to save the database, and the database will be deleted if the servers reloads the plugin (Server reboot included).
* /dbm load <database> : When you create and save a database, you need to load it. If the autoload value is false, you need to load your database when the server starts or reloads.
* /dbm unload <database> : Unload a database. (WARN : You will not be able to use your database).

## Permissions :
* databasemaker.* : All permissions in one.
* databasemaker.create : Create a database
* databasemaker.remove : Remove a database
* databasemaker.load : Load a database
* databasemaker.unload : Unload a database
* databasemaker.config : Set configuration of any database.
* databasemaker.<database>.config : Set configuration of one database.
* databasemaker.<database>.see : Use the database
* databasemaker.<database>.add : Add an item
* databasemaker.<database>.edit : Edit an item
* databasemaker.<database>.remove : Remove an item
* databasemaker.<database>.load : Load the database
* databasemaker.<database>.unload : Unload the database


## Incoming updates : 
* v1.1 : You will be able to create a GUI for a database :)
* v1.2 : With the token "$<database>.<item>", you will be able to use a database value in your commands (Like an argument).
** Tips : The database needs to have only one type of value : String <name>. Then it could be used like args.
* v1.3 : You will be able to use commands with your database (Create a GUI, which send commands when you click on an item :) )

