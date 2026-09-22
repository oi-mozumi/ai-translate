# AI Translate builds

Ready-made builds of [AI Translate](https://gitlab.com/oi_mozumi/ai-translate),
a Vencord plugin that translates Discord messages with an AI model of your
choice. The plugin itself, its instructions and the install command live on
GitLab.

Vencord only runs plugins that were built into it, so the install command
downloads Vencord with AI Translate already inside. Those files are made here:
every hour GitHub Actions checks whether Vencord or AI Translate has a new
version, and when one does, it builds the two together and publishes the
result on the [Releases](https://github.com/oi-mozumi/ai-translate/releases)
page. The install command and the plugin's own updater download from there, so
there is nothing to download by hand.

Each release links to the exact source it was built from. The build steps are
in [`build/github.sh`](https://gitlab.com/oi_mozumi/ai-translate/-/blob/release/build/github.sh)
in the plugin's repository. `latest.txt` names the newest build; the robot
updates it with every build, which also keeps GitHub from pausing the hourly
schedule.

## Licence

GPL-3.0-or-later, the same as Vencord and AI Translate.
