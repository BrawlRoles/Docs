{% hint style="success" %}
Permissions:

Bot permission: `SEND MESSAGES`, `EMBED LINKS`<br>User permission: `ADMINISTRATION`
{% endhint %}

##Description

With this command we can add a role that will be handed out if the Brawl Stars user has a specific amount of trophies with a specific Brawler.


##Usage
``-brawler <add / remove> <role> [trophies] [brawler]``


| Argument | Description |
| :--- | :--- | 
| brawler | Command name. |
| add/remove | Add or remove the role from the database. |
| role | The role the member gets (removed) for the required trophies the following brawler has. |
| trophies | The amount of trophies required for the user to claim the role saved with the following brawler. |
| brawler | The brawler name that needs a specific amount of trophies to claim the role. |

{% hint style="info" %}
When a brawler has 110 trophies, and we've saved a brawler role for 50, 100 and 150 brawler-trophies. The member will only get one role. In our case the 100 trophies role will be handed out.
{% endhint %}

{% hint style="danger" %}
The role argument must be one word, the role id, the mentioned role, or we can search for it when there are multiple roles with the argument we've inserted.
{% endhint %}

##How to actually use it


If we want to add the role ``Sandy_550`` when the member verifies and has the brawler ``Sandy`` at 550 trophies, we use this command.

```
-brawler add @Sandy_550 550 Sandy
```


When we want to remove the role `Sandy_550` from the database we have to enter the following command.

```
-brawler remove @Sandy_550
```