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
Hit up jewel to publish -or- if you've been setup with the "production-merge" branch (which is a local-only branch), continue with the following steps.

1. Open your Github Desktop App
2. Select your "livetesting-main" branch
3. From the command line: merge the "TESTING" branch into your "production-merge" branch
4. From the Github Desktop App: hit "Push Origin"
5. Go to Github.com > thepurpleflower.org repo > Pull Requests
6. Open and review PR for `preview` branch into `main` branch
7. Check to make sure that the `CNAME` file is not in the commit and is not changed. If the PR looks good, you can safely merge and close the PR
8. It can take a couple of minutes for the live site to reflect the changes
7. Verify by going to https://thepurpleflower.org


## Caution

Working directly on the producton code base (thepurpleflower.org) can wreak havoc when we do need to work on staging site (new.thepurpleflower.org) due to the disparate CNAME files that need to be separate in each repo due to github hosting the sites.

If an update is accidentally made on production and not staging, then it should manually be copied over to the staging code base and committed- so future updates don't accidentally roll-back production.

## Setting Up a Local "preview-to-production" Branch


1. Add the live repo as a remote named 'live-testing'
git remote add live-testing https://github.com/The-Purple-Flower/thepurpleflower.org.git

2. Create the "Production-Merge" Branch
git checkout -b production-merge

3. Edit the CNAME file so it matches the PRODUCTION website
thepurpleflower.org

4. Push and Link to the Live Repo's "Preview" Branch
git push -u live-testing production-merge:preview



## Queing Updates

Currently, jewel can publish changes by making a few Github command line calls. There is likely a way to automate this so that anyone with access to the live site repo can click a button to publish. That's what's TBD.

## Optimizations

https://www.minifier.org/