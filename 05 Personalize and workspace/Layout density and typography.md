---
aliases:
- Layout density and typography
tags:
- kplex-help/how-to
- kplex/styling
- kplex/layout
Friend:
- '[[02 Navigate and explore/Mobile and touch]]'
- '[[04 Filter and focus/Keep layout vs Reflow]]'
Next:
- '[[05 Personalize and workspace/Node styles from help tags]]'
---
Use **Configure Plex layout** to expose live layout controls. K-Plex supports independent horizontal and vertical density, Parent/Child column counts, base font size, regular-node width and wrapped labels.

Large Parents, Children, Friends, Challengers and Siblings regions get their own size limits and can scroll independently. Parent rows support up to three columns and Child rows up to seven. Different device/surface profiles let desktop, tablet, mobile, sidepanel and pop-out layouts stay tuned for their available space.

Typography is also global presentation policy: increasing **Maximum label length**, **Maximum node width**, or enabling **Wrap node labels** makes long titles easier to scan without changing note names.

For working space rather than text density, use [[05 Personalize and workspace/Fullscreen and Zen mode|Fullscreen and Zen mode]]. Neither mode automatically fits the graph; use Fit to screen if desired.

## Readability and compact-pane improvements

**Maximum label length is independent of horizontal/vertical density.** A label limit of 100 does not shrink when you make the layout denser. Under **Settings → K-Plex → Visual styling**, device-specific typography choices apply consistently to both the center and surrounding nodes, including sparse configurations with only one field overridden.

When editing the layout from a narrow or short pane, K-Plex keeps slider controls usable and prevents the panel from colliding with the bottom-left disclosure. Font size, label length and node width controls stack vertically, with **Wrap node labels** below them. Slider gestures that begin on a slider continue to adjust that control rather than unexpectedly panning the Plex.

In **this help vault**, the base node label limit is **100 characters**, while maximum node width and wrapping remain separate layout choices. Long titles may still be constrained by the available on-screen width.

[Changes: PR #108](https://github.com/zsviczian/kplex/pull/108) · [PR #112](https://github.com/zsviczian/kplex/pull/112).
