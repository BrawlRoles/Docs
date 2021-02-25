{% hint style="success" %}
Permissions:

Bot permission: `SEND MESSAGES`, `EMBED LINKS`<br>User permission: `ADMINISTRATION`
{% endhint %}

##Description

With this command we can save a success in Brawl Stars in our database. Available successes can be `solo`, `duo`, `3vs3`, `verified`, `highestTrophies`.

##Usage

`-role <add / remove> <role> [add / remove] [solo / duo / 3vs3 / verified / highestTrophies] [wins / highestTrophies]`

| Argument | Description |
| :--- | :--- | 
| role | Command name. |
| add/remove | Add or remove the role from the database. |
| role | The role the member gets (removed) for solo, duo, 3vs3 wins, the highest trophies or just when the verification was successful. |
| add/remove | Wheter the role should be added or removed from the member. |
| solo / duo / 3vs3 / verified / highestTrophies | The event in which the player must have an amount of wins, the highest trophies or the role gets added/removed upon verification. |
| wins / highestTrophies | The amount of wins, or the highest trophies is needed to get the Role. |

{% hint style="info" %}
When a player has 110 solo wins, and we've saved a verification role for 50, 100 and 150 solo wins. The member will only get one role. In our case the 100 solo wins role.
{% endhint %}

{% hint style="danger" %}
The role argument must be one word, the role id, the mentioned role or we can search for it when there are multiple roles with the argument we've inserted.
{% endhint %}

##How to actually use it

![](../../assets/knirpsii_profile.png)

We already set a role in the `verification` command that will be added to verified members. When we want to add another role to verified members, we can use the command like shown below.

```
-role add @BS_Player add verified
```
If we want to remove a role when the member verifies himself we use this command.

```
-role add @Not_Verified remove verified
```
We have the Brawl Stars profile with the tag `#YU9G98V8` as shown in the picture above. We also have the role `@Dach_Legend` on the Discord server. If we want to give the role `@DACH_Legend` to every player which has more than 15.000 Trophies as his personal best, when the member verifies himself, we have to enter the following command.

```
-role add @Dach_Legend add highestTrophies 15000
```
If the player must have more than 1000 3vs3 victories to get the role `@+15k ⚔`, we enter the following command.

```
-role add @+15k ⚔ add 3vs3 15000
```
If we want the player to get the role `@Verified` as soon as he verifies himself, with no other conditions, we enter the following command.

```
-role add @Verified add verified
```
When we want to remove the role `@Dach_Legend` from the database we have to enter the following command.

```
-role remove @Dach_Legend
```