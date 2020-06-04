{% hint style="success" %}
Permissions:

Bot permission: `ADMINISTRATION`<br>User permission: `ADMINISTRATION`
{% endhint %}

##Description

With this command you can set a channel in your Discord Server where Brawl-Roles is logging everything into about the verification save a success in Brawl Stars in our database. Availiable successes can be ``3vs3``, ``duo``

##Usage

-role <add / remove> <role> <add / remove> <solo / duo / 3vs3 / verified / highestTrophies> [wins / highestTrophies]

- Command name
- Add or remove it from the database
- The role the member gets
- If the role should be added or removed
- the event type he must have an amount of wins or the role gets added/removed upon verification
- the amount of wins or highestTrophies is needed to get the Role

{% hint style="danger" %}
The role argument must be one word, the role id, the mentioned role or you can search for it when there are multiple roles with the argument you have inserted.
{% endhint %}

##How to actually use it

![](../../assets/knirpsii_profile.png)

We have the Brawl Stars Profile with the tag `#YU9G98V8` as shown in the picture above. We also have the role `@Dach Legend` on the Discord server. If we want to give the role `@DACH Legend` to every player which has more than 15.000 Trophies as his personal best, when the member verifies himself, we have to enter the following command.

```
-role add @Dach Legend add highestTrophies 15000
```

If the player must have more than 1000 3vs3 Victories to get the role `@Dach Legend`, we enter the following command.

```
-role add @Dach Legend add 3vs3 15000
```

If we want the bot to remove the role `@Dach Legend` from the player if he has more than 400 Solo Victories, we enter the following command.

```
-role add @Dach Legend remove solo 400
```

if we want the player to get the role `@Dach Legend` as soon as he verifies himself, with no other conditions, we enter the following command.

```
-role add @Dach Legend add verified
```

When we want to remove the role `@Dach Legend` we have to enter the following command.

```
-role remove @Dach Legend
```