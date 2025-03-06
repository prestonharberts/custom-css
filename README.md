# My Custom CSS

This is a place where I put various CSS changes I make to some applications, and how to apply them. One of my favorite things to do is find an app that is either based on the web or even a desktop app with an Inspect Element menu and tune it until it looks just right with my (subjective) taste.

## Firefox

First, I recommend installing the [CSS Override extension by swcolegrove](https://addons.mozilla.org/en-US/firefox/addon/css-override/?utm_source=addons.mozilla.org&utm_medium=referral&utm_content=search). This lets you save CSS snippets to the website and sync changes across your Firefox account.

Another extension I recommend is the [Progressive Web Apps extension by Filip S](https://addons.mozilla.org/en-US/firefox/addon/pwas-for-firefox/) that lets you save a website to your start menu and/or pin it to your taskbar. Even better is that you can apply CSS to the `userChrome.css` to hide the application titlebar, leaving you with just the contents of the website.

### Progressive Web Apps for Firefox userChrome.css

This file (at least on Linux) is kept at `~/.local/share/firefoxpwa/profiles/00000000000000000000000000/chrome/userChrome.css`. I suggest making all web apps using PWAs with the Default profile so you don't have to keep changing this CSS. To find the location of this folder on Windows or Mac, open `about:support` in your PWA, and look for "Profile Directory" under Application Basics. Make a new file `userChrome.css` inside the `chrome` folder, and paste this into it:

```css
#titlebar {
  visibility: collapse !important;
}

#TabsToolbar {
  visibility: collapse !important;
}
```

Make sure you're signed into Firefox and have it set up just the way you want it. Change the following in `about:config` to enable the `userChrome.css`:

```css
toolkit.legacyUserProfileCustomizations.stylesheets - true
```

The CSS for the following can be found in this repository's `css` folder.

### ChatGPT

`css/chatgpt.css`

<p align=center><img src="https://github.com/user-attachments/assets/3cff3cfb-f216-46ac-8228-797adb3a315c" width="768"></p>

<p align=center><img src="https://github.com/user-attachments/assets/ddad4d19-e793-47c5-8bca-496f6e38b67f" width="768"></p>

### Monkeytype

`css/monkeytype.css`

My custom settings can be found in this repository's `config/monkeytype.json`.

<p align=center><img src="https://github.com/user-attachments/assets/6c0f9e0c-2b47-4e16-b2cc-dd949fbaedb0" width="768"></p>

<p align=center><img src="https://github.com/user-attachments/assets/3ccdfaa8-96b3-478b-b031-675cd84a9ead" width="768"></p>

## Obsidian

All CSS (`obsidian-main.css`, `obsidian-plugins.css`, and `obsidian-bible.css`) can be imported as CSS snippets in your vault's `.obsidian/snippets` folder. I have limited dark mode support and all my CSS is meant to work with the Adwaita theme, which you can install through the Theme option in Obsidian's settings. `obsidian-plugins.css` changes the appearance of certain plugins that I make use of in Obsidian, and `obsidian-bible.css` is meant to be used with the Bible in markdown generated by my [BibleGateway-to-Obsidian](https://github.com/prestonharberts/biblegateway-to-obsidian) script, which the NET translation of the Bible is available to be downloaded from my project.

<p align=center><img src="https://github.com/user-attachments/assets/43d5fc2b-2cd1-4c9e-89c5-5d4c52e27ed7" width="768"></p>

<p align=center><img src="https://github.com/user-attachments/assets/7188781d-6890-4d4f-928b-78f30a973ca7" width="768"></p>

<p align=center><img src="https://github.com/user-attachments/assets/26d13ca1-6e0d-4078-8dab-fc4a79ca2744" width="768"></p>
