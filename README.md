# purpleflower
purpleflower.org

New Website Development for ThePurpleFlower.org

We have 2 repos serving 2 versions of the site:

1. thepurpleflower.org (live site) repo serves the live site at https://thepurpleflower.org (and https://www.thepurpleflower.org) based on the MAIN branch.
2. new.thepurpleflower.org (preview site) repo serves the preview site at https://new.thepurpleflowerofcc.org (note the different domain name) based on the TESTING branch.


## Local Development

The site is not dynamic and can be worked on locally without any special applications beyond using GIT for code management and to allow you to push to the Github server, where the website is hosted. All development is done inside the new.thepurpleflowerofcc.org repo.

A] To get started:
1. Install the GitHub Desktop App
2. Login with your GitHub account, that's a member of The Purple Flower organization
3. Under "Current Repository" select "Add" and then "Clone Repository..."
4. Select *New.ThePurpleFlowerofCC.org*
5. Select a location on your computer where the files will be copied

B] To view the site on your local machine:
1. Open your web browser and then "File > Open"
2. Navigate to the location you selected in the previous setup instructions
3. Select "index.html" and voila! The site will load

C] To make edits and preview them before going live:
1. Open your Github Desktop App
2. Make sure your "TESTING" branch is selected and active
3. Edit the .html file of choice (e.g. index.html) in your favorite editor (SublimeText is simple)
4. Make edits
5. Refresh your browser (see step B)

D] To preview edits on the staging site:
1. Open your Github Desktop App
2. Review the edits. It will show you line-by-line edits.
3. Enter a description of the change(s) you've made. 
4. Click "Commit"
5. Click "Push Origin" to upload the changes to the staging site
6. Review your updates at https://new.thepurpleflowerofcc.org

E] To push edits live:
Hit up jewel to publish -or- if you've been setup with the "livetesting-main" branch (which is a local-only branch), continue with the following steps.

1. Open your Github Desktop App
2. Select your "livetesting-main" branch
3. From the command line: merge the "TESTING" branch into your "livetesting-main" branch
4. From the Github Desktop App: hit "Push Origin"
5. Go to Github.com > thepurpleflower.org repo > Pull Requests
6. Review the open pull request that should have been created automatically after the "livetesting-main" branch was pushed
7. Assuming it all looks good and can be merged automatically, hit 'merge' to close the PR — be sure to make sure that the CNAME file IS NOT CHANGED ... as that will make the live site error out
8. It can take a couple of minutes for the live site to reflect the changes
7. Verify by going to https://thepurpleflower.org

## Queing Updates

Currently, jewel can publish changes by making a few Github command line calls. There is likely a way to automate this so that anyone with access to the live site repo can click a button to publish. That's what's TBD.

## Optimizations

https://www.minifier.org/