{% hint style="success" %}
Permissions:

Bot permission: `ADMINISTRATION`<br>User permission: `ADMINISTRATION`
{% endhint %}

##Description

With this command we can change the bot's prefix of the server.

##Usage

-setprefix <prefix>

| Argument | Description |
| :--- | :--- | 
| setprefix | Command name. |
| prefix | The new prefix. |

{% hint style="danger" %}
There is a minimum of 1 and a maximum of 5 characters for the prefix.
{% endhint %}

##How to actually use it

If we want to change the default prefix from `-` to `$` we use the following command.

```
-setprefix $
```

{% hint style="info" %}
When we mention the bot it returns us its prefix.<br>We can also mention the bot and enter a command without prefix `@BrawlRoles help`.
{% endhint %}