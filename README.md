# Scroll-Triggered Animations Debugger

A DevTools extension to visualize and debug [CSS Scroll-Triggered Animations](https://developer.chrome.com/blog/scroll-triggered-animations) (`timeline-trigger`, `animation-trigger`, `trigger-scope`).

- Visualize the Scroll-Triggered Animation’s scroller, element, and subject.
- Supports both ScrollTimeline (`scroll()`) and ViewTimeline (`view()`).
- Shows an active/inactive status light indicator that switches from red (Inactive) to green (Active) when the trigger activates.
- Plays nice with `position: sticky`.
- Visualize the `timeline-trigger-activation-range` (blue) and `timeline-trigger-active-range` (green) debug lines and boxes.
- Edit the `timeline-trigger-activation-range` and `timeline-trigger-active-range` values live.

## Demo

https://github.com/user-attachments/assets/b80bdeb7-b1d8-4d99-ae85-e63478684f55

## Installation

You can [get the extension from the Chrome Web Store](https://chromewebstore.google.com/detail/ganooodmdnigcfdddlijnhkipjklbgag).

[![Available on the Chrome Web Store](./assets/chrome-webstore.svg)](https://chromewebstore.google.com/detail/ganooodmdnigcfdddlijnhkipjklbgag)

If you like this extension, please leave a review on the Chrome Web Store. I’d appreciate it.

## Usage

Once installed, a new “Scroll-Triggered Animations” pane gets added to Chrome DevTools’s Elements Panel. To use it, inspect an Element using Chrome DevTools as you’d normally do and select the “Scroll-Triggered Animations” pane to see a visualization of the Scroll-Triggered Animations that are added to that element. The visualization is a live representation of the scroller, animated element, and – in case of a ViewTimeline – tracked subject: as you scroll in the document, the visualization and trigger active/inactive status light also update.

Use the top toolbar to switch between multiple animations _(if more than one)_. Also included in the top toolbar are an active/inactive status light indicator, the trigger name and actions, scroller name, timeline type, and progress numbers: total scroll progress, effect progress, actual scroll offset _(in pixels)_. Use the controls in the top-right corner of the visualization to set the scale factor. Typically you don’t need to set the scale factor, as the visualization automatically adapts itself to the available space.

At the bottom of the pane is a range editor for `timeline-trigger-activation-range` and `timeline-trigger-active-range` _(collapsible via the “Edit Values” toggle when vertical space is limited)_. The visualization shows indicators for both the activation range (blue) and active range (green): in case of a ScrollTimeline these are dashed lines on the scroller’s contents, and in case of a ViewTimeline these are shaded boxes representing the areas for the configured range values. Change the values live using the dropdowns and/or the inputs.

## FAQ

There are some known issues and questions that get asked regularly. Find these in the Issue list with the https://github.com/bramus/scroll-triggered-animations-debugger-extension/labels/FAQ label. Note that GitHub by default hides closed issues. To see the full list of FAQ items, use [this direct link](https://github.com/bramus/scroll-triggered-animations-debugger-extension/issues?q=label%3AFAQ+)

## Reporting problems / Filing feature requests

Please [file an issue](https://github.com/bramus/scroll-triggered-animations-debugger-extension/issues) if you want to report a problem or make a feature request. When reporting a problem, please add a link to a URL where I can reproduce the problem.

## License

This extension is closed source for the time being. This might change over time.
