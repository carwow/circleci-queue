# CircleCI Concurrency Control Orb

CircleCI Orb to limit workflow concurrency.

Why? Some jobs (typically deployments) need to run sequentially and not
parallel, but also run to completion. So CircleCI's native `auto-cancel` is not
quite the right fit.

Fork of eddiewebb/queue v3 pre-release.

Usage: https://circleci.com/developer/orbs/orb/carwow/queue

## Superseded pipelines

By default, when a newer pipeline is found ahead of the current one, the job
cancels itself and shows as failed. Set `on-superseded: skip` to end the job
successfully and skip its remaining steps instead. Make sure any job that
requires it can safely run when the steps were skipped.
