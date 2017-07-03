# Weapon Hooks

## OnCreateWorldProjectile

``` csharp
void OnCreateWorldProjectile(HitInfo info, Item item)
{
    Puts("OnCreateWorldProjectile works!");
}
```

 * Called when a projectile is created
 * Returning a non-null value overrides default behavior

## OnExplosiveDropped

``` csharp
void OnExplosiveDropped(BasePlayer player, BaseEntity entity)
{
    Puts("OnExplosiveDropped works!");
}
```

 * Called when the player drops an explosive item (C4, grenade, ...)
 * No return behavior

## OnExplosiveThrown

``` csharp
void OnExplosiveThrown(BasePlayer player, BaseEntity entity)
{
    Puts("OnExplosiveThrown works!");
}
```

 * Called when the player throws an explosive item (C4, grenade, ...)
 * No return behavior

## OnMeleeThrown

``` csharp
void OnMeleeThrown(BasePlayer player, Item item)
{
    Puts("OnMeleeThrown works!");
}
```

 * Called when the player throws a melee item (axe, rock, ...)
 * No return behavior

## OnRocketLaunched

``` csharp
void OnRocketLaunched(BasePlayer player, BaseEntity entity)
{
    Puts("OnRocketLaunched works!");
}
```

 * Called when the player launches a rocket
 * No return behavior

## OnWeaponFired

``` csharp
void OnWeaponFired(BaseProjectile projectile, BasePlayer player, ItemModProjectile mod, ProtoBuf.ProjectileShoot projectiles)
{
    Puts("OnWeaponFired works!");
}
```

 * Called when the player fires a weapon
 * No return behavior

## OnReloadMagazine

``` csharp
void OnReloadMagazine(BaseProjectile projectile, BasePlayer player, ItemModProjectile mod, ProtoBuf.ProjectileShoot projectiles)
{
    Puts("OnReloadMagazine works!");
}
```

 * Called when the player reloads a magazine
 * Returning a non-null value overrides default behavior
 
## OnReloadWeapon

``` csharp
void OnReloadWeapon(BaseProjectile projectile, BasePlayer player, ItemModProjectile mod, ProtoBuf.ProjectileShoot projectiles)
{
    Puts("OnReloadWeapon works!");
}
```

 * Called when the player reloads a weapon
 * Returning a non-null value overrides default behavior