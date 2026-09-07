# What Is Browser Fingerprinting? (And How to Test Yours)

*This post contains affiliate links. If you sign up through them, I may earn a commission at no extra cost to you.*

---

Every website you visit can identify you without cookies, without your name, and without asking. The technique is **browser fingerprinting**, and if you manage multiple accounts, it's the single most important thing to understand — because it's how your accounts get linked together.

## What a fingerprint is made of

Your browser hands every site a bundle of technical details, just by rendering a page:

- **User agent** — browser name, version, and OS
- **Screen size and color depth** — your display's exact characteristics
- **Canvas and WebGL** — how *your* machine uniquely draws graphics (the loudest signal)
- **Installed fonts** — the specific font list on your device
- **Language, time zone, and locale**
- **Hardware details** — CPU cores, device memory, touch capability
- **Audio and media capabilities**

Any one of these is unremarkable. Combined, they produce a value that is — statistically — unique to you. In studies covering millions of browsers, the overwhelming majority of fingerprints are one-of-a-kind.

## Why cookies made this worse

Cookies can be deleted. Fingerprinting was built to be permanent — it works in private mode, survives cookie clears, and operates silently. That permanence is exactly why anti-tracking and multi-account work had to evolve past cookies.

## How to test your own fingerprint

Open one of the public fingerprint-test sites (search "browser fingerprint test" — several well-known ones exist). It will show you:

- your **fingerprint hash** — the unique ID derived from your setup
- **how unique** each parameter is
- which values stand out most

Try it in private mode and after clearing cookies — the hash barely changes. That's the whole problem in one experiment.

## The fingerprint problem for multi-account work

The failure mode that matters to account managers:

1. You log into account A in your normal browser.
2. You log into account B in a fresh Chrome profile — different cookies, fresh login.
3. **Both sessions present the same fingerprint.**

To the platform, that's two accounts used from the same computer. The cookies said "different people"; the fingerprint said "same person." The fingerprint wins. That's how legitimate operators get wrongly flagged for account association.

## What actually changes your fingerprint

Changing your user agent alone doesn't work — it creates a *contradiction* (claims to be a Mac, renders like a PC), and contradictions are themselves detectable. A real solution changes **all the parameters together, consistently**:

- a coherent device story (UA + screen + GPU + platform all agreeing)
- per-profile separation (no shared values across accounts)
- a matching IP (country, sometimes city)
- values that stay stable session after session

That's the job of an antidetect browser. RoxyBrowser exposes **160+ fingerprint parameters** per profile and keeps them consistent, on a Chromium kernel synced with official Google releases so the profile looks like a current, ordinary machine. There's a permanent free plan (2 profiles, no card) if you want to see your fingerprint change properly: [try RoxyBrowser free](https://mrait.ca/go/freebrowser).

## Test it yourself, end to end

The two-profile experiment takes ten minutes:

1. Create two RoxyBrowser profiles ([quick start guide](./how-to-use-roxybrowser.md)).
2. Open the same fingerprint test site in each.
3. Compare — different hash, different canvas/WebGL values, different story per profile.

That visible difference is the entire value of the tool category, demonstrated on one screen.

**Related:** [What is an antidetect browser?](./what-is-an-antidetect-browser.md) · [RoxyBrowser review](./roxybrowser-review-2026.md) · [Course Step 2: antidetect vs VPNs](./antidetect-course-explained.md)
