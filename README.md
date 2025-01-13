# ACG Utilities for IBM Planning Analytics

# ACG Model Documenter.exe
* When attached to an IBM Planning Analytics model, this utility will output a Microsoft Excel document detailing all assets with the model.
# ACG Model Cleaner
(Source Code): https://github.com/ACG-Code/ACGModelClean
* This utility is used to remove unwanted assets (e.g., Cubes, Dimensions, Views, etc.) from an IBM Planning Analytics model.
# ACG-KillTransactionLogger.exe
(Source Code): https://github.com/ACG-Code/ACG_GetTransactions
* This application is used to stop the ACG_GetTransactions tool in cases where the log files
have become too large to index.  In cases where the numerous log files exist, or cube logging
has been left on during data loads, the transaction log retrieval can run for long periods of time.  This tool can interrupt the log retrieval to allow for clean up activities.
# ACG_GetTransactions.exe 
(Source Code): https://github.com/ACG-Code/ACG_GetTransactions
* This utility will retrieve recent transaction logs and store in a cube within the IBM PA model.  Along with our TurboIntegrator processes, this tool is used to keep track of value changes over time.
# ACG-SecretsManager.exe
(Source Code): https://github.com/ACG-Code/ACG_SecretsManager
* The ACG Secrets Manager utility is used to maintain a local database or "secrets" entries.  For REST API interaction or tasks which require a username and password, this tool can be used to maintain an encrypted database of those entries.
# PyPromote.exe
(Source Code): https://github.com/ACG-Code/PyPromote
* The  PyPromote utility allows IBM Planning Analytics administrators to deploy asset between model without the need for a model restart.   When deploying updated objects to other environments (e.g. Dev, Test, Prod, etc.), administrators have historically needed to bring down the target instance, copy files, and restart the model.  This is a time-consuming practice that can be difficult to track.  With PyPromote, all deployments are tracked in a cube within the model.
# TM1Backup.exe
(Source Code): https://github.com/ACG-Code/TM1Backup 
* The ACG TM1Backup tool is used to create backup copies of the IBM PA "data" directory.  This tool allows the IBM PA Administrator to specify a number of backup files to maintain as well as specify the number of logs files to maintain.
  * Usage `TM1Backup.exe <servername> <source path> <destination path> <logs directory> [options] `
   * Options: 
      * `-k <number>` - Number of backup files to keep
      * `-l <number>` - Number of log files to keep
      * `-f` - Backup feeder files
      * `-z` - Use ZIP format instead of 7zip
      * `-h` - Show Help Screen
      * `-v` - Show Version Information
# FindIt.exe
(Source Code): https://github.com/ACG-Code/FindIt
* Search Data directory for files containing string
* Searches *.pro, *.rux, and *.sub
* FindIt.exe <string\> <data_directory\> <output path and filename\>