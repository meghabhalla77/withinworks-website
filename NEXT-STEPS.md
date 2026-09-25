# Next steps for Megha (guide her through these in chat)

Agent instructions: Megha is non-technical. Walk her through ONE step at a time,
in plain language, and wait for her to confirm before moving on. Never ask her
to run commands. When she says a step is done, verify it yourself where possible.

## Status
- [x] Site is built and deployed on Vercel (managed by Sahil for now).
- [ ] Domain withinworksleadership.com needs to point at Vercel. **This is the current step.**
- [ ] Later: Sahil transfers the Vercel project to Megha's own Vercel account.
- [ ] Later: Stripe account (must be created by Megha, tied to her bank details).

## Current step: point the domain at Vercel (done in GoDaddy)

Goal: two DNS records in Megha's GoDaddy account.

Guide her like this:
1. Go to godaddy.com and sign in.
2. Click your name at the top right, then "My Products".
3. Find "withinworksleadership.com" and click "DNS" next to it.
4. In the list of records, look for rows where Type is "A". There will be one
   with Name "@" and one with Name "www". Delete both of them (trash icon).
5. Click "Add New Record". Type: A. Name: @. Value: 76.76.21.21. Save.
6. Click "Add New Record" again. Type: A. Name: www. Value: 76.76.21.21. Save.
7. Done. It can take up to an hour to take effect.

Agent verification (run yourself, do not ask her to):
    dig +short withinworksleadership.com A
    dig +short www.withinworksleadership.com A
Both should print 76.76.21.21. Then check https://withinworksleadership.com loads.
If the old values (13.248.243.5 / 76.223.105.230) still show, DNS has not propagated yet; wait and retry.

Easier alternative (so Megha never has to do DNS again): in GoDaddy, Account
Settings > Delegate Access > Invite, add Sahil's email with "Products, Domains
and Purchase" access. Then Sahil handles DNS.

## After DNS works
Tell Megha the site is live at https://withinworksleadership.com and that she
can ask for any change to the site in this chat. Changes go live after Sahil
deploys them (until the Vercel handover, deploys are done from Sahil's machine).
