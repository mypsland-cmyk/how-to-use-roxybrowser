# Antidetect Browser Course, Step 4: Set Up a Windows 10/11 VM for Your Antidetect Browser

> **Meta title:** Windows 10/11 VM for an Antidetect Browser: VirtualBox, VMware or Cloud (Step 4)
> **Meta description:** Antidetect Browser Course Step 4 — build a Windows 10/11 virtual machine (VirtualBox, VMware, or cloud) to run your antidetect browser, with sensible RAM/CPU/disk settings and proxy hookup.
> **Suggested slug:** `antidetect-browser-course-windows-vm`

*This post contains affiliate links. If you sign up through them, I may earn a commission at no extra cost to you.*

**📺 Watch the video version:**

[![antidetect browser course: create windows 10 computer (Step 4)](https://img.youtube.com/vi/3eqxPU8NAYA/hqdefault.jpg)](https://www.youtube.com/watch?v=3eqxPU8NAYA&list=PLxY412qgkijKLUO1Gplz2q0MyCQC59Vnt)

---

Step 4 answers a question serious operators eventually ask: *should my antidetect browser live in its own machine?* The answer is a virtual machine — a full Windows 10/11 environment isolated from your daily computer, dedicated to profile work.

## Why run the browser in a VM at all?

RoxyBrowser already isolates profiles from each other. A VM adds a second ring: it isolates **the whole working environment from your personal machine** — separate system, separate storage, one machine for "work identities," one for life. For teams, a VM (or cloud instance) also becomes a shared, consistent workplace that any operator can log into.

## Your three options

1. **Local VM on your own hardware** — VirtualBox (free) or VMware Workstation Player on your Windows/Linux/Mac machine. Cheapest; performance depends on your host.
2. **Dedicated spare PC** — skip virtualization entirely; install Windows and the browser directly.
3. **Cloud Windows VM** — rent a Windows instance by the hour/month. Runs on someone else's always-on hardware, accessible from anywhere, easy to snapshot and clone.

## Building the VM: sensible specs

For a Windows 10/11 VM running RoxyBrowser with a handful of open profiles:

- **RAM:** 4–8 GB to the VM (8 GB if you keep many profiles open; the host needs its own headroom on top)
- **CPU:** 2–4 vCPUs
- **Disk:** 60–100 GB (Windows itself eats ~30 GB; browser profiles and extensions add up)
- **Video:** leave 3D acceleration off unless a workflow demands it — default virtual graphics are the least surprising choice

If you're on VirtualBox: install a licensed Windows 10/11 image, install Guest Additions (or VMware Tools) for sane resolution and clipboard, and take a **snapshot immediately after setup** — it's your rollback point whenever an experiment goes sideways.

## Network and proxy hookup

Inside the VM, keep networking on the default NAT/Bridged mode so the guest reaches the internet normally — then do the proxy work at the **profile level inside RoxyBrowser**, exactly as in [Step 1](./antidetect-course-free-proxy.md). The VM doesn't replace per-profile proxies; it just gives them a clean, dedicated place to live. (Routing the entire VM through one proxy is a valid advanced pattern — but then every profile in it shares that IP, which defeats per-profile separation.)

## Install and verify

1. Install RoxyBrowser inside the VM from the [official download](https://mrait.ca/go/freebrowser).
2. Open a profile, hit the proxy **Check**, confirm IP and location.
3. Visit a fingerprint test site from the profile and confirm results match the profile's story.
4. Snapshot the VM again — this is your known-good "workstation" state.

## Next in the course

- **Step 6:** [Create an iPhone device profile (and validate it)](./antidetect-course-iphone-device.md)
- Skipped ahead? [Step 3: how to use an antidetect browser](./antidetect-course-how-to-use.md)

**→ [Try RoxyBrowser free](https://mrait.ca/go/freebrowser)** — the free 2-profile plan runs fine inside a modest VM.
