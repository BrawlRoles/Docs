{% hint style="success" %}
Permissions:

Bot permission: `ADMINISTRATION`<br>User permission: `ADMINISTRATION`<br><br>Before the command can be used the verification-log must be enabled.
{% endhint %}

##Description

With this command you can enable the verification. 

##Usage

-verification <enable / disable> [channel] [with image] [name change] [role]

- Command name
- Whether the verification should be enabled or disabled
- The channel in which the verification will take place
- If the member must send an image with the verify command ([The image should look like this](../../assets/knirpsii_profile.png)) 
- If the members name should be changed to his/her Brawl Stars player name
- The default role every verified member gets

{% hint style="danger" %}
The role argument must be one word, the role id, the mentioned role or you can search for it when there are multiple roles with the argument you have inserted.
{% endhint %}

##How to actually use it

We want to enable the verification in the channel `#verification`. The verification will be with an image, and we won't change the members name. The role is `@Verified`.

```
-verification enable #verification yes no @Verified
```

{% hint style="info" %}
The verify command only works in the channel we've inserted.
{% endhint %}

When we want to change something like the channel or the role, we need to disable the verification and enable it again

```
-verification disable
```