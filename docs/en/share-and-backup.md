# Sharing, backup and cloud drives

English · [简体中文](../zh-CN/share-and-backup.md) · [Back to the home page](../../README.md)

## Share a deck with someone

1. From the menu on a deck card on the home page, or at the top right of the editor, choose “Share”.
2. A PDF is attached by default, so the other person can read it without LemonRiver. Clear the tick if you do not need it; the package gets much smaller.
3. Choose “Create package” and wait while every page is drawn. A long deck takes ten seconds or more.
4. When it is done, choose “Show in Finder”. The zip is in the workspace’s “shared” folder; send it over WeChat, email or a cloud drive.

The other person sees three things: a PDF, a “how to open” note, and a “LemonRiver-files” folder. The note explains how to install LemonRiver.

**What travels**: the deck itself, the assets and theme it uses, and the chapters and notes in the story board.

**What stays here**: your conversations with the Agent and the settings on your computer.

## Open a package someone sent you

1. Open the LemonRiver home page.
2. Drop the zip onto the home page, or choose “Import” at the top right and pick it.
   - Safari unpacks downloaded zips by itself, leaving a folder. You can drag that whole folder onto the home page instead.
3. The confirmation shows a thumbnail of every page, the page count and the version it was made with. If it is the right one, choose “Import”.

> **Security notice**A deck is program code, and it runs on your computer once imported. Only import packages from people you trust. The preview before importing is only pictures; nothing runs.

**The same deck came back**: if you already have this deck (you sent it to a colleague and they sent back a changed copy), the confirmation tells you which pages changed, and you can choose:

- **“Keep both”**: both stay, and “imported” is added to the new one’s name.
- **“Replace”**: the new one replaces yours, and the old one goes to the trash for 30 days.

**Why an import fails**:

- **“This is not a LemonRiver package”**: the other person sent a different zip, or the download did not finish.
- **“A file in the package was changed or is missing”**: someone unpacked the zip and edited it, or the cloud download went wrong. Ask them to share it again.
- **“This package was made with a newer LemonRiver”**: update LemonRiver in Settings first, then import.

## Backup

A backup packs the whole workspace into one zip: every deck, asset, theme and folder, plus settings such as theme, language and Agent preferences.

1. Open “Settings → Backup”.
2. Choose a backup location. To send it to a cloud drive automatically, choose that drive’s sync folder (setup for each drive is below); to keep it on this computer, the default “LemonRiver 备份” folder is enough.
3. Turn on “Back up every day”: one backup a day while LemonRiver is open. You can also choose “Back up now” at any time.
4. “Keep the latest” decides how many backups stay; older ones are deleted. Only backups LemonRiver made are deleted; other files you put in the folder are never touched.

**What a backup leaves out**: your conversations with the Agent, the trash, packages you shared, and the Agent’s auto-approve switch (for safety you turn it on again on a new computer).

## Restore a backup, or move to a new computer

