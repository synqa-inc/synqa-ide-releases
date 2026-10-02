# Synqa IDE

**Your AI coding agents, all in one place, with a tiny pixel office to watch them work.**

Synqa IDE is a Mac app for running AI coding agents such as Claude Code and Codex. Start several at once, follow what each one is doing, step in when one needs you, then review and commit its changes. Every agent shows up as a little pixel-art worker in Synqa HQ, a virtual office that sits beside your work.

<p align="center">
  <a href="https://github.com/synqa-inc/synqa-ide-releases/releases/latest/download/Synqa-IDE-arm64.dmg"><strong>Download for Mac (Apple silicon)</strong></a>
  ·
  <a href="https://github.com/synqa-inc/synqa-ide-releases/releases">All releases</a>
</p>

![Synqa IDE: a finished agent conversation next to the Synqa HQ pixel office](images/01-hero-thread-office.png)

Powered by [BB](https://github.com/get-bb/bb).

---

## Highlights

### Synqa HQ: watch your agents at work

![Synqa HQ, a pixel-art office full of AI agents at desks, in meeting rooms and in the lounge](images/03-office.png)

Synqa HQ is our take on **BB Office**, the pixel office plugin for BB. Each of your agents becomes a worker, and where it sits tells you what it is doing:

- **Busy agents sit at desks.** Agents working on related jobs meet up in a meeting room.
- **Idle agents relax in the lounge**, and after a while (30 minutes by default) they walk out the door.
- **A coloured ring under each worker** shows its state: working, thinking, waiting for you, failed or idle. A worker that needs you shows an amber speech bubble.
- **Hover** to see a worker's name, **click** to see who it works with, and **double-click** to jump straight into its conversation.
- **A footer keeps count** of how many agents are working, need you, have failed or are idle. You can show every project or just one.
- **Posters on the wall** show how much of each AI plan's usage you have used.
- **Six pixel-art characters**, plus two office pets, Claudio and Gitcat.

The office has open-plan desks, focus offices, huddle rooms, project rooms, a boardroom, a library, a cafe and a lounge. Prefer something smaller? Switch to the compact BB Office floor plan.

Keep the office wherever suits you: as a **floating** window you can drag and shrink, **docked** in the side panel, or in **its own window**. You can also hide it and bring it back from the menu bar.

**Make it yours by asking.** Tell an agent "turn off the pets" or "make idle agents leave after an hour". It shows you the change first and applies it only when you say yes.

### Run many agents at once, safely

![An agent's changes ready for review, with a Commit button](images/02-thread-diff-review.png)

- **Each conversation can get its own copy of your project**, so agents working side by side don't trip over each other's changes. Synqa cleans up these copies when you're done with them.
- **Agents can start helper agents.** Synqa shows each agent's helpers in its header, with a dot for each one's status.
- **Review before anything lands.** The Review button shows exactly what changed. When you're happy, commit with one click, and let AI write the commit message if you like.
- **Pull requests from the conversation.** See an agent's linked pull request, mark it ready or merge it, using your own GitHub sign-in.

### Plan work on a board

![The Tasks board with Backlog, Todo, In Progress, In Review and Done columns](images/04-tasks-board.png)

**Tasks** is a simple project board built in. Write tasks, sort them into columns, and hand one to an agent. The agent is asked to move the task to **In Review** when it finishes, so you can check its work.

### Lives in your menu bar

The menu-bar icon lists your running agents and any that need you. From there you can open the app, show the office, or stop every running agent at once with **Pause all agents**. You can also close the window and leave your agents running in the background.

### Looks good, light or dark

![Synqa IDE in dark mode, with the office keeping its own colours](images/05-dark-thread-office.png)

Synqa IDE has its own look: a charcoal, warm paper and signal green palette, with the JetBrains Mono font for code. Prefer something else? BB's original look is one click away, along with Nord, Dracula, Solarized, Gruvbox and Catppuccin.

---

## Ready out of the box

Synqa IDE is built on BB and keeps every BB feature. It adds a few things so you can get going without setting anything up:

| | Synqa IDE | Plain BB |
| --- | --- | --- |
| Synqa HQ pixel office | Installed and on | Not included |
| Tasks board | Installed and on | Optional install |
| Look | Synqa theme, with BB's look still available | BB theme |
| Menu-bar icon and background running | Included | Not included |
| Usage tracking (telemetry) | **Off** | On by default (anonymous) |
| Updates | Downloaded in the background from this page | BB's own updates |
| Your data | Its own folder, separate from BB | BB's folder |

You can run Synqa IDE and BB side by side. They don't share data.

---

## Install

1. [Download Synqa IDE](https://github.com/synqa-inc/synqa-ide-releases/releases/latest/download/Synqa-IDE-arm64.dmg).
2. Open the downloaded file and drag **Synqa IDE** into your **Applications** folder.
3. Open Synqa IDE from Applications.

The app is signed by Synqa and notarized by Apple, so your Mac opens it like any other app.

### Updates

Synqa IDE checks this page for new versions, downloads them in the background, and asks you to restart when one is ready. You don't need a GitHub account.

**On version 1.0.0?** That version can't update itself. Download and install 1.0.1 (or any newer version) by hand once, using the steps above. After that, updates arrive automatically.

## What you need

- **A Mac with Apple silicon** (M1 or newer) running **macOS 13 Ventura or later**. Intel Macs, Windows and Linux are not supported.
- **At least one AI coding agent you're already signed in to**, such as Claude Code, Codex, Pi, or another agent that supports ACP (for example Cursor or opencode). Synqa IDE doesn't come with its own AI. It uses the agents and subscriptions you already have.
- **The GitHub CLI** (`gh`), signed in, if you want to work with pull requests.

## Where your data lives

Synqa IDE keeps its data on your Mac, mainly in the **`~/.synqa`** folder in your home folder, with the desktop app's own files in `~/Library/Application Support/Synqa IDE`. It is kept separate from BB's data, even if you have BB installed too.

To remove Synqa IDE completely, quit it, move it from Applications to the Bin, and delete the `~/.synqa` and `~/Library/Application Support/Synqa IDE` folders.

## Privacy

- **No usage tracking by default.** Synqa IDE doesn't send analytics about how you use it.
- **The pixel office runs entirely on your Mac.**
- Some things do go online, as you'd expect: your agents talk to their AI providers, and the app checks GitHub for updates.
- **Optional BB account features use BB's online service.** If you sign in to a BB account, remote access goes through it, and bb cloud AI (on by default once you sign in) writes thread titles and commit messages and transcribes voice input through BB's hosted service. You can turn bb cloud AI off in settings.

## Report a problem

Email **[karl@synqa.ca](mailto:karl@synqa.ca)**, or use **Report a bug** in the app's sidebar (it opens an email for you). Tell us your Synqa IDE version (Settings → Updates), what you did, and what happened.

---

## Credits

Synqa IDE is **powered by [BB](https://github.com/get-bb/bb)**, the open-source agent app by Michael Yong. Thank you to the BB project for the engine underneath everything here.

The pixel office is **BB Office** by Michael Yong. Synqa HQ adds our own floor plan, furniture, signs, status rings and window options on top of it. BB Office is built on:

- [Pixel Agents](https://github.com/pixel-agents-hq/pixel-agents) by Pablo De Lucca (MIT), for the office engine, furniture, characters and pets
- [JIK-A-4's MetroCity character pack](https://jik-a-4.itch.io/metrocity-free-topdown-character-pack) (CC0), which the characters are based on
- [Hugeicons](https://hugeicons.com/) (MIT), for the floor plan icon

Synqa IDE is an independent project. It isn't made or endorsed by the BB project, Anthropic, OpenAI, Cursor or Pixel Agents. Their names appear here only to say what Synqa IDE works with or is built on.

## Licence

Synqa IDE is released under the [MIT Licence](LICENSE), the same licence as BB. The LICENSE file keeps the original BB copyright notice, and [THIRD_PARTY_NOTICES](THIRD_PARTY_NOTICES) lists BB, BB Office and the office art.

This repository holds the app downloads and update files.
