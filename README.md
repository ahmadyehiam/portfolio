# Ahmad Yehia — Portfolio site

| File | What it is |
|---|---|
| `index.html` | The public portfolio. It reads everything from `content.json`. |
| `admin.html` | Your back-office: edit content, make tracked links, see analytics, publish. |
| `content.json` | All the text, metrics and case studies. |
| `assets/` | Stylesheet, screenshots and your CV. |

## 1. Put it online (GitHub Pages, free, ~10 min)

1. Create a GitHub account if you don't have one, then a **new public repository**, e.g. `portfolio`.
2. On the repo page click **Add file → Upload files**, drag in everything from this folder (keep the `assets` folder), and commit.
3. Go to **Settings → Pages**, set *Source* to **Deploy from a branch**, branch `main`, folder `/ (root)`, and save.
4. After a minute your site is live at `https://<your-username>.github.io/portfolio/`.
   For a custom domain (e.g. `ahmadyehia.com`), add it under **Settings → Pages → Custom domain**.

## 2. Connect the back-office (so Publish works)

1. GitHub → your avatar → **Settings → Developer settings → Personal access tokens → Fine-grained tokens → Generate new token**.
2. *Repository access*: **Only select repositories** → your portfolio repo.
   *Permissions*: **Contents → Read and write**. Set an expiry date you're comfortable with.
3. Open `https://<your-site>/admin.html` → **Publish & settings**, fill in username, repo, branch (`main`) and the token → **Test connection**.

The token is stored only in that browser. Use **Forget token** on shared computers.
The admin page is public but useless without your token, and it's hidden from search engines.

## 3. Turn on analytics (GoatCounter, free, no cookies)

1. Sign up at goatcounter.com and pick a site code (e.g. `ahmadyehia`).
2. In admin → **Analytics**, enter that code, then **Publish**. Tracking starts on the live site.
3. To see stats inside the back-office: GoatCounter → **Settings → API** → create a key with **Read statistics**, paste it in the API key box.
   If your browser blocks the API, the panel links you to your GoatCounter dashboard instead; the same data is there.
4. Tick **Don't count my own visits** in each browser you use.

What gets counted: page visits, each case study read (half-visible for 1.5s), reaching the contact section,
LinkedIn / email / CV clicks, case-study filters, and visits from tracked links.

## 4. Tracked links

In **Tracked links**, add each company you apply to. You get a link like `…/?r=k7f2qm`.
Send that link in the application; Analytics shows visits per code next to the company.
Company names are kept only in your browser, so use **Download backup** now and then.

## Notes

- `assets/Ahmad-Yehia-CV.pdf` includes your phone number. Clear the CV path in settings to hide the download button.
- B.TECH screenshots: the payouts screen has statement IDs and balances blurred. Check you're allowed to show them publicly.
- Gold "Add:" notes on case studies only appear in **Preview**, never on the live site.
