---
{"dg-home":false,"dg-publish":true,"permalink":"/sans-titre/","dgHomeLink":false,"dgPassFrontmatter":true}
---


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

It's a bit of work to set this all up, but when you're done you'll have a digital garden in which you are in control of every part of it, and can customize it as you see fit. Which is what makes digital gardens so delightful.  
Lets get started:

1.  First off, you will need a GitHub account. If you don't have this, create one [here](https://github.com/signup).
2.  You'll also need a Netlify account. You can sign up using your GitHub account [here](https://app.netlify.com/)
3.  Open [this repo](https://github.com/oleeskild/digitalgarden), and click the green "Deploy to netlify" button. This will open netlify which in turn will create a copy of this repository in your GitHub account. Give it a fitting name like 'my-digital-garden'. Follow the steps to publish your site to the internet.
4.  Now you need to create an access token so that the plugin can add new notes to the repo on your behalf. Go to [this page](https://github.com/settings/tokens/new?scopes=repo) while logged in to GitHub. The correct settings should already be applied. If you don't want to generate this every few months, choose the "No expiration" option. Click the "Generate token" button, and copy the token you are presented with on the next page.
5.  In Obsidian open the setting menu and find the settings for "Digital Garden". The top three settings here is required for the plugin to work.  
    Fill in your GitHub username, the name of the repo with your notes which you created in step 3. Lastly paste the token you created in step 4. The other options are optional. You can leave them as is.
6.  Now, let's publish your first note! Create a new note in Obsidian. And add the following to the top of your file




**This does two things:**

-   The dg-home setting tells the plugin that this should be your home page or entry into your digital garden. (It only needs to be added to _one_ note, not every note you'll publish).
    
-   The dg-publish setting tells the plugin that this note should be published to your digital garden. Notes without this setting will not be published. (In other terms: Every note you publish will need this setting.)
    

7.  Open your command pallete by pressing CTRL+P on Windows/Linux (CMD+P on Mac) and find the "Digital Garden: Publish Single Note" command. Press enter.
8.  Go to your site's URL which you should find on [Netlify](https://app.netlify.com/). If nothing shows up yet, wait a minute and refresh. Your note should now appear.

Congratulations, you now have your own digital garden, hosted free of charge!  
You can now start adding links as you usually would in Obisidan, with double square brackets like this: [Some Other Note](app://obsidian.md/Some%20Other%20Note)) to the note that you just published. You can also link to a specific header by using the syntax [Some Other Note > A Header](app://obsidian.md/Some%20Other%20Note#A%20Header). Remember to also publish the notes your are linking to as this will not happen automatically. This is by design. You are always in control of what notes you actually want to publish. If you did not publish a linked note, the link will simply lead to a site telling the user that this note does not exist.