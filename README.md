## Archived

Since the theme moved to docsy, this preview build broke.
It was a workaround because we didn't have permissions for the main repository.
Now that's resolved we should use the CI pipeline set up there.

---

[![Build Status](https://drone.sfosc.robin-it.com/api/badges/Beanow/sfosc-drone-cron/status.svg)](https://drone.sfosc.robin-it.com/Beanow/sfosc-drone-cron)

This is a workaround for [sfosc/sfosc #79](https://github.com/sfosc/sfosc/issues/79) to build the preview at a regular interval.
https://sfosc.org/preview/

It runs a cronjob to see if the SHA hash of the main repository has changed.
https://github.com/sfosc/sfosc

If it has, it will push a new build to https://github.com/sfosc/preview.
