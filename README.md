# furling-legal

The public pages App Review requires for **Furling**: privacy policy, terms of
use, and a support page with a real address on it.

Published as a GitHub Pages site. Live at
<https://rokopavelic.github.io/furling-legal/>.

| Where it is used | URL |
|---|---|
| Privacy Policy — App Store Connect field *and* the in-app paywall link | `/privacy.html` |
| Terms of Use — in-app paywall link | `/terms.html` |
| Support URL — App Store Connect field | `/support.html` |
| Marketing / home | `/index.html` |

The app reads these from one module, `src/lib/legal.ts`, so no URL is ever
inlined in a component.

## Editing

**The source of truth is `legal/` in the private app repo**, not this one. Edit
there, then copy the five files across and push. Keeping the copy here editable
is how the sibling project's policy drifted out of sync with its app.

A privacy policy that describes an app that no longer exists is worse than none,
so any change to what the app sends, stores or charges for is a change to
`privacy.html` in the same breath.
