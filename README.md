# young-group-site-deploy

Publishes **younggroupmtg.com** from the private repo `DYoung-cpu/young-group-site`, every 5 minutes when `main` has changed.

The website repo holds no deploy credentials, so people who edit the site never handle them. This repo fetches the site with a read-only key and uploads it to Vercel, which builds it.

Run it by hand: **Actions → Publish younggroupmtg.com → Run workflow**.

The Vercel token expires **2027-10-24**. Renew it in Vercel, then `gh secret set VERCEL_TOKEN -R DYoung-cpu/young-group-site-deploy`.