1. On the new computer, install LemonRiver first (download: https://github.com/SegawaBeer/lemonriver-slide/releases/latest ), make sure the cloud drive client is installed and signed in, and the backup file is downloaded to this computer.
2. Open “Settings → Backup”, choose “Restore from backup…”, pick one from the list, or choose “Choose another backup file…” to find it.
3. Tick the decks to restore and choose “Restore”.
   - A deck with the same name on this computer goes to the trash first, and stays recoverable for 30 days.
   - Decks on this computer that are not in the backup are left alone.
   - When an asset has the same name but different content, the copy on this computer is kept.

## Put backups on a cloud drive

**The cloud drive client does the uploading**: LemonRiver never signs in to your cloud account. It only writes backups into a folder on your computer. Install and sign in to the cloud drive’s desktop client first.

Cloud drive clients work in one of two ways:

- **With a sync folder**(the drives that give you a sync folder once their client is installed; each is covered below): files put in the folder upload by themselves. Choose that folder as the backup location; LemonRiver lists the ones it can find under “Change”.
- **With folder backup only**: let LemonRiver back up to the default “LemonRiver 备份” folder, then add that folder to the cloud drive client’s automatic backup.

The first time LemonRiver backs up into a cloud folder, macOS may ask whether to allow access to files managed by someone else. Choose “Allow”. If you chose “Don’t Allow”, turn it back on under “System Settings → Privacy & Security → Files and Folders”.

### iCloud Drive

1. Open “System Settings”, click your name at the top, then click “iCloud”.
2. Turn on “iCloud Drive” and make sure “Sync this Mac” is on.
3. Back in LemonRiver, open “Settings → Backup → Change” and choose “iCloud Drive”.
4. **Check that it uploaded**: in the Finder sidebar open “iCloud Drive → LemonRiver 备份”. When there is no cloud or progress icon beside the file, it is uploaded. You can also check on icloud.com.

- Free iCloud is only 5GB, and one backup can be a few hundred MB. If space runs out, lower “Keep the latest” or buy more iCloud storage.
- When restoring on a new computer, a cloud icon beside the backup means it is not downloaded yet: double-click it, wait for the download, then restore.

### Baidu Netdisk

Baidu Netdisk’s desktop client offers two ways; either works:

- <strong>Option 1: Sync Space.</strong>In the client, open “Sync Space” (同步空间) and follow the steps to make a local folder the sync folder (it is called “BaiduSyncdisk” by default). Then in LemonRiver “Settings → Backup → Change”, choose “Baidu Netdisk Sync Space”.
   - Note: Sync Space works both ways. A file you delete on this computer is deleted from the drive too, and when LemonRiver deletes an old backup, the copy on the drive goes with it.
- <strong>Option 2: folder backup.</strong>Keep LemonRiver backing up to the local “LemonRiver 备份” folder. In the Baidu Netdisk client find “Automatic backup” (自动备份), choose “Add backup folder” (添加备份文件夹), and pick that folder.
   - This goes one way: deleting an old backup on this computer leaves the copy on the drive, so clean it up there from time to time.
   - Free accounts have a monthly upload limit for automatic backup (the client says 10G a month). After that, wait for next month or upgrade.

**Check that it uploaded**: open the matching folder in Baidu Netdisk; the backup with the newest date means the upload finished.

### Tencent Weiyun

1. Install Tencent Weiyun’s desktop client and sign in.
2. Keep LemonRiver backing up to the local “LemonRiver 备份” folder.
3. If your Weiyun client offers “Automatic backup” or a sync folder, add this folder to it.
4. If it does not, then after a backup choose “Show in Finder” in LemonRiver and drag the newest backup zip into Weiyun to upload it.

- Weiyun’s free space is small; setting “Keep the latest” to 3 is a good idea.

### Dropbox

1. Install Dropbox’s desktop client and sign in; “Dropbox” appears in the Finder sidebar.
2. In LemonRiver “Settings → Backup → Change”, choose “Dropbox”.
3. **Check that it uploaded**: in Finder open “Dropbox → LemonRiver 备份”. A green tick beside the file means it is uploaded.

- When restoring on a new computer, a cloud icon beside the file means it is online only: double-click it, wait for the download, then restore.

### OneDrive

1. Install OneDrive (you can find it in the App Store) and sign in; “OneDrive” appears in the Finder sidebar.
2. In LemonRiver “Settings → Backup → Change”, choose “OneDrive”. Work and personal accounts are listed separately; pick yours.
3. **Check that it uploaded**: no cloud or progress icon beside the file means it is uploaded; you can also check on onedrive.com.

- When restoring on a new computer, the method above applies: if the file is online only, double-click to download it first.

### Nutstore

1. Install Nutstore’s desktop client and sign in. It comes with a “My Nutstore” sync folder.
2. In LemonRiver “Settings → Backup → Change”, choose “Nutstore · My Nutstore” (or another sync folder you made).
3. **Check that it uploaded**: in the Nutstore client, look at the folder’s sync status; when nothing is waiting to upload, it is done.

- Nutstore’s free plan has a monthly upload limit, so a big backup may only upload a few times a month.

### Other cloud drives

Any cloud drive whose client can upload a folder on this computer automatically will work:

- If it has a sync folder, choose “Choose another folder…” under “Change” and pick it.
- If not, use the default “LemonRiver 备份” folder and make the cloud client upload that folder automatically.

## Cloud drive questions

- <strong>The backup succeeded, but it is not on the drive.</strong>LemonRiver only writes into the folder; the cloud drive client does the uploading. Check that the client is running, signed in, and not paused.
- <strong>The drive is full.</strong>Lower “Keep the latest”, or clean up old backups on the drive. The size of the last backup is shown after “Last backup”.
- <strong>There are files like “conflicted copy”.</strong>That happens when two computers back up into the same folder. Give each computer its own backup folder, or leave automatic backup on only one computer.
- <strong>How do I restore on a new computer?</strong>See “Restore a backup, or move to a new computer” above. The key is letting the cloud drive download the backup to the new computer first.
- <strong>I do not want to use a cloud drive.</strong>The default “LemonRiver 备份” folder is in your home folder. You can also choose a folder on an external drive and plug it in before backing up.
