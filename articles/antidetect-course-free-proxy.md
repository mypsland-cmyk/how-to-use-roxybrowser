# Antidetect Browser Course, Step 1: How to Get a Free Proxy (and Test It Properly)

> **Meta title:** How to Get a Free Proxy for an Antidetect Browser (Step 1)
> **Meta description:** Antidetect Browser Course Step 1 — what proxies do in profile-based workflows, how to get started with a free trial, and how to test reliability, speed, and geo-targeting.
> **Suggested slug:** `antidetect-browser-course-free-proxy`

*This post contains affiliate links. If you sign up through them, I may earn a commission at no extra cost to you.*

**📺 Watch the video version:**

[![Antidetect Browser Course: How to Get Free Proxy (Step 1)](https://img.youtube.com/vi/8UHSmgzVONw/hqdefault.jpg)](https://www.youtube.com/watch?v=8UHSmgzVONw&list=PLxY412qgkijKLUO1Gplz2q0MyCQC59Vnt)

---

This is Step 1 of my free antidetect browser course, and it starts where every good multi-account setup starts: **the proxy layer**. The browser handles fingerprints; the proxy handles where you appear to be. Get this layer wrong and nothing else matters.

## What a proxy actually does in a profile workflow

Every profile in an antidetect browser should present two things to a website: a plausible device (the fingerprint) and a plausible location (the IP). The proxy supplies the IP. Without it, ten profiles all share your home IP — and one shared IP undoes ten perfect fingerprints.

The rule of the course: **one profile, one IP, held stable.** An account that logs in from a different country every Tuesday looks wrong no matter how good its fingerprint is.

## What kinds of proxies exist (and which to start with)

- **Residential** — IPs from real consumer ISPs. The practical default for social, marketplace, and ad work.
- **Mobile** — IPs from carrier networks, shared naturally by many real users. Higher trust, higher cost.
- **Datacenter** — cheap and fast, but easily flagged for sensitive platforms. Fine for QA and testing.

## How to start free (the smart way)

Instead of hunting unreliable free proxy lists (which are frequently dead, slow, or worse — compromised), start with a **free trial from a reputable proxy provider**. A trial gives you real IPs long enough to answer the only question that matters: *are these IPs good enough for your actual accounts?*

RoxyBrowser makes this easy two ways: the [free plan](https://mrait.ca/go/freebrowser) includes integration with its own **RoxyIP** proxy pool, and the browser accepts any third-party proxy you already have.

## The 4-point proxy test

Before committing any IP to a real account, run this checklist from inside the profile:

1. **Geolocation** — does the exit IP resolve to the country/city you chose? Check an IP-lookup site from the profile.
2. **Speed** — load a heavy page or run a quick speed test. Painfully slow IPs get accounts abandoned mid-session.
3. **Stability** — reconnect a few times over a day. Does the IP hold, or rotate out from under your session?
4. **Cleanliness** — check the IP against blocklist/detection checkers. An IP already burned by someone else's abuse inherits their reputation.

An IP that passes all four is worth attaching to an account and keeping.

## Setting it in RoxyBrowser

Profile settings → proxy → enter host, port, username, password → **Check** → confirm the reported IP and location match what you ordered. That's the whole mechanical part — the judgment is in choosing and testing well, which is what this step teaches.

## Next in the course

- **Step 2:** [Antidetect browsers explained — fingerprints, VPNs, and privacy browsers](./antidetect-course-explained.md)
- Or jump to the practical bit: [How to use an antidetect browser](./antidetect-course-how-to-use.md)

**→ [Start RoxyBrowser free](https://mrait.ca/go/freebrowser)** — the free plan plus a proxy trial is all you need for this step.
