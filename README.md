# Project: Crossroads

Project: Crossroads is a shared multiplayer platform for singleplayer games —
one launcher and one updater, with a separate multiplayer adapter per game. It
is built from the useful foundations of the abandoned VaultMP project and
redesigned for current private testing.

It is an independent community project, not affiliated with or endorsed by the
publishers or owners of any supported game. You must own a legal copy of any
game you want to play.

## What actually works right now

**KotOR I** is where the active work is. Several players can see each other as
their own characters, with their own name, face and appearance taken from their
save; movement and animation are mirrored; equipment changes reach the right
player mid-session; and players can walk between areas and still see each other.

**Fallout 3** has two-player movement and visible remote players in the
exterior world. Work on it is currently paused while KotOR moves forward.

**Neither is finished.** Combat, quests, inventory, NPCs and dialogue are not
synchronized in either game. Only players are shared.

**Please keep sessions to 2–3 players.** There is a known scaling problem in how
appearance and equipment are shared, and larger sessions get worse rather than
better. Fixing it is the current priority.

Other games listed in the launcher are development placeholders. There is no
adapter behind them.

## Private multiplayer tester

The current tester targets Windows, plus:

- **Fallout 3**: Game of the Year Edition, `Fallout3.exe` 1.7.0.3 produced by
  the Fallout Anniversary Patcher, and FOSE 1.2 beta 2
- **KotOR I**: the English Steam release

Download the
[Project: Crossroads private network tester](downloads/Project-Crossroads-Private-Network-Test.zip),
extract it to a normal folder, and follow the included README.

That download is a small bootstrap containing the launcher and its updater.
After setup, the launcher checks this repository's update channel and installs
verified Crossroads program updates, so testers do not download replacement ZIP
files. Updates are fetched over HTTPS and must pass a published SHA-256 check;
a failed check installs nothing and leaves the existing build alone.

## Status

This is a trusted-friend development test, not a finished public multiplayer
release.

A host may set a join code, and a server started with one admits only players
who present it. A server started without one is open and will admit anyone who
can reach it. Gameplay traffic is not encrypted in either case, and a join code
is not a password — treat a session as visible to anyone on the network path.
What the server does enforce is that it validates every field of every packet it
receives and never trusts what a client reports about itself.

Project: Crossroads does not include or redistribute Fallout 3, KotOR, FOSE, the
Fallout Anniversary Patcher, or any game asset. Obtain those separately from
their original sources.
