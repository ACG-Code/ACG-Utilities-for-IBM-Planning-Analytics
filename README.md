# ACG Utilities for IBM Planning Analytics

# ACG model Documenter.exe
* When attached to an IBM Planning Analytics model, this utility will output a Microsoft Excel document detailing all assets with the model.
# ACG-KillTransactionLogger.exe
* This application is used to stop the ACG_GetTransactions tool in cases where the log files
have become too large to index.  In cases where the numerous log files exist, or cube logging
has been left on during data loads, the transaction log retrieval can run for long periods of time.  This tool can interrupt the log retrieval to allow for clean up activities.
# ACG-SecretsManager.exe
* The ACG Secrets Manager utility is used to maintain a local database or "secrets" entries.  For REST API interaction or tasks which require a username and password, this tool can be used to maintain an encrypted database of those entries.
# ACG_GetTransactions.exe 
* This utility will retrieve recent transaction logs and store in a cube within the IBM PA model.  Along with our TurboIntegrator processes, this tool is used to keep track of value changes over time.
# PyPromote.exe
* The  PyPromote utility allows IBM Planning Analytics administrators to deploy asset between model without the need for a model restart.   When deploying updated objects to other environments (e.g. Dev, Test, Prod, etc.), administrators have historically needed to bring down the target instance, copy files, and restart the model.  This is a time-consuming practice that can be difficult to track.  With PyPromote, all deployments are tracked in a cube within the model.
# TM1Backup.exe
* The ACG TM1Backup tool is used to create backup copies of the IBM PA "data" directory.  This tool allows the IBM PA Administrator to specify a number of backup files to maintain as well as specify the number of logs files to maintain.
# FindIt.exe
* Search Data directory for files containing string
* Searches *.pro, *.rux, and *.sub
* FindIt.exe <string\> <data_directory\> <output path and filename\>