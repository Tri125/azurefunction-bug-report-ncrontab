# azurefunction-bug-report-ncrontab

Minimal repro case for an issue found on Microsoft.NET.Sdk.Functions 3.0.7

Run the function and call the endpoint to execute ``http://localhost:7071/api/Function1``

You will get the following error:

``
System.Private.CoreLib: Exception while executing function: Function1. ClassLibrary1: Could not load file or assembly 'NCrontab, Version=3.3.1.0, Culture=neutral, PublicKeyToken=null'. The system cannot find the file specified.
``

There is no problem on Microsoft.NET.Sdk.Functions 3.0.3.
