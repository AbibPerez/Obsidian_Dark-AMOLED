## Borders
|Variable|Default value|
|---|---|
|`--border-width`|`1px`|

## Colors

## Base colors

The base colors is a neutral color palette ranging from light to dark. These values should typically only be defined by themes.

|Variable|Default value (light mode)|Default value (dark mode)|
|---|---|---|
|`--color-base-00`|`#ffffff`|`#1c1c1c`|
|`--color-base-05`|`#fcfcfc`|`#212121`|
|`--color-base-10`|`#fafafa`|`#232323`|
|`--color-base-20`|`#f6f6f6`|`#282828`|
|`--color-base-25`|`#efefef`|`#2e2e2e`|
|`--color-base-30`|`#e4e4e4`|`#333333`|
|`--color-base-35`|`#dadada`|`#3f3f3f`|
|`--color-base-40`|`#bdbdbd`|`#555555`|
|`--color-base-50`|`#ababab`|`#666666`|
|`--color-base-60`|`#707070`|`#999999`|
|`--color-base-70`|`#5c5c5c`|`#b3b3b3`|
|`--color-base-100`|`#222222`|`#dadada`|
### Accent color

The accent color is used to draw attention to interactive elements, such as links and primary buttons, and can be overridden by the user under **Settings → Appearance** in the Obsidian app.

| Variable     | Default value | Description       |
| ------------ | ------------- | ----------------- |
| `--accent-h` | `258`         | Accent hue        |
| `--accent-s` | `88%`         | Accent saturation |
| `--accent-l` | `66%`         | Accent lightness  |

`--accent-h`, `--accent-s`, and `--accent-l` combine into the following accent color variables:

| Variable           | Description                                                      |
| ------------------ | ---------------------------------------------------------------- |
| `--color-accent`   | The accent color                                                 |
| `--color-accent-1` | A shifted accent shade, used for hover and active states         |
| `--color-accent-2` | A further-shifted accent shade, used for hover and active states |
### Extended colors

Extended color variables define the broader range of colors used for status messages (errors, warnings, success), callouts, syntax highlighting, graph nodes, and Canvas elements.

Each extended color has an additional RGB variable with a `-rgb` suffix that you can use to create colors with opacity, using the `rgba` function.

For example, the following snippet uses the default variable to set the text color, and the RGB variable to set a background color to red with 20% opacity.

```css
color: var(--color-red);
background-color: rgba(var(--color-red-rgb), 0.2);
```

| Variable             | Default value (light mode) | Default value (dark mode) |
| -------------------- | -------------------------- | ------------------------- |
| `--color-red`        | `#e93147`                  | `#fb464c`                 |
| `--color-orange`     | `#ec7500`                  | `#e9973f`                 |
| `--color-yellow`     | `#e0ac00`                  | `#e0de71`                 |
| `--color-green`      | `#08b94e`                  | `#44cf6e`                 |
| `--color-cyan`       | `#00bfbc`                  | `#53dfdd`                 |
| `--color-blue`       | `#086ddd`                  | `#027aff`                 |
| `--color-purple`     | `#7852ee`                  | `#a882ff`                 |
| `--color-pink`       | `#d53984`                  | `#fa99cd`                 |
### Black and white

Black and white colors let you create masks with opacity.

|Variable|Default value (light mode)|Default value (dark mode)|
|---|---|---|
|`--mono-0`|`white`|`black`|
|`--mono-100`|`black`|`white`|
### Semantic colors

Semantic colors are derived from the base color palette based on their intended use.

#### Surface colors

Primary background

Alt. primary background

Secondary background

Alt. secondary background

|Variable|Description|
|---|---|
|`--background-primary`|Primary background|
|`--background-primary-alt`|Background for surfaces on top of primary background|
|`--background-secondary`|Secondary background|
|`--background-secondary-alt`|Background for surfaces on top of secondary background|
|`--background-modifier-hover`|Hovered elements|
|`--background-modifier-active-hover`|Active hovered elements|
|`--background-modifier-border`|Border color|
|`--background-modifier-border-hover`|Border color (hover)|
|`--background-modifier-border-focus`|Border color (focus)|
|`--background-modifier-error-rgb`|Error background, RGB value|
|`--background-modifier-error`|Error background|
|`--background-modifier-error-hover`|Error background (hover)|
|`--background-modifier-success-rgb`|Success background, RGB value|
|`--background-modifier-success`|Success background|
|`--background-modifier-message`|Messages background|
|`--background-modifier-form-field`|Form field background|

#### Interactive colors

|Variable|Description|
|---|---|
|`--interactive-normal`|Background for standard interactive elements|
|`--interactive-hover`|Background for standard interactive elements (hover)|
|`--interactive-accent`|Background for accented interactive elements|
|`--interactive-accent-hsl`|Background for accented interactive elements in HSL|
|`--interactive-accent-hover`|Background for accented interactive elements (hover)|

### Text colors

#### Text foreground colors

|Variable|Description|
|---|---|
|`--text-normal`|Normal text|
|`--text-muted`|Muted text|
|`--text-faint`|Faint text|
|`--text-on-accent`|Text on accent background when accent is dark|
|`--text-on-accent-inverted`|Text on accent background when accent is light|
|`--text-success`|Success text|
|`--text-warning`|Warning text|
|`--text-error`|Error text|
|`--text-accent`|Accent text|
|`--text-accent-hover`|Accent text (hover)|

