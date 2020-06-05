{% hint style="success" %}
Permissions:

Bot permission: `ADMINISTRATION`<br>User permission: `BAN_MEMBERS`
{% endhint %}

##Description

With this command you can set, reset or get a Usertag of a server member. You can also find the user, the tag is saved to with the option find.

##Usage

`-tag <option> [user / tag] [tag]`

| option | Description | Usage |
| :--- | :--- | :--- |
| find | Find a user saved in the Database by its Tag | -tag find <tag> |
| get | get a tag saved by the mentioned user in the Database | -tag get <user> |
| reset | reset a user's tag | -tag reset <user> |
| set | link a tag to the mentioned user | -tag set <user> <tag> |
|  |  |  |


{% hint style="danger" %}
The user argument must be one word, the member id, the mentioned member or you can search for it when there are multiple members with the argument you have inserted.
{% endhint %}

##How to actually use it

![](../../assets/knirpsii_profile.png)


We have the tag `#YU9G98V8` but we don't know who saved themselves as this user. So we can find him/her with the following command.
```
-tag find #YU9G98V8
```

If we want to get the Tag saved by the user `@Knirpsii`, we run the following command.

```
-tag get @Knirpsii
```

If we want to reset the Tag from the user `@Knirpsii`, we can do so with the following command.

```
-tag reset @Knirpsii
```

If we want to edit the tag from the user `@Knirpsii` to `#YU9G98V8`` we can do so with this command.
```
-tag set @Knirpsii #YU9G98V8
```
