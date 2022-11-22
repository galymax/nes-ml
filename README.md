# NES ML

Simple markup language as enty point to learning HTML

▶️ [Preview](https://galymax.github.io/nes-ml/)  
⌨️ [Try it](https://codepen.io/maximDCI/pen/rNKLBgv)

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
- font
- CSS
- JS 
in the `head` of your HTML document

```html
<link href="https://fonts.googleapis.com/css?family=Press+Start+2P" rel="stylesheet">
<link rel="stylesheet" href="./css/styles.css">
<script src="./js/nes-ml.js"></script>
```

- Use the NES ML tags to add content to the page

## Tags
The following tags are available
### `intro`
Same as `box` but all text is centered
```html
<intro>
    Content
</intro>
```
<img src="preview/intro.png" width="456">

### `box`
Container with a black outline
```html
<box>
    Content
</box>
```
<img src="preview/box.png" width="456">

### `box-title`
Title of a `box` or `intro`
```html
<box>
    <box-title>That's me</box-title>
</box>
```
<img src="preview/box-title.png" width="456">

### `message`
Black text box with white text
```html
 <message>Thanks for dropping by, stranger!</message>
```
<img src="preview/message.png" width="376">

### `headline`
Big headline
```html
<headline>Content</headline>
```
<img src="preview/headline.png" width="384">

### `bubble`
Speech bubble
```html
<bubble>Content</bubble>
```
<img src="preview/bubble.png" width="368">

### Avatars
| Tag               | Result        |
| -------------     | ------------- |
| `<ash></ash>`     | <img src="preview/ash.png" width="84"> |
| `<mario></mario>` | <img src="preview/mario.png" width="90"> |
| `<pokeball></pokeball>` | <img src="preview/pokeball.png" width="90"> |
| `<bulbasaur></bulbasaur>` | <img src="preview/bulbasaur.png" width="126"> |
| `<charmander></charmander>` | <img src="preview/charmander.png" width="132"> |
| `<squirtle></squirtle>` | <img src="preview/squirtle.png" width="132"> |
| `<kirby></kirby>` | <img src="preview/kirby.png" width="102"> |

### Social Media Links
- The url of the link goes between opening and closing tag
- For `twitter`, `whatsapp`, `gmail` and `github` only the handle/email address/phone number needs to be specified, the rest of the url is constructed automatically.

| Tag               | Result        |
| -------------     | ------------- |
| `<twitter>@davidsinclair</twitter>`     | <img src="preview/twitter.png" width="64"> |
| `<whatsapp>+49123456789</whatsapp>` | <img src="preview/whatsapp.png" width="64">  |
| `<github>@galymax</github>` | <img src="preview/github.png" width="64">  |
| `<linkedin>https://www.linkedin.com/in/maxim-werkhowski-b990611bb</linkedin>` | <img src="preview/linkedin.png" width="64">  |
| `<facebook>[profile url]</facebook>` | <img src="preview/facebook.png" width="64">  |
| `<instagram>[feed url]</instagram>` | <img src="preview/instagram.png" width="64">  |
| `<gmail>mail@email.com</gmail>` | <img src="preview/gmail.png" width="64">  |
| `<youtube>[channel url]</youtube>` | <img src="preview/youtube.png" width="64">  |
| `<twitch>[profile url]</twitch>` | <img src="preview/twitch.png" width="64">  |
| `<reddit>[profile url]</reddit>` | <img src="preview/reddit.png" width="64">  |

### `progress-[0-100]`
Progress bar with title
- `progress-` tags exist in variants from `<progress-0>` to `<progress-100>` in steps of `1`
```html
<progress-95>JavaScript</progress-95>
```
<img src="preview/progress.png" width="388">

## Compatibility
Tested on
- Chrome ✔
- Firefox ✔
- Safari ✔
- Edge ✔

## How it works
- Styling is based on [NES.css](https://nostalgic-css.github.io/NES.css/)
- The language takes advantage of HTML5's freedom to use custom tag names