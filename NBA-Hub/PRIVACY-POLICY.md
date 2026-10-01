# nba-hub Privacy Policy

Effective date: October 1, 2026

nba-hub is a Reddit app, built on Reddit's Developer Platform (Devvit), that posts and maintains live basketball game threads (NBA and WNBA) in subreddits where a moderator has installed it. This policy explains what information the app handles, where it goes, and what it does not do.

## Summary

- The app does not collect, sell, or share personal information.
- Viewers of a game thread are not identified, tracked, or profiled.
- The only user identifier the app ever handles is the Reddit username of the moderator who installs it, used once for an installation notice.
- Everything the app stores lives inside Reddit's infrastructure and is operational data about games and threads.

## Information the app handles

### Viewers

When you open a game thread, the app's web view requests game data from the app's server, which runs inside Reddit's platform. That request does not include your Reddit username, email address, IP address, or any identifier the app could use to recognize you. The app does not use analytics, advertising, fingerprinting, cookies, or third-party scripts.

Two display preferences, the light/dark theme and the full/half court view, are kept in your own browser's local storage so the app remembers them. They never leave your device and the app cannot read them from the server.

### Moderators

When a moderator installs the app, Reddit sends the app an installation event containing the subreddit name and the installing moderator's Reddit username. The app sends a single Reddit private message with those two facts to the developer (u/0xgod) so the developer knows where the app is in use. This information is not stored by the app or shared further.

Moderators use the app's settings page and menu items, which Reddit provides. Menu actions can send a status report to the subreddit's modmail; that report contains only game and thread information.

### Game data

All basketball data (scores, play-by-play, box scores, shot locations, odds, injuries, team logos, player headshots) comes from ESPN's public data services. The app's server fetches it; your browser never contacts ESPN directly through this app. The app has no relationship with ESPN beyond reading that public data.

## What the app stores

The app uses Reddit's Redis storage, scoped to the subreddit where it is installed, for operational data only:

- which Reddit post corresponds to which game, and the state of that thread (posted, pinned, locked, postgame posted, removed by a moderator);
- short-lived caches of ESPN responses, built game views, and proxied images so that one fetch serves every viewer of a thread;
- bookkeeping for the once-a-minute maintenance job, such as the time of its last run.

None of this is about a person. Caches expire automatically (seconds to a day); thread records are kept for as long as the app maintains the thread and are removed when the app is uninstalled from the subreddit, in line with Reddit's platform behavior.

## What the app does not do

- It does not read your comments, votes, browsing history, or any content you post.
- It does not request or store your Reddit profile, email address, or location.
- It does not use third-party analytics, advertising networks, or tracking pixels.
- It does not sell, rent, or share any information with anyone.
- It does not transmit any information to the developer's own servers; there are none.

## Children

The app is intended for use on Reddit by people who meet Reddit's minimum age requirements. It does not knowingly collect information from anyone, including children.

## Reddit's role

The app runs entirely on Reddit's Developer Platform. Reddit's own Privacy Policy governs Reddit's handling of your account and activity, including data that Reddit makes available to apps. See https://www.reddit.com/policies/privacy-policy.

## Changes

If this policy changes, the effective date above will be updated and the new version will be published at the same location. Material changes will also be noted in the app's listing.

## Contact

Questions about this policy: send a Reddit message to u/0xgod.
