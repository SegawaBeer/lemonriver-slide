# Usage guide

English · [简体中文](../zh-CN/guide.md) · [Back to the home page](../../README.md)

The same guide is in the app, under "Usage guide" in the sidebar.

Slides in LemonRiver are written and changed by an AI agent, while you watch the result in the browser and adjust it by hand. Any agent works, as long as it can read and write files on your computer.

There are two ways to work. Pick the one that suits you, or mix them:

- **Talk to your agent**: type to it, and it creates the deck and changes each page. Best if you like typing and want the agent to do most of the work.
- **Edit in the interface**: change text, styles, images and page order in LemonRiver itself, and leave comments for the agent where you cannot. Best if you like working by hand and seeing every change.

Both ways start with “Prepare”.

## Prepare (once)

1. <strong>Get an agent.</strong>Use the one you already have; all it needs is to open a folder on your computer and read and write the files in it. Common ones:
   - Common elsewhere: Claude Code, Codex, Gemini CLI, Grok, Cursor, GitHub Copilot, OpenCode and others
   - Common in China: WorkBuddy, DuMate, DeepSeek Harness, Trae, 千问办公, 豆包, Kimi CLI and others
2. <strong>Let the agent work in the LemonRiver folder.</strong>If you installed LemonRiver with the installer, the folder is “Personal folder → LemonRiver”; if you set it up from the command line, it is the folder you created.
   - Agents that run in a terminal: go into that folder first, then start the agent.
   - Agents with a window: use their “Open folder” and pick this folder.
   - The folder already holds notes for the agent: how to write slides, how to handle comments, and how to know which page you are looking at. Most agents read them on their own; if yours does not seem to, tell it “read the AGENTS.md in this folder first”.
3. **Open LemonRiver in the browser** (click the lemon in the Dock or on the desktop) and put it side by side with the agent, so you can talk and watch at the same time.
4. **Let the agent see the page**: add an MCP server in the agent’s settings, with the command `node node_modules/@lemonriver/core/bin.js mcp` and the LemonRiver folder as its working directory. Claude Code offers to enable it when you open this folder.

How to install, sign in to, or pay for an agent is up to its own instructions; LemonRiver does not handle any of that.

## Way 1: talk to your agent

1. Open the agent and make sure it is in the LemonRiver folder.
2. **Create**: just say what you need, for example “Make a Q3 business review, about 10 pages, for the leadership team; here is the data: …”. The agent asks a few questions first. The finished deck appears on the home page; refresh if it does not.
3. **Change a page**: open that page in the browser and tell the agent “change this page: shorter title, bigger numbers”. The agent knows which page you are viewing. You can also name the page: “turn the bar chart on page 3 into a line chart”.
4. **Add, remove or reorder pages**: “add a page about risks after page 4”, “swap the last two pages”.
5. **Speaker notes**: “write about 150 words of notes for every page”. They go into each page’s “Speaker notes”, and the presenter view shows them while you present.
6. Other things you can say: “make the whole deck darker and simpler”, “check the typos and numbers that do not add up”, “lay out page 2 like this screenshot” (send the agent the screenshot).

## Way 2: edit in the interface

1. **Start from a deck**: have the agent write a first draft (way 1, step 2), import a package someone shared, or “Duplicate” a deck you already have on the home page. A new workspace comes with a short practice deck, so you can try every step below on it. For now you cannot add new text or images to a blank page.
2. **Change text**: double-click the text on the page and type.
3. **Change the look**: click to select, then use the “Format” panel on the right to change size, weight, colour, background, alignment, position and size. Hold Shift to select several; ⌘Z undoes.
4. **Swap an image**: select the image, click “Replace image”, pick one from your assets, and crop it if you like. Upload new images in “Assets” on the left first.
5. **Manage pages**: drag the thumbnails on the left to reorder; right-click to “Duplicate” or delete. Press B to open the “Story board” and see the whole structure and write notes for each page.
6. **Speaker notes**: write them right in “Speaker notes”.
7. **What the interface cannot do, leave a comment**: click “Comment”, click an element or drag a box, and write the change you want, such as “make this three cards” or “add a year-on-year table”. You can leave as many as you like. When you are done, tell the agent “apply comments” (in Claude Code you can also type `/apply-comments`); it goes through them one by one, and each comment disappears once it is done.

## Finish

- **Self-check**: in the “Story board”, click “Self-check” to look for type that is too small, content that runs off the page, text that crosses the edge, and missing speaker notes.
- **Present**: “Present” at the top right of the editor goes full screen; the presenter view shows the current page, the next page, the notes and a timer.
- **Export**: PDF, PPTX (the text stays editable) and a web page. Sharing and backups are in the sections below.

## Common questions

- **The agent says it is done, but the browser shows nothing**: check that the agent opened the LemonRiver folder, then refresh the home page.
- **What the agent wrote does not look like slides, or it edited the wrong files**: tell it “read the AGENTS.md in this folder first and follow its rules”.
- **I broke something**: ⌘Z undoes changes made in the interface; before a big change, “Duplicate” a deck on the home page as a spare; deleted decks stay in the trash for 30 days.
- **My comments did nothing**: comments are only notes until you tell the agent to “apply comments”.
