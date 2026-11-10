# Funding Dept Home Ready Check (forwarder + rates feed)

The Home Ready Check quiz by Daniel Herrera, Mortgage Loan Officer (NMLS #2337126), Funding Dept., powered by Mpire Financial (NMLS #2108504), now lives on Daniel's website: https://getreadytobuyahome.phonesites.com/#hrc

What this repo still does:
- `index.html` forwards anyone using the old fundingdept.github.io link to the quiz on the website (tagged `src=old-quiz-link` unless the link already had a tracking tag).
- `rates.json` is the daily 30-yr FHA / VA rate feed the website quiz reads. It is updated by `.github/workflows/update-rates.yml`. Keep this running.
- `.github/workflows/lead-heartbeat.yml` sends a daily test through the FormSubmit lead path.

The previous quiz page is in this repo's git history (the commit before "Forward old quiz link to the website").
