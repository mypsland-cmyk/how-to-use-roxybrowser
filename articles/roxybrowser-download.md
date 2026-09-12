# RoxyBrowser Download & Install Guide (Windows, macOS, Linux)

*This post contains affiliate links. If you sign up through them, I may earn a commission at no extra cost to you.*

---

Looking for the RoxyBrowser download? Here's the safe path — official source, platform-specific steps, first-run setup, and the two-minute checks that confirm you installed the real thing.

## Step 1: Create your account first

RoxyBrowser's download lives behind a (free) account — which is also how you get the [permanent free plan](https://mrait.ca/go/freebrowser): 2 profiles, no credit card, no expiry. Sign up at **[mrait.ca/go/freebrowser](https://mrait.ca/go/freebrowser)** and confirm your email. The download links for all platforms are in your account dashboard.

## Step 2: Download for your OS

From the dashboard, pick your platform:

- **Windows** — installer `.exe`, supports Windows 10/11 (a VM works too — see the [Windows VM course step](./antidetect-course-windows-vm.md))
- **macOS** — `.dmg`, drag to Applications as usual
- **Linux** — package for mainstream distributions

Only ever download from the official site you reached through your own sign-up — antidetect browsers are impersonated by phishing sites precisely because people store business logins in them. If a search result offers you a "RoxyBrowser crack" or a mirror download, that's malware, full stop.

## Step 3: Install

It installs like any normal desktop application — no special drivers, no kernel-level components:

- **Windows:** run the installer, follow the wizard, launch from the Start menu
- **macOS:** open the `.dmg`, drag RoxyBrowser into Applications, first launch may ask you to confirm it in Gatekeeper (right-click → Open)
- **Linux:** install the package with your distribution's package manager, launch from the menu

## Step 4: First-run setup (5 minutes)

1. **Log in** with the account from Step 1.
2. **Create your first profile** — the defaults are sensible. Name it for its job (`ClientA-Instagram`, `Store-US`).
3. **Attach a proxy if you have one** — profile settings → proxy → host/port/user/pass → *Check*. No proxy yet? RoxyIP is integrated, and [Step 1 of the course](./antidetect-course-free-proxy.md) covers testing one properly.
4. **Open the profile and log into your first account.** Sessions persist between uses — closing a profile is like closing a laptop, not logging out.

The full tour of what you just installed — dashboard, profiles, synchronizer, API — is in the [complete walkthrough](./how-to-use-roxybrowser-walkthrough.md).

## Step 5: Verify it's the real RoxyBrowser

Two quick checks:

- **Kernel check:** from inside a profile, confirm the browser identifies with a current Chromium version — RoxyBrowser keeps its kernel synced with official Google releases.
- **Fingerprint check:** open a public fingerprint test site inside the profile — you should see a coherent, ordinary device story. Compare it with a second profile ([quick-start guide](./how-to-use-roxybrowser.md)) and the two should tell different stories.

## System requirements (practical)

Any machine that runs Chrome comfortably runs RoxyBrowser: 4 GB RAM minimum (8 GB for many concurrent profiles), a normal dual-core CPU, and a few hundred MB of disk per handful of profiles. It's a desktop app for Windows, macOS, and Linux — there's no mobile version.

## Troubleshooting quick hits

- **Download won't start** — check your account dashboard for the correct regional link, and disable download-intercepting browser extensions on the page.
- **macOS blocks first launch** — right-click → Open (Gatekeeper one-time confirmation for newly notarized apps).
- **Profiles closed unexpectedly** — sessions persist; just reopen the profile. Cookies and logins survive.

**Related:** [How to use RoxyBrowser (10-minute setup)](./how-to-use-roxybrowser.md) · [RoxyBrowser free plan explained](./roxybrowser-pricing-and-free-plan.md) · [Is RoxyBrowser safe?](./is-roxybrowser-safe.md)
