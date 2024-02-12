# CircleCI Concurrency Control Orb

CircleCI Orb to limit workflow concurrency.

Why? Some jobs (typically deployments) need to run sequentially and not
parallel, but also run to completion. So CircleCI's native `auto-cancel` is not
quite the right fit.

Fork of eddiewebb/queue v3 pre-release.

Usage: https://circleci.com/developer/orbs/orb/carwow/queue