#### Text background colors

|Variable|Description|
|---|---|
|`--text-selection`|Selected text background|
|`--text-highlight-bg`|Highlighted text background|

#### Caret color

Defines the color of the caret, the blinking text entry cursor.

|Variable|Description|
|---|---|
|`--caret-color`|Caret color|
## Cursor
|Variable|Default value|Description|
|---|---|---|
|`--cursor`|`default`|Cursor for interactive elements|
|`--cursor-link`|`pointer`|Cursor for links|

## Icons

|Variable|Description|
|---|---|
|`--icon-size`|Shorthand for icon width and length|
|`--icon-stroke`|Shorthand for icon stroke width|
|`--icon-color`|Icon color|
|`--icon-color-hover`|Icon color (hovered)|
|`--icon-color-active`|Icon color (active)|
|`--icon-color-focused`|Icon color (focused)|
|`--icon-opacity`|Icon opacity|
|`--icon-opacity-hover`|Icon opacity (hovered)|
|`--icon-opacity-active`|Icon opacity (active)|
|`--clickable-icon-radius`|Clickable icon button radius|

### Icon sizes

| Variable                 | Default value |
| ------------------------ | ------------- |
| `--icon-xs`              | `14px`        |
| `--icon-s`               | `16px`        |
| `--icon-m`               | `18px`        |
| `--icon-l`               | `18px`        |
| `--icon-xl`              | `32px`        |
| `--icon-xs-stroke-width` | `2px`         |
| `--icon-s-stroke-width`  | `2px`         |
| `--icon-m-stroke-width`  | `1.75px`      |
| `--icon-l-stroke-width`  | `1.75px`      |
| `--icon-xl-stroke-width` | `1.25px`      |
## Layers
|Variable|Default value|
|---|---|
|`--layer-cover`|`5`|
|`--layer-sidedock`|`10`|
|`--layer-status-bar`|`15`|
|`--layer-popover`|`30`|
|`--layer-slides`|`45`|
|`--layer-modal`|`50`|
|`--layer-notice`|`60`|
|`--layer-menu`|`65`|
|`--layer-tooltip`|`70`|
|`--layer-dragged-item`|`80`|

## Radiuses

|Variable|Default value|
|---|---|
|`--radius-s`|`4px`|
|`--radius-m`|`8px`|
|`--radius-l`|`12px`|
|`--radius-xl`|`16px`|
## Spacing

|Variable|Default value|
|---|---|
|`--size-2-1`|`2px`|
|`--size-2-2`|`4px`|
|`--size-2-3`|`6px`|
|`--size-4-1`|`4px`|
|`--size-4-2`|`8px`|
|`--size-4-3`|`12px`|
|`--size-4-4`|`16px`|
|`--size-4-5`|`20px`|
|`--size-4-6`|`24px`|
|`--size-4-8`|`32px`|
|`--size-4-9`|`36px`|
|`--size-4-12`|`48px`|
|`--size-4-16`|`64px`|
|`--size-4-18`|`72px`|
## Typography

### Fonts

|Variable|Description|
|---|---|
|`--font-interface-theme`|Font used for UI elements|
|`--font-text-theme`|Font used for text in the editor|
|`--font-monospace-theme`|Font used for monospaced content such as code blocks and inline code|

#### Font size

Obsidian uses both relative and fixed font sizes depending on the context.

- Use `--font-*` (relative) variables in the editor.
- Use `--font-ui-*` (fixed) variables for UI elements.

|Variable|Default value|Description|
|---|---|---|
|`--font-text-size`|`16px`|Editor font size. Defined by the user under Appearance settings.|
|`--font-smallest`|`0.8em`||
|`--font-smaller`|`0.875em`||
|`--font-small`|`0.933em`||
|`--font-ui-smaller`|`12px`||
|`--font-ui-small`|`13px`||
|`--font-ui-medium`|`15px`||
|`--font-ui-large`|`20px`||

#### Font weight

|Variable|Default value|
|---|---|
|`--font-thin`|`100`|
|`--font-extralight`|`200`|
|`--font-light`|`300`|
|`--font-normal`|`400`|
|`--font-medium`|`500`|
|`--font-semibold`|`600`|
|`--font-bold`|`700`|
|`--font-extrabold`|`800`|
|`--font-black`|`900`|

#### Text formatting

As of Obsidian 1.6 `--bold-modifier` is the recommended way to change the weight of bolded text. The bold modifier value stacks on top of other font weights. This allows text which may already be bolded to have an even heavier weight, e.g. `## Bold **bolder**`. Recommended values for `--bold-modifier` are between 100 and 300.

|Variable|Description|
|---|---|
|`--font-weight`|Regular text weight|
|`--bold-modifier`|Added weight for bolded text|
|`--bold-weight`|Bold text font weight|
|`--bold-color`|Bold text color|
|`--italic-color`|Italic text color|

#### Line heights

|Variable|Default value|Description|
|---|---|---|
|`--line-height-normal`|`1.5`|Default line height|
|`--line-height-tight`|`1.3`|Used in search results, tree items, tooltips, and other smaller spaces|

#### Paragraph spacing

|Variable|Description|
|---|---|
|`--heading-spacing`|Spacing above headings|
|`--p-spacing`|Spacing between paragraphs|
