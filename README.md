# NES ML

Simple markup language as enty point to learning HTML

It was originally designed for a one-hour web dev workshop for people with no prior coding experience.

## Concept
Several workshops were conducted using NES.css before NES ML was created. I found that getting used to the XML(HTML) syntax takes longer for people than the time available during a one-hour workshop. That's why NES ML was created to simplify the syntax while still producing for an appealing result.

### Key features
- Tag names based on common terms
- No attributes
- Minimal nesting required
- Lots of pre-defined styling
- Full structured page can be built only using simple tags

## Usage
Include the 

## Tags
The following tags are available
### `box`
Container with a black outline
```html
<box>
    Content
</box>
```
### `intro`
Same as `box` but all text is centered
```html
<intro>
    Content
</intro>
```
<img src="preview/intro.png" width="398">

### `box-title`
Headline of a `box` or `intro`
```html
<box>
    <box-title>That's me</box-title>
</box>
```
### `message`
Black text box with white text
```html
 <message>Thanks for dropping by, stranger!</message>
```
### `headline`
Headline
```html
<headline>Content</headline>
```
### Avatars
| Tag               | Result        |
| -------------     | ------------- |
| `<ash></ash>`     | <img src="preview/ash.png" width="84"> |
| `<mario></mario>` | Content Cell  |

## Compatibility
Tested on
- Chrome ✔
- Firefox ✔
- Safari ✔
- Edge ✔

## How it works
- Styling is based on [NES.css](https://nostalgic-css.github.io/NES.css/)
- The language takes advantage of HTML5's freedom to use custom tag names