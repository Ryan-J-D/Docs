# Mailbox hooks

## CanUseMailbox

``` csharp
void CanUseMailbox(BasePlayer player, Mailbox mailbox)
{
    Puts("CanUseMailbox works!");
}
```

 * Called when a player tries to use a mailbox
 * Returning true or false overrides default behavior