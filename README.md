<p align="center">
  <img src="https://raw.githubusercontent.com/zaneGittins/bifract/main/web/static/logo.png" alt="Bifract logo" width="140">
</p>

# Boring Binaries Behaving Badly

**How to baseline endpoint behavior, and catch what doesn't fit.**

An Antisyphon Anti-cast by Zane Gittins, November 18, 2026.

Defenders have the home turf advantage, but only if we know our environment better than the attacker does. This talk turns "baseline your environment" into a recipe you can run in the SIEM you already have: **choose** what to count, **count** days instead of events, and **compare** with first seen, rarity, and coverage. Then we use it to catch signed, boring binaries doing things they shouldn't.

📑 **Slides:** [Boring-Binaries-Behaving-Badly_Zane-Gittins_2026.pdf](Boring-Binaries-Behaving-Badly_Zane-Gittins_2026.pdf)

## 🧪 Try it yourself

Everything from the live demo runs free at **[labs.bifract.io](https://labs.bifract.io)**. Open a lab in GitHub Codespaces; there's nothing to install.

* **Lab 001:** the intrusion from the demo. Five hosts, three days of Sysmon, Windows logs, Zeek, and Autoruns. Hunt it with first seen remote tools, beacon scoring, and provenance graphs (`pgr()`). The walkthrough also covers what the demo skipped: the ClickFix initial access, the password spray, and the service on WS03.
* **Lab 002:** a month of data for the RMM example from the slides, with first seen, rarity, and coverage. It also walks through three checks for whether a baseline will work on your own data.

### Bifract

* [Bifract](https://github.com/zaneGittins/bifract)
* [Bifract Labs](https://labs.bifract.io)
* [Bifract Docs](https://docs.bifract.io)

### Resources and Blog Posts

* [Enriching Sysmon w/ Velociraptor Blog Post](https://signalsleuth.io/2025/08/31/sysmon_enrichment.html)
* [MagicSword LOLRMM](https://github.com/magicsword-io/LOLRMM)
* [CelesTLSH](https://github.com/Magonia-Research/CelesTLSH-Hashes/)
* [NoDoze Research Paper](https://www.ndss-symposium.org/ndss-paper/nodoze-combatting-threat-alert-fatigue-with-automated-provenance-triage/)
* [Canary Tokens](https://canarytokens.org/nest/)
* [RITA](https://github.com/activecm/rita)

### Velociraptor Artifacts

* [Windows.EventLogs.SysmonProcessEnriched](https://docs.velociraptor.app/exchange/artifacts/pages/windows.eventlogs.sysmonprocessenriched/)
* [Linux Honeyfiles](https://docs.velociraptor.app/exchange/artifacts/pages/linux.detection.honeyfiles/)
* [Windows Honeyfiles](https://docs.velociraptor.app/exchange/artifacts/pages/windows.detection.honeyfile/)
