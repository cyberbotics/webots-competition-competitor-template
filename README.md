# webots-competition-competitor

[![Webots Badge](https://badgen.net/badge/icon/Rankings?label=Webots)](https://cyberbotics.github.io/webots-competition-organizer-template/)

## Register

- Make a new repository out of [the template](https://github.com/cyberbotics/webots-competition-organizer-template/generate).
- Add `lukicdarkoo` to [Manage access](https://docs.github.com/en/free-pro-team@latest/github/administering-a-repository/managing-teams-and-people-with-access-to-your-repository#inviting-a-team-or-person) section so the [organizer](https://github.com/lukicdarkoo-bot) can clone your private repository.
- Add your repository to [competitors.txt](https://github.com/cyberbotics/webots-competition-organizer-template/edit/master/competitors.txt).

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

Once your changes are pushed, the Webots GitHub action runs the competition and publishes the result at https://cyberbotics.github.io/webots-competition-organizer-template/.

It takes a few minutes (possibly hours if the simulation is complex) for running the simulation.
