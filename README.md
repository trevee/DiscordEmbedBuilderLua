# DiscordEmbedBuilderLua
### example:
```lua
local messageEmbed = MessageEmbed:New();
messageEmbed:SetColor('#ffeb00');
messageEmbed:SetAuthor('github.com/oxince', 'image url');
messageEmbed:SetTitle('Cool embed')
messageEmbed:SetDescription('fr its cool! get at https://github.com/oxince/DiscordEmbedBuilderLua/');
messageEmbed:AddField('PROgrammer #1', 'oxince', false);
messageEmbed:SetFooter('sent by github')
messageEmbed:SetTimestamp();


-- create your own WebhookHandler, its just a post request with this given data
WebhookHandler:ExecuteWebhook(RV.PrivateWebhook, {
  -- given data
  ['embeds'] = {
    messageEmbed.embed
  }
});
```
