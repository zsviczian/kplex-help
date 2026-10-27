---
aliases:
- Layout density and typography
tags:
- kplex/workspace
- kplex-help/how-to
- kplex/styling
- kplex/layout
Friend:
- '[[02 Navigate and explore/Mobile and touch]]'
- '[[04 Filter and focus/Keep layout vs Reflow]]'
Next:
- '[[05 Personalize and workspace/Node styles from help tags]]'
---
# Layout density and typography

Are long titles hard to read, or is the map too crowded for your screen? Adjust spacing, text and columns, or use One-sided layout in a narrow pane.

![[Assets/Screenshot - Layout controls.png]]

*The layout panel combines spacing, columns and readable labels; One-sided layout applies to the current device and pane context.*

Large Parents, Children, Friends, Challengers and Siblings regions get their own size limits and can scroll independently. Parent rows support up to three columns and Child rows up to seven. Different device/surface profiles let desktop, tablet, mobile, sidepanel and pop-out layouts stay tuned for their available space.

Typography is also global presentation policy: increasing **Maximum label length**, **Maximum node width**, or enabling **Wrap node labels** makes long titles easier to scan without changing note names.

For working space rather than text density, use [[05 Personalize and workspace/Fullscreen and Zen mode|Fullscreen and Zen mode]]. Neither mode automatically fits the graph; use Fit to screen if desired.

![[Assets/Screenshot - Node styling.png]]

*Settings provides shared text defaults as well as the live layout controls beside the graph.*

## Readability and compact-pane improvements

**Maximum label length is independent of horizontal/vertical density.** A label limit of 100 does not shrink when you make the layout denser. Under **Settings → K-Plex → Visual styling**, device-specific typography choices apply consistently to both the center and surrounding nodes, including sparse configurations with only one field overridden.

When editing the layout from a narrow or short pane, K-Plex keeps slider controls usable and prevents the panel from colliding with the bottom-left disclosure. Font size, label length and node width controls stack vertically, with **Wrap node labels** below them. Slider gestures that begin on a slider continue to adjust that control rather than unexpectedly panning the Plex.

In **this help vault**, the base node label limit is **100 characters**, while maximum node width and wrapping remain separate layout choices. Long titles may still be constrained by the available on-screen width.

## One-sided layout

Select **One-sided layout** below the Parents and Children sliders in Layout controls to put Friends and Challengers together in one shared list on the left. This removes the separate right-hand Challenger area without discarding Challenger relationships or changing their meaning and filters.

The checkbox changes the current device and pane context. All six choices are available under **Settings → K-Plex → Plex behavior → One-sided layout**: desktop, tablet and mobile, each with main-tab and side-panel choices. Pop-outs follow their device's main-tab choice for this option.

This is a compact alternative to the standard four-direction layout, not a custom layout engine or an additional ontology region. **One-sided layout** is the current label; earlier development notes called it Simplified layout.

For color rather than geometry, see [[05 Personalize and workspace/Colors and themes]]. For temporarily hiding the whole graph group, see [[05 Personalize and workspace/Sidecar]].
