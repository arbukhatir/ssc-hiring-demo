# نظام طلبات التوظيف للأندية — معاينة الواجهة

**Club Hiring Request System — UI demo**
Sharjah Sports Council · مجلس الشارقة الرياضي

**▶ [View the demo](https://arbukhatir.github.io/ssc-hiring-demo/)**

---

## What this is

A **static, front-end-only demo** of the interface for an internal system that
lets Sharjah Sports Council member clubs submit hiring requests and lets the
Council's HR function review and decide on them.

It exists so the design can be shown and discussed without installing anything.
Open the link, or open `index.html` from a local copy — it needs no server, no
database, no build step and no network access.

## What this is *not*

> This repository contains **only the user interface**. It is a mock-up.

- ❌ No application code, no backend, no database
- ❌ Nothing is saved — buttons and forms do not submit anywhere
- ❌ No login; the four views are switched from the top (or bottom) navigation
- ❌ **No real data.** Every candidate name, reference number, date and salary
  is invented. The club names are the Council's real member clubs, but nothing
  attributed to them is real.

The working application is a separate, private Laravel system.

## What you can look at

| View | Shows |
|---|---|
| **لوحة النادي** | Club dashboard — status summary, filters, request list |
| **نموذج طلب توظيف** | The six-section hiring request form |
| **تفاصيل الطلب** | A single request: details, timeline, correspondence |
| **لوحة المجلس** | Council HR queue and the decision panel |

Plus the status badges, the Council-only section, and the navy footer.

## Design

Follows the design language of the Council's public site,
**[ssc.shj.ae](https://ssc.shj.ae)**, together with the corporate identity guide
(*دليل استخدام الهوية المؤسسية*):

| | |
|---|---|
| Typeface | **Alexandria** — self-hosted, embedded in the page |
| Navy | `#183254` |
| Gold | `#DFC07F` |
| Sand | `#F2E9D4` |
| Motif | The Sharjah arch (mihrab) |
| Direction | Arabic-first, RTL |

**Accessibility.** Gold measures 1.75:1 on white, so — as on the live site — it
never carries text on a light ground; gold surfaces take black labels (11.98:1).
Status is shown with an icon *and* a word, never colour alone. Every control has
a 44 px minimum touch area.

**Mobile.** Phones get a different layout, not a squeezed desktop: a bottom
navigation bar within thumb reach, the request table re-flowed into cards, and
filters collapsed behind a disclosure. Verified with no horizontal scroll at
320 px and 375 px, and in landscape.

## Running it locally

Download `index.html` and open it. That is the whole procedure — everything,
including the typeface and the logo, is embedded in the one file.

## Provenance

The Sharjah Sports Council logo is used with the Council's own brand assets
under its identity guidelines. Alexandria is licensed under the
[SIL Open Font License 1.1](https://openfontlicense.org).

---

*Interface demonstration only. Not a deployed system, and not for entering real
candidate information.*
