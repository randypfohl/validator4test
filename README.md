# validator4test
Class used to define, manage and log validation of objects during automated test execution.

<b>concrete constructor</b>
<p>
For validation of non-primitive types, add child validators in the constructor using addChildValidator().  Child validators must including "this" as the parent validator in the arguments to ensure proper indentation management for logging and reporting.
</p>
<b>executeVerifications()</b>
 - Use verify() methods to include verification of primitive data types only (e.g. String, Boolean, Integer).
 - Use the addKnownIssue() to include notes about known bugs or other issues causing validation failures.

The mock AnObjectValidator includes a rough example of these.
