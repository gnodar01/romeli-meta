# Privacy Policy for romeli

**Last updated:** October 25, 2026

## Overview

This Extension is a browser extension. This privacy policy describes how user data is handled.

## Data Collection and Use

This Extension does **not** collect, transmit, or share any personal data. All data (user preferences and activity logs) are stored locally on user devices using the browser's built-in storage API and is never sent to any external server or third party.

## Permissions

This extension uses the following browser permissions:

* *bookmarks*: romeli is a bookmark manager: its single purpose is to browse, organize and edit the user's own bookmarks. It reads the bookmark tree to display folders as hierarchical tags, and creates, moves, renames and removes bookmarks and folders only when the user asks (adding or removing a tag, renaming a tag, deleting an item, undo/redo). Bookmarks are never sent anywhere; the browser's own sync remains the only place they are stored.
* *storage*: romeli stores the extension's own settings: preferences, keyboard bindings, the color theme, and the user's custom tag order for bookmarks. These use chrome.storage.sync so they follow the user across their signed-in browsers. chrome.storage.session holds the IDs of romeli's open windows, so a shortcut focuses the existing window instead of opening a second one. No browsing data or personal information is stored, and nothing is sent to any server.
* *activeTab*: romeli uses this only when the user explicitly invokes it, through its keyboard shortcut or toolbar button. When the user presses "bookmark this page", romeli reads the current tab's URL and title to pre-fill the new bookmark. When the user opens romeli, it reads the current tab's URL to jump to that page's bookmark if one exists. romeli never reads other tabs, page contents or browsing history, and requests no host permissions.
* *favicon*: romeli shows each bookmark's site icon next to it in the list, so the user can recognize bookmarks at a glance. Icons come from Chrome's local favicon cache (`chrome-extension://…/_favicon/`), so no network requests are made to the bookmarked sites or any third party.
* *clipboardWrite*: romeli lets the user copy a bookmark's URL, title, or tag path to the clipboard with a keyboard command, and copy their keymap or theme as JSON from the options page to back it up or share it. romeli only writes to the clipboard in direct response to the user's action and never reads the clipboard.

These permissions are used solely for the extension's core functionality and do not involve collecting or transmitting user data.

romeli performs no remote code execution. All JavaScript is bundled in the extension package at build time (Svelte compiled with Vite). The extension loads no external scripts, uses no eval() or new Function(), and makes no network requests. Its only requests load its own packaged files.

## Third-Party Services

This Extension does not use any third-party analytics, tracking, or advertising services.

## Data Storage

All extension data is stored locally on your device using the chrome.storage API. You can clear this data at any time by uninstalling the extension.

## Changes to This Policy

If changes are made to this privacy policy, the "Last updated" date above will be updated.

## Contact

If you have questions about this privacy policy, please open an issue on the romeli's GitHub page.
