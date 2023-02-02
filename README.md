To replicate problem:

### Install dependencies

`pnpm install`

### Prune

`pnpm exec turbo prune --scope=@storis/monorepo-migration-apps`

### Check lockfile integrity

```
cd out
pnpm install --frozen-lockfile
```

Getting error:

```
λ pnpm install --frozen-lockfile
Scope: all 12 workspace projects
Lockfile is up to date, resolution step is skipped
 ERR_PNPM_LOCKFILE_MISSING_DEPENDENCY  Broken lockfile: no entry for '/qs/6.10.3' in pnpm-lock.yaml

This issue is probably caused by a badly resolved merge conflict.
To fix the lockfile, run 'pnpm install --no-frozen-lockfile'.
```
