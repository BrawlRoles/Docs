{% hint style="success" %}
Permissions:

Bot permission: `SEND MESSAGES`, `EMBED LINKS`, `MANAGE WEBHOOKS`<br>User permission: `ADMINISTRATION`
{% endhint %}

##Description

With this command you can set a channel in your Discord Server where Brawl-Roles is logging everything into.

##Usage

`-verificationlog <enable / disable> [channel]`

| Argument | Description |
| :--- | :--- | 
| verificationlog | Command name. |
| add/remove | Whether the verification-log should be enabled and set to a channel or should be disabled. |
| channel | The channel in which the verification will be logged. |

{% hint style="warn" %}
We recommend making this channel only visible for Moderator and Administrator.
{% endhint %}

##How to actually use it

For enabling and set the verification-log to `#verification-log` we need to enter the following command.

```
-verificationlog enable #verification-log
```

For change or disable we need to disable the command. When changing we have to use the command from above after we disabled it.

```
-verificationlog disable
```