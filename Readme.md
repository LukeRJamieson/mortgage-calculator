# Offset Mortgage Calculator

A single-page home loan planner for Victoria, Australia. Everything runs in the browser; there is no server and no build step.

- Weekly, fortnightly and monthly repayments, with your own nominated repayment
- Offset account (balance, linkage, monthly growth from you and a partner) and debt-free date
- Offset vs extra repayments optimiser
- RBA cash rate history since your loan start
- Property valuations (Mooroolbark suburb data, plus your council, bank and agent figures)
- Victorian Homebuyer Fund buy-back, including the income-threshold repayment
- Rental income with land tax and tax effects
- Monthly budget from your take-home pay

## Host it on GitHub Pages

1. Create a new repository on GitHub, for example `mortgage-calculator`.
2. Upload `index.html` (and this README) to the root of the repository.
   - On the web: **Add file → Upload files**, drag the files in, then **Commit changes**.
   - Or from a terminal:
     ```sh
     git init
     git add index.html README.md
     git commit -m "Offset mortgage calculator"
     git branch -M main
     git remote add origin https://github.com/<your-username>/mortgage-calculator.git
     git push -u origin main
     ```
3. In the repository, open **Settings → Pages**.
4. Under **Build and deployment**, set **Source** to **Deploy from a branch**, choose **main** and **/ (root)**, then **Save**.
5. After a minute the site is live at `https://<your-username>.github.io/mortgage-calculator/`.

To update it later, replace `index.html` and commit again.

## Saving and sharing your figures

- **Save in this browser** keeps named scenarios in your browser's local storage. They don't sync between devices.
- **Copy share link** puts all your figures into the link after `#plan=`. Anyone with the link sees them. The part after `#` is never sent to GitHub's servers, but it is stored wherever the link is pasted (messages, email, browser history).
- **Download data file / Open data file** saves and loads a `mortgage-plan.json` file.

A public GitHub Pages site is visible to anyone, but your figures are not in the site itself: they only exist in your browser, your share links and your data files.

## Data notes

Suburb figures and RBA cash rates were researched in September 2026 and are built into the page. To refresh them, edit the `RBA_CHANGES` and `MARKET` constants near the top of the script in `index.html`. All results are estimates, not financial advice.
