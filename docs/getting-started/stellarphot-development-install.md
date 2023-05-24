# Install `stellarphot` for development

1. Fork a copy of the repository on github: go to [https://github.com/feder-observatory/stellarphot](https://github.com/feder-observatory/stellarphot) and click the "Fork" button
2. On *your fork* click the green code button and copy the URL.
3. Change directory to where you want to folder with the code to be: `cd name_of_folder`
4. Make a copy of stellarphot on your computer: `git clone url_for_your_fork`
5. Change directory to stellarphot: `cd stellarphot`
6. Add link to "official" copy: `git remote add upstream https://github.com/feder-observatory/stellarphot.git`
7. Check that your remotes are set up: `git remote -v`
    1. You should see two remotes, one called `origin` and one called `upstream`
8. Fetch info about all of the remotes: `git fetch --all`
8. Set the "official" copy of the "main" branch to the `upstream` copy: `git branch -u upstream/main`

