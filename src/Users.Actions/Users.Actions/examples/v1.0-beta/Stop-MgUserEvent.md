### Example 1: Using the Stop-MgUserEvent Cmdlet
```powershell
Import-Module Microsoft.Graph.Users.Actions
$params = @{
	Comment = "Cancelling for this week due to all hands"
}
# A UPN can also be used as -UserId.
Stop-MgUserEvent -UserId $userId -EventId $eventId -BodyParameter $params
```
This example shows how to use the Stop-MgUserEvent Cmdlet.
To learn about permissions for this resource, see the [permissions reference](/graph/permissions-reference).
