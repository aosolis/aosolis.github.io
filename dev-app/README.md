# Teams App Studio - Alpha Edition
The tools bundled in the Teams App Studio are designed to help you build enticing Microsoft Teams integrations.

# Installation Instructions
1. Open your Microsoft Teams client.
2. Ensure that you are in the developer preview.

![Developer Preview](DeveloperPreview.PNG "Developer Preview" )

3. Go to the App Gallery.

![App Gallery](AppGallery.PNG "App Gallery" )


4. Click Upload a custom App.

![Upload a Custom App](UploadCustomApp.PNG "Upload a Custom App" )

5. Select the alpha.zip file.
6. Press Add.

![Add Custom App](SideloadAdd.PNG "Add Custom App" )

7. Press Done.

After uploading the zip, the Teams App Studio can be found in your app flyout.

![App Flyout](Flyout.PNG "App Flyout" )

It includes these tools:

## 1. Manifest Editor Tab
This tab will help you build and edit your Microsoft Teams application manifest. The application manifest is required to sideload your application in Microsoft Teams for testing and to submit your application to the Office Store.

### Alpha Notes:
1. The welcome text is incorrect. Start your manifest by either creating a new one or importing an existing one.
2. Compose extensions are not currently supported. Importing a manifest with a compose extension will cause it to be removed upon export.
3. The exported manifest may not be valid if you have errors in any of the screens during manifest creation (including the App Details screen).
4. Valid Domains for tabs do not show errors properly. Valid domains must be valid https:// URLs and if you do not provide a valid https:// URL (for example, empty values are not valid and need to be deleted before proceeding) you will not be able to close the edit dialog.

## 2. Card Editor Tab and Card Bot
This tab works together with the bot (accessed through the Conversation tab) to help preview what a card sent through BotFramework will look like in Microsoft Teams. The flow starts on the Card Editor tab. You can edit the card properties in a form or through raw JSON. Once you have chosen the properties you want for your card you can copy the C# or Javascript code used to generate the card in your own bot or have the Card Bot send you the card to preview it. To send the card you must login first.

### Alpha Notes:
1. The image space is ambiguous. You must paste a valid image URL for the bot to send you the correct image. The image must be accessible from the internet for BotFramework to be able to send it in the preview.
2. The Card Editr may log you out after periods of inactivity. This is normal for the alpha, please log back in if this happens.