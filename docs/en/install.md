# Install

English · [简体中文](../zh-CN/install.md) · [Back to the home page](../../README.md)

## Mac installer (recommended)

No Node.js and no terminal needed. It runs on Apple silicon Macs (M1 and later) with macOS 11 or newer.

1. Open the [latest release](https://github.com/SegawaBeer/lemonriver-slide/releases/latest) and download `LemonRiver-<version>-arm64.dmg` from "Assets" at the bottom of the page.
2. Double-click the downloaded file and drag LemonRiver into Applications in the window that opens.
3. Open the Applications folder and double-click LemonRiver. **Don't open it straight from the disk image window**; drag it into Applications first.
4. macOS blocks it the first time, because the installer is not notarized by Apple:
   1. Click "Done" in the message.
   2. Open System Settings → Privacy & Security, scroll to the Security section and click "Open Anyway".
   3. Enter your login password. It opens normally from then on.
5. The first launch takes a dozen seconds or so to set up the workspace, then your browser opens on the LemonRiver usage guide.

Once it is installed:

- Your decks live in your home folder under LemonRiver; that is the folder to open in your agent (see the [usage guide](guide.md)).
- The lemon in the Dock and on the desktop opens LemonRiver in your browser.
- When a new version comes out the app tells you; click "Update now". You don't need to download the installer again.

## Start a workspace from the command line

With Node.js 20.19+ or 22.12+ installed you can make a workspace yourself, on Windows and Linux too:

```bash
npx @lemonriver/cli init my-slide --use-pnpm
cd my-slide
pnpm dev
```

init installs the dependencies as well (npm, pnpm, yarn and bun all work; swap `--use-pnpm` for `--use-npm` and so on). Open the address the terminal shows and carry on in the browser.

## Common problems

- **"Drag LemonRiver into Applications first, then open it from there"**: you opened it from the disk image. Drag it into Applications and open it from there.
- **No "Open Anyway" button in System Settings**: open LemonRiver once so macOS blocks it; the button only appears after that.
- **The page doesn't open in the browser**: click the lemon in the Dock again. If it still fails, open an [issue](https://github.com/SegawaBeer/lemonriver-slide/issues) with the message you see.
