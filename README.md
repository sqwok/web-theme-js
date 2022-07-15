# web-theme-js
A function you can use to build a new theme for the Sqwok web app.

# the function.
Simply run this function inside the browser developer tools console.

```
const styles = {
  '--color-avatar-bg': '',
  '--color-avatar-text': '',
  '--color-background': '',
  '--color-border': '',
  '--color-button-bg': '',
  '--color-button-text': '',
  '--color-chat-bg': '',
  '--color-chat-border': '',
  '--color-chat-shadow': '',
  '--color-chat-text': '',
  '--color-chat-text-dim': '',
  '--color-danger': '',
  '--color-footer-bg': '',
  '--color-footer-text': '',
  '--color-footer-text-bright': '',
  '--color-header-bg': '',
  '--color-header-shadow': '',
  '--color-header-text': '',
  '--color-header-text-bright': '',
  '--color-link': '',
  '--color-logo': '',
  '--color-message-permalink': '',
  '--color-modal-dialog-bg': '',
  '--color-modal-overlay-bg': '',
  '--color-modal-text-dim': '',
  '--color-modal-text': '',
  '--color-popout-bg': '',
  '--color-popout-bg-inverse': '',
  '--color-popout-border': '',
  '--color-popout-shadow': '',
  '--color-popout-text': '',
  '--color-popout-text-inverse': '',
  '--color-popout-tooltip-bg': '',
  '--color-popout-tooltip-text': '',
  '--color-shadow': '',
  '--color-shadow-dim': '',
  '--color-text-bright': '',
  '--color-text-dim': '',
  '--color-text': '',
  '--color-user-select-bg': '',
  '--color-user-select-text': '',
  '--color-warn': '',
  '--color-md-blockquote-border': '',
  '--color-md-blockquote-text': '',
  '--color-md-code-bg': '',
  '--color-md-code-text': '',
  '--color-md-link-text': '',
  '--color-md-list-text': '',
  '--color-md-mention-bg': '',
  '--color-md-mention-text': '',
  '--color-md-pre-bg': '',
  '--color-md-pre-border': '',
  '--color-md-pre-mention-bg': '',
  '--color-md-pre-mention-text': '',
  '--color-md-pre-text': '',
  '--shadow-header': '',
  '--shadow-footer': '',
  '--shadow-modal': '',
};
const el = document.documentElement;

for (const style in styles) {
  el.style.setProperty(style, styles[style] || undefined);
}
```

For example to change only the core colors of the site:
```
  '--color-background': 'blue',
  '--color-border': 'hsl(220deg 50% 10%)',
  '--color-shadow': 'green',
  '--color-text': '#be5ae4',
  '--color-text-dim': 'grey',
```

To experiment with new theme changes, simply add valid css colors to any of the properties and run the function again.

Shadow properties take the form of css `box-shadow` e.g. `1px 1px 2px blue`

You can refresh the page to reset.

If you come up with a theme you think other people would enjoy, let us know by creating a post about it https://sqwok.im or email it to user-themes@sqwok.im and we will consider adding it to the site as an available option.
