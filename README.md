# Lupulus

Lupulus<sup id="a1">[\[1\]](#f1)</sup> is my custom keyboard layout which is suited for writing texts in Czech, German and English languages, combined with programming and working in Terminal. It was made using [Ukelele](http://scripts.sil.org/cms/scripts/page.php?site_id=nrsi&id=ukelele) and is meant to be used with Mac keyboard having US English layout:

![](https://cdn.shopify.com/s/files/1/0810/3669/files/mac-us-english-keyboard_1024x1024.png?1871373995114389746)

## Installation

The keyboard layout is installed by moving it and its icon to `~/Library/Keyboard Layouts`.

## Disabling System Layouts

By default, there has to be at least one system keyboard layout activated in macOS. In order to disable all system keyboard layouts and to have only the custom one listed, further steps have to be performed.

1\. Duplicate the current keyboard layout preference file to a temporary location and open it for editing.

```bash
cp ~/Library/Preferences/com.apple.HIToolbox.plist /tmp
open /tmp/com.apple.HIToolbox.plist
```

2\. Manually remove the entries for system keyboard layouts listed under the key `AppleEnabledInputSources`.

3\. Copy the edited version of the preference file back to its original location:

```bash
cp /tmp/com.apple.HIToolbox.plist ~/Library/Preferences/
```

4\. Restart the computer.

## Attribution

The keyboard layout uses the icon “[Hops](https://thenounproject.com/term/hops/9254/)” by [The Crew at Fusionary](https://thenounproject.com/fusionary/) from the [Noun Project](thenounproject.com).

---

<a id="f1"></a>[1] *Humulus lupulus is the latin name for hops.* [↩](#a1)
