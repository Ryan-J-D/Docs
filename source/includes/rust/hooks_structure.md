# Structure Hooks

## CanAssignBed

``` csharp
void CanAssignBed(SleepingBag bag, BasePlayer player, ulong targetPlayerId)
{
    Puts("CanAssignBed works!");
}
```

 * Called when a player attempts to assign a bed or sleepingbag to another player
 * Returning a non-null value overrides default behavior

## CanBuild

``` csharp
void CanBuild(Planner planner, Construction prefab, Vector3 position)
{
    Puts("CanBuild works!");
}
```

 * Called when the player tries to build something
 * Returning a non-null value overrides default behavior

## CanChangeCode

``` csharp
void CanChangeCode(CodeLock codeLock, BasePlayer player, string newCode, bool isGuestCode)
{
    Puts("CanChangeCode works!");
}
```

 * Called when a player tries to change the code on a codelock
 * Returning a non-null value overrides default behavior

## CanPickupLock

``` csharp
void CanPickupLock(BasePlayer player, BaseLock lock)
{
    Puts("CanPickupLock works!");
}
```

 * Called when a player attempts to pickup a lock
 * Returning true or false overrides default behavior
 

## CanHideStash

``` csharp
void CanHideStash(StashContainer stash, BasePlayer player)
{
    Puts("CanHideStash works!");
}
```

 * Called when a player tries to hide a stash
 * Returning a non-null value overrides default behavior

## CanLock

``` csharp
void CanLock(BaseLock baseLock, BasePlayer player)
{
    Puts("CanLock works!");
}
```

 * Called when the player tries to lock a keylock or codelock
 * Returning a non-null value overrides default behavior

## CanSeeStash

``` csharp
void CanSeeStash(StashContainer stash, BasePlayer player)
{
    Puts("CanSeeStash works!");
}
```

 * Called when a player is looking at a hidden stash
 * Returning a non-null value overrides default behavior

## CanSetBedPublic

``` csharp
void CanSetBedPublic(SleepingBag bed, BasePlayer player)
{
    Puts("CanSetBedPublic works!");
}
```

 * Called when a player tries to set a bed public
 * Returning a non-null value overrides default behavior

## CanUnlock

``` csharp
void CanUnlock(BaseLock baseLock, BasePlayer player)
{
    Puts("CanUnlock works!");
}
```

 * Called when the player tries to unlock a keylock or codelock
 * Returning a non-null value overrides default behavior

## CanUseLockedEntity

``` csharp
void CanUseLockedEntity(BasePlayer player, BaseLock baseLock)
{
    Puts("CanUseLockedEntity works!");
}
```

 * Called when the player tries to use an entity that is locked
 * Returning true or false overrides default behavior

## OnCodeEntered

``` csharp
void OnCodeEntered(CodeLock codeLock, BasePlayer player, string code)
{
    Puts("OnCodeEntered works!");
}
```

 * Called when the player has entered a code in a codelock
 * Returning a non-null value overrides default behavior

## OnCupboardAuthorize

``` csharp
void OnCupboardAuthorize(BuildingPrivlidge privilege, BasePlayer player)
{
    Puts("OnCupboardAuthorize works!");
}
```

 * Called when a cupboard attempts to authorize a player
 * Returning a non-null value overrides default behavior

## OnCupboardClearList

``` csharp
void OnCupboardClearList(BuildingPrivlidge privilege, BasePlayer player)
{
    Puts("OnCupboardClearList works!");
}
```

 * Called when an attempt is made to clear a cupboard authorized list
 * Returning a non-null value overrides default behavior

## OnCupboardDeauthorize

``` csharp
void OnCupboardDeauthorize(BuildingPrivlidge privilege, BasePlayer player)
{
    Puts("OnCupboardDeauthorize works!");
}
```

 * Called when a cupboard attempts to deauthorize a player
 * Returning a non-null value overrides default behavior

## OnDoorClosed

``` csharp
void OnDoorClosed(Door door, BasePlayer player)
{
    Puts("OnDoorClosed works!");
}
```

 * Called when the player closed a door
 * No return behavior

## OnDoorOpened

``` csharp
void OnDoorOpened(Door door, BasePlayer player)
{
    Puts("OnDoorOpened works!");
}
```

 * Called when the player opened a door
 * No return behavior

## OnEntityBuilt

``` csharp
void OnEntityBuilt(Planner plan, GameObject go)
{
    Puts("OnEntityBuilt works!");
}
```

 * Called when any structure is built (walls, ceilings, stairs, etc.)
 * No return behavior

## OnHammerHit

``` csharp
void OnHammerHit(BasePlayer player, HitInfo info)
{
    Puts("OnHammerHit works!");
}
```

 * Called when the player has hit something with a hammer
 * No return behavior

## OnStructureDemolish

``` csharp
void OnStructureDemolish(BaseCombatEntity entity, BasePlayer player)
{
    Puts("OnStructureDemolish works!");
}
```

 * Called when the player selects DemolishImmediate from the BuildingBlock or BaseCombatEntity menu
 * Returning a non-null value overrides default behavior

## OnStructureRepair

``` csharp
void OnStructureRepair(BaseCombatEntity entity, BasePlayer player)
{
    Puts("OnStructureRepair works!");
}
```

 * Called when the player repairs a BuildingBlock or BaseCombatEntity
 * No return behavior

## OnStructureRotate

``` csharp
void OnStructureRotate(BaseCombatEntity entity, BasePlayer player)
{
    Puts("OnStructureRotate works!");
}
```

 * Called when the player rotates a BuildingBlock or BaseCombatEntity
 * No return behavior

## OnStructureUpgrade

``` csharp
void OnStructureUpgrade(BaseCombatEntity entity, BasePlayer player, BuildingGrade.Enum grade)
{
    Puts("OnStructureUpgrade works!");
}
```

 * Called when the player upgrades the grade of a BuildingBlock or BaseCombatEntity
 * Returning a non-null value overrides default behavior

## CanAffordUpgrade

``` csharp
void CanAffordUpgrade(BasePlayer player, BuildingBlock block, BuildingGrade.Enum grade)
{
    Puts("CanAffordUpgrade works!");
}
```

 * Called when the resources for an upgrade are checked
 * Returning true or false overrides default behavior
 
## CanChangeGrade

``` csharp
void CanChangeGrade(BasePlayer player, BuildingBlock block, BuildingGrade.Enum grade)
{
    Puts("CanChangeGrade works!");
}
```

 * Called when a player tries to change a building grade
 * Returning true or false overrides default behavior
 
## CanDemolish

``` csharp
void CanDemolish(BasePlayer player, BuildingBlock block, BuildingGrade.Enum grade)
{
    Puts("CanDemolish works!");
}
```

 * Called when a player tries to demolish a building block
 * Returning true or false overrides default behavior