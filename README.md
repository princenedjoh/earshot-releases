# Earshot

Meeting notes, without the bot. Earshot records a meeting from your Mac itself, so nothing joins the call. It turns speech into text on the device, works out who said what, and writes notes with decisions and action items.

This repository holds downloads only. The app is in early beta.

## Download

Get the newest build from [Releases](https://github.com/princenedjoh/earshot-releases/releases).

| Your Mac | File |
|---|---|
| Apple silicon (M1 or newer) | `Earshot-<version>-mac-apple-silicon.zip` |
| Intel | `Earshot-<version>-mac-intel.zip` |

Requires macOS 14.4 or later.

## Opening it the first time

This beta is not signed with an Apple Developer ID, so macOS warns before opening it.

1. Unzip, then drag **Earshot** into Applications.
2. Double-click it. macOS says it could not verify the app. Click **Done**.
3. Open **System Settings → Privacy & Security**, scroll to the message about Earshot, and click **Open Anyway**.

If macOS says the app is damaged, run this in Terminal and open it again:

```bash
xattr -dr com.apple.quarantine /Applications/Earshot.app
```

## Docs

Setup, guides and known limits: https://www.nedjoh.com/docs/earshot

## Privacy

Audio is transcribed on your Mac and is never uploaded. Recordings, transcripts and voice fingerprints stay in Earshot's local folder. If you connect a cloud AI model for notes, the meeting's text is sent to that provider.

## Feedback

Open an [issue](https://github.com/princenedjoh/earshot-releases/issues) with what happened and your macOS version.
