# webots-competition-competitor

[![Webots Badge](https://badgen.net/badge/icon/Rankings?label=Webots)](https://cyberbotics.github.io/webots-competition-organizer-template/)

## Register
- Make a new repository out of [the template](https://github.com/cyberbotics/webots-competition-organizer-template/generate).
- Add `lukicdarkoo` to [Manage access](https://docs.github.com/en/free-pro-team@latest/github/administering-a-repository/managing-teams-and-people-with-access-to-your-repository#inviting-a-team-or-person) section so the [organizer](https://github.com/lukicdarkoo-bot) can clone your private repository.
- Add your repository to [competitors.txt](https://github.com/cyberbotics/webots-competition-organizer-template/edit/main/competitors.txt).

## Develop

Download and install [Webots](https://github.com/cyberbotics/webots/releases/latest) on your local computer.

Create the following directory structure:
```bash
git clone https://github.com/cyberbotics/webots-competition-organizer-template.git
git clone [url_to_this_repo] webots-competition-organizer-template/controllers/participant_controller
```

Run the simulation:
```bash
webots webots-competition-organizer-template/worlds/competition.wbt
```

Once you are satisfied with the result, you can push the changes:
```bash
cd webots-competition-organizer-template/controllers/participant_controller
git add -A
git commit -m "Great improvement"
git push
```

## See preview
Once the changes are pushed it is usefull to verify whether your controller works properly in the competition.
The Webots GitHub action generates a preview of the competition and publishes it to the `gh-pages` branch.
Therefore, you have to choose the `gh-pages` branch [as the publishing source](https://docs.github.com/en/free-pro-team@latest/github/working-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site#choosing-a-publishing-source).
Then, you can access the preview at `[your_username].github.io/[your_repo_name]`.
