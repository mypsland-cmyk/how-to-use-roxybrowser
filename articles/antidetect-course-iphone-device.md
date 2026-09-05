# Antidetect Browser Course, Step 6: Create a Convincing iPhone Device Profile (and Validate It)

*This post contains affiliate links. If you sign up through them, I may earn a commission at no extra cost to you.*

**📺 Watch the video version:**

[![antidetect browser course: create an iPhone device (Step 6)](https://img.youtube.com/vi/j-Yh7cl0lSg/hqdefault.jpg)](https://www.youtube.com/watch?v=j-Yh7cl0lSg&list=PLxY412qgkijKLUO1Gplz2q0MyCQC59Vnt)

---

Step 6 is where fingerprint craft gets specific: building a profile that convincingly presents as an **iPhone**. Mobile-looking profiles matter because most social platform activity is mobile — a "person" who never touches a phone is its own kind of odd. This is also the step where you learn to *validate* a profile like a professional.

## The parameters that make the phone

In RoxyBrowser's profile settings, these are the dials that matter:

1. **User agent** — an iPhone Safari UA string matching a current iOS version. This is the headline claim; everything else must agree with it.
2. **Viewport / screen** — iPhone-class dimensions and device pixel ratio. A claimed phone with a 1920×1080 screen is an instant contradiction.
3. **WebGL vendor/renderer** — must report Apple-class GPU values. WebGL is one of the loudest mismatch signals a profile can emit.
4. **Time zone and language** — set both to where your proxy IP lives (you chose the IP in [Step 1](./antidetect-course-free-proxy.md); the phone should live there too).
5. **Platform and touch signals** — the profile should claim and *behave* as a touch device where the browser exposes that.

The rule that governs all of it: **one story, told everywhere.** UA says iPhone 15 on iOS 18 → screen says iPhone 15 → GPU says Apple → time zone says the IP's country. Six small true-ish claims beat one big exotic one.

## The professional part: validation

Amateurs set a user agent and stop. The validation loop is what makes profiles trustworthy:

1. Save the profile and launch it.
2. Open public fingerprint test pages from *inside* the profile.
3. Read the results like a skeptic: does the device story hold up across UA, screen, WebGL, fonts, time zone?
4. Check the exit IP's country against the profile's time zone/language.
5. Fix contradictions, save, and re-test until the report is boring and consistent.

Re-validate any profile whenever you change its fingerprint or proxy — a five-minute habit that protects months of account history.

## Fair-use framing

A believable device profile is a tool for legitimate multi-account work: managing client social accounts, testing how sites behave on devices you don't own (QA), and keeping work identities separate. It isn't a tool for impersonating people or defeating platform rules — know the terms of every platform you operate on, and use skills only on accounts you're entitled to manage.

## Next in the course

- Miss the fundamentals? [Step 2: antidetect browsers explained](./antidetect-course-explained.md)
- Ready for the tool tour: [complete RoxyBrowser walkthrough](./how-to-use-roxybrowser-walkthrough.md)

**→ [Try RoxyBrowser free](https://mrait.ca/go/freebrowser)** — its 160+ fingerprint parameters make this step a settings exercise, not an engineering project.
