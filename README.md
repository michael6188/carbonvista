# CarbonVista — ESG Report Writer (prototype)

A clickable prototype of an AI tool that helps companies write their ESG (Environmental, Social and Governance) report.

**Status:** UI prototype only. The "AI" writing is simulated. It fills a fixed text template with the figures you type in, and nothing is saved or sent anywhere.

## How it works (the 5 steps)

1. **Company profile:** name, reporting year, industry.
2. **Frameworks:** pick HKEX ESG Reporting Code, GRI, ISSB (IFRS S1 & S2) and/or SASB.
3. **ESG data:** enter 12 environmental, social and governance metrics.
4. **AI draft:** generate each report section. Your figures show in green, missing figures in amber, and writing prompts in grey.
5. **Review & export:** check what is accepted, then export. Export is not built yet.

## How to run it

No installation needed.

- **Easiest:** double-click `index.html` to open it in Chrome, Edge, Safari or Firefox. You need an internet connection because it loads a small library and fonts.
- **If the page is blank:** some browsers block this when opening a file directly. In VS Code, install the *Live Server* extension, right-click `index.html`, and choose **Open with Live Server**.

## Files

| File | What it is |
|------|------------|
| `index.html` | The whole app: page styles, content lists, and app logic |
| `README.md` | This file |

Inside `index.html`, the parts you're most likely to edit are marked with numbered comments:
1. **CONTENT:** the steps, frameworks and metrics lists
2. **FAKE AI:** the draft text templates (later replaced by a real AI call)
3. **ICONS**
4. **THE APP:** the screens

To change the main colour, edit `--accent` near the top of the `<style>` block.

## Roadmap

- [ ] Get feedback from 2–3 people who write ESG reports
- [ ] Move to a proper project setup (e.g. React + a small server)
- [ ] Connect a real AI model through a server, so the API key is never in the browser
- [ ] Spreadsheet import
- [ ] Word / PDF export
- [ ] Save reports to a database and add user accounts

## Important

AI-drafted ESG content must be checked by a person against source records before publication. Never commit API keys or passwords to this repository. Keep them in a `.env` file, which `.gitignore` excludes.
