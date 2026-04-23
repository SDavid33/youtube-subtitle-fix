# YouTube Subtitle Fix - Smart Line-Wrapping - Better Readability

Improves how YouTube subtitles look and behave with smarter line wrapping, better readability, optional per-line background boxes, and cleaner handling of translator notes.

## Files

- `tampermonkey.user.js` - Tampermonkey userscript version
- `enhancer-for-youtube.js` - script version for Enhancer for YouTube

## What it does

- Changes subtitle text color
- Changes subtitle size in normal mode and fullscreen mode
- Adjusts subtitle background color and opacity
- Supports one shared background box or per-line background boxes
- Keeps subtitles centered
- Lets you move subtitles higher on the screen
- Adds text shadow for better readability
- Wraps long lines automatically
- Tries to keep line breaks more natural and balanced
- Prefers two-line subtitles when possible
- Allows three lines only when needed
- Keeps translator notes in square brackets together
- Preserves a two-line layout when a translator note is already on its own line

## Main settings

- `textColor` - subtitle text color
- `backgroundColor` - subtitle background color as RGB values
- `backgroundOpacity` - background transparency from `0` to `1`
- `fontSizeNormal` - subtitle size in normal mode
- `fontSizeFullscreen` - subtitle size in fullscreen mode
- `lineHeight` - spacing between subtitle lines
- `maxWidthPercent` - maximum subtitle width relative to the video width
- `enableAutoLineBreaks` - turns smart wrapping on or off
- `maxCharsPerLine` - target line length for smart wrapping
- `perLineBackground` - separate background per line or one shared box
- `paddingY` / `paddingX` - inner spacing inside the background box
- `borderRadius` - roundness of subtitle background corners
- `offsetNormal` / `offsetFullscreen` - subtitle height from the bottom
- `extraPerLine` - extra upward offset for multi-line subtitles
- `textShadow` - subtitle text shadow

## Safe starter preset

```js
lineHeight: 1.20,
maxWidthPercent: 78,
enableAutoLineBreaks: true,
maxCharsPerLine: 44,
perLineBackground: true,
```

## Install

### Tampermonkey

1. Install the Tampermonkey browser extension.
2. Create a new script.
3. Replace the template with the contents of `tampermonkey.user.js`.
4. Save and open any YouTube video.

### Enhancer for YouTube

1. Open Enhancer for YouTube settings.
2. Find the custom script section.
3. Paste in the contents of `enhancer-for-youtube.js`.
4. Save and reload YouTube.

## Notes

- This script only changes how subtitles are displayed.
- It does not modify the subtitle file itself.
- Final behavior can still depend on how YouTube renders captions internally.
- Best results usually come from adjusting `maxWidthPercent`, `maxCharsPerLine`, and `lineHeight` together.

## Screenshots

<img width="1894" height="1030" alt="image" src="https://github.com/user-attachments/assets/77635209-86fd-448c-b322-f5e034f40398" />




<img width="1907" height="1052" alt="image" src="https://github.com/user-attachments/assets/eac8d517-537e-4f31-862d-69f4841ff0b9" />


## Greasy Fork

[Greasy Fork script page](https://greasyfork.org/en/scripts/575046-youtube-subtitle-fix-smart-line-wrapping-better-readability)
