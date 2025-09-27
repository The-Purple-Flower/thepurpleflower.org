# purpleflower
purpleflower.org

New Website Development for ThePurpleFlower.org

## Local Development

The site is not dynamic and can be worked on locally without any special applications. 

A] To get started:
1. Install the GitHub Desktop App
2. Login with your GitHub account, that's a member of The Purple Flower organization
3. Under "Current Repository" select "Add" and then "Clone Repository..."
4. Select ThePurpleFlower.org
5. Select a location on your computer where the files will be copied

B] To view the site on your local machine:
1. Open your web browser and then "File > Open"
2. Navigate to the location you selected in the previous setup instructions
3. Select "index.html" and voila! The site will load

C] To make edits and preview them before going live:
1. Edit the .html file of choice (e.g. index.html) in your favorite editor (SublimeText is simple)
2. Make edits
3. Refresh your browser (see step B)

D] To push edits live:
1. Open your Github Desktop App
2. Review the edits. It will show you line-by-line edits.
3. Enter a description of the change(s) you've made. 
4. Click "Commit"
5. You will now see a screen that says "No local changes" with a button to "Push Origin" — click that
6. It can take a couple of minutes for the live site to reflect the changes
7. Verify by going to https://thepurpleflower.org

## Queing Updates

For when you're making edits and want to save them without them going live ... instructions coming soon.

Short is that we have 2 repos serving 2 versions of the site.

1. thepurpleflower.org (live site) repo serves the live site at https://thepurpleflower.org (and https://www.thepurpleflower.org)
2. new.thepurpleflower.org (preview site) repo serves the preview site at https://new.thepurpleflowerofcc.org (note the different domain name)

Updates will always happen in the second (new.thepurpleflower.org) repo so that changes can be confirmed before pushed live.

Currently, jewel can publish changes by making a few Github command line calls. However, there is a way to automate this so that anyone with access to the live site repo can click a button to publish. That's what's TBD.

## Optimizations

https://www.minifier.org/
