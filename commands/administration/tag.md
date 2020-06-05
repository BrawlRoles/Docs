{% hint style="success" %}
Permissions:

Bot permission: `ADMINISTRATION`<br>User permission: `BAN_MEMBERS`
{% endhint %}

##Description

With this command you can set, reset or get a Usertag of a server member. You can also find the user, the tag is saved to with the option find.

##Usage

`-tag <option> [member / tag] [tag]`

| option | Description | Usage |
| :--- | :--- | :--- |
| find | Find a  |
| set| set, get remove the role from the database |
| role | The role the member gets (removed) for solo, duo, 3vs3 wins, the highest trophies or just when the verification was successful. |
| add/remove | Wheter the role should be added or removed from the member |
| solo / duo / 3vs3 / verified / highestTrophies |  |
|  |  |

| Argument | Description |
| :--- | :--- | 
| tag | Command name. |
| set/reset/find/get | set, get remove the role from the database |
| role | The role the member gets (removed) for solo, duo, 3vs3 wins, the highest trophies or just when the verification was successful. |
| add/remove | Wheter the role should be added or removed from the member |
| solo / duo / 3vs3 / verified / highestTrophies |  |
|  |  |


{% hint style="danger" %}
The user argument must be one word, the member id, the mentioned member or you can search for it when there are multiple members with the argument you have inserted.
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

We have the Brawl Stars Profile with the tag `#YU9G98V8` as shown in the picture above. We also have the role `@Dach_Legend` on the Discord server. If we want to give the role `@DACH_Legend` to every player which has more than 15.000 Trophies as his personal best, when the member verifies himself, we have to enter the following command.

```
-role add @Dach_Legend add highestTrophies 15000
```

If the player must have more than 1000 3vs3 victories to get the role `@+15k ⚔`, we enter the following command.

```
-role add @+15k ⚔ add 3vs3 15000
```

if we want the player to get the role `@Verified` as soon as he verifies himself, with no other conditions, we enter the following command.

```
-role add @Verified add verified
```

When we want to remove the role `@Dach_Legend` from the database we have to enter the following command.

```
-role remove @Dach_Legend
```