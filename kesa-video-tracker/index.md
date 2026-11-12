---
layout: page
title: Kesa Video Tracker
permalink: /kesa-video-tracker/
---

Kesa Video Tracker counts the short and long videos you watch, shows your statistics, and displays a large banner when you watch more videos in a day than your limit.

[Privacy policy]({{ '/kesa-video-tracker/privacy/' | relative_url }})

## Supported sites

| Site | Counts as |
|---|---|
| YouTube Shorts | short |
| YouTube videos | long |
| YouTube previews (a video that plays when you hover a thumbnail) | long, or short for a Short |
| TikTok | short |
| Instagram Reels | short |

## What counts as a watched video

- A video counts only after it has actually played for a while: 5 seconds for short videos, 30 seconds for long videos, and 30 seconds for YouTube previews. You can change these times in Settings.
- Each video counts once per day, even if you watch it again or scroll back to it. A preview and the full video count as the same video.
- Paused videos, YouTube ads, and videos in the Instagram home feed don't count.

## The daily limit banner

When you watch more videos in a day than your limit, a full-screen banner appears over the video and pauses it. You can choose:

- **Close this tab**
- **Keep watching**: the banner appears again after the next video.
- **Don't show again today**: no more banners until tomorrow.

You can set three limits in Settings: all videos, short videos only, and long videos only. A limit of 0 turns it off. By default the banner appears when you watch more than 30 videos in a day.

## Statistics

Click the extension icon in the toolbar to open the popup:

- **Today:** short, long and total videos, with watch time, and progress toward each limit.
- **Last 14 days:** a chart of videos per day, split into short and long. Hover a day for details, or open the table view.
- **Scoreboard:** a calendar of the last 20 weeks. Each day shows the icon of the site you watched most, and brighter tiles mean more videos. A red ring marks days over a limit.
- **Summary:** averages for the last 7 and 30 days, all-time totals, total watch time, and how many days went over a limit.

## Streaks and achievements

The extension keeps score, and it isn't always kind about it.

- **Streak card:** the popup shows your current streak. Days in a row over your limit give you a hot streak ("3-day streak over the limit. Impressive commitment to the wrong goal."). Days in a row under it give you a clean streak. The banner mentions your hot streak too. Streaks need at least one daily limit.
- **Achievements:** 17 badges, shown in the popup. Hover or focus a badge to see what it takes, or the comment you earned. Locked badges show your progress.
- **Pop-ups:** when you unlock an achievement, a small card appears in the corner of the page for a few seconds. You can turn these off in Settings.

| Badge | How to unlock |
|---|---|
| 🎬 It Begins | Watch your first video |
| 💯 Hundred Club | Watch 100 videos |
| 🧟 Thousand-Yard Stare | Watch 1,000 videos |
| 👍 Thumb Athlete | Watch 1,000 short videos |
| 🥔 Couch Potato | Watch 10 hours of video |
| 🛋️ Couch Archaeologist | Watch 100 hours of video |
| 🏆 Lifetime Achievement | Watch 1,000 hours of video |
| 🏃 Marathon | Watch 100 videos in one day |
| 🌀 Shorts-aholic | Watch 50 short videos in one day |
| 🚨 Limit Breaker | Go over your daily limit once |
| 🔁 Repeat Offender | Go over your limit on 10 days |
| 🔥 Hot Streak | Go over your limit 3 days in a row |
| 🌋 Unstoppable | Go over your limit 7 days in a row |
| 🦉 Night Owl | Watch 10 videos between midnight and 5 am |
| 🌍 Grand Tour | Watch YouTube, TikTok and Instagram on the same day |
| 🧘 Monk Mode | Stay under your limit 7 days in a row |
| 🌱 Touched Grass | Stay under your limit 30 days in a row |

Achievements and streaks are worked out from your daily statistics, so history from before an update counts too. Deleting all statistics in Settings also resets achievements.

## Settings

Open Settings from the popup to change:

- the daily limits
- how many seconds a video must play before it counts
- which sites are tracked
- whether the banner pauses the video
- whether achievement pop-ups appear
- debug logging, for troubleshooting

You can also export your statistics as a JSON file, reset today's counts, or delete all statistics.

## Troubleshooting

If videos on a site aren't being counted:

1. Open Settings, turn on **Debug logging**, and save.
2. Reload the video page and open the browser's developer console (F12, then the Console tab).
3. Look for lines starting with `[KesaVideoTracker]`. They show each detected video, each counted view, and each banner decision.

Sites change their pages from time to time, which can stop detection on one site. If that happens, [open an issue](https://github.com/kesa-md/docs/issues) and include those console lines.
