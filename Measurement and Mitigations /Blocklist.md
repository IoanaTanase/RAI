# Blocklists

The default AI classifiers are sufficient for most content moderation needs. However, you might need to screen for items that are specific to your use case. Blocklists let you add custom terms to the AI classifiers. You can use blocklists to screen for specific terms or phrases that you want to flag in your content.

Code samples on: https://learn.microsoft.com/en-us/azure/ai-services/content-safety/how-to/use-blocklist?tabs=windows%2Crest

## Blocklists in Foundry

Source: https://learn.microsoft.com/en-us/azure/ai-foundry/how-to/use-blocklists

You can create custom blocklists in the Azure AI Foundry portal as part of your content filtering configurations. The following steps show how to create custom blocklists as part of your content filters in Azure AI Foundry portal.

### Create a blocklist 
1. Go to Azure AI Foundry and navigate to your project. Then select the Safety+ Security page on the left nav and select the Blocklists tab.

![image](https://github.com/user-attachments/assets/5a9beb13-90d9-4630-9c47-e22cfa244518)

2. Select Create a blocklist. Enter a name for your blocklist, add a description, and select an Azure OpenAI resource to connect it to. Then select Create Blocklist.

3. Select your new blocklist once it's created. On the blocklist's page, select Add new term.

4. Enter the term that should be filtered and select Add term. You can also use a regex. You can delete each term in your blocklist.

### Attach a blocklist to a content filter configuration

1. Once the blocklist is ready, go back to the Safety+ Security page and select the Content filters tab. Create a new content filter configuration. This opens a wizard with several AI content safety components.

![image](https://github.com/user-attachments/assets/120245b3-da34-4a1e-8ad6-85a48ba783f7)

2. On the Input filter and Output filter screens, toggle the Blocklist button on. You can then select a blocklist from the list. There are two types of blocklists: the custom blocklists you created, and prebuilt blocklists that Microsoft provides—in this case a Profanity blocklist (English).

3. You can now decide which of the available blocklists you want to include in your content filtering configuration. The last step is to review and finish the content filtering configuration by selecting Next. You can always go back and edit your configuration. Once it’s ready, select a Create content filter. The new configuration that includes your blocklists can now be applied to a deployment.

