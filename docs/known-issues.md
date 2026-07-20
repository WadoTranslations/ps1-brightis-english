# Known issues

A quick check here before you file a report saves us both time. If what you
found is not on this list, please do report it.

## Intentional, not bugs

- **The default hero name is "Alted."** You can rename him at the name-entry
  prompt. Lowercase letters live in the slots where the voiced kana used to
  be, which is why the on-screen keyboard looks the way it does.
- **Old Japanese save files keep their Japanese location names.** The name is
  baked into the save when you create it. Saves you make in the English patch
  record English location names; ones carried over from a Japanese playthrough
  keep what they had.
- **Some item strings go past the edge of the inventory.** These particular item
  addresses are referenced elsewhere in the game and truncating them would have
  caused issues.
- **Pocketstation instructions on tavern, store, and dojo posters are untranslated.** 
  For some reason I couldn't find these text addresses anywhere. They might be baked
  into a movie file? Leaving it for a future update.

## Minor

- A few of the longest lines sit close to the right edge of the text box. If
  you ever see one actually cut off or overflowing, that is a real bug, so
  please send a screenshot.

If you hit anything else, [open an issue](../../issues/new/choose).
