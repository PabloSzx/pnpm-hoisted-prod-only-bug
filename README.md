# pnpm-hoisted-prod-bug

Install all dependencies:

```
pnpm i
```

```
Lockfile is up-to-date, resolution step is skipped
Packages: +4
++++
Packages are hard linked from the content-addressable store to the virtual store.
  Content-addressable store is at: /home/pablosz/.pnpm-store/v3
  Virtual store is at:             node_modules/.pnpm
node_modules/@prisma/client: Running postinstall script, done in 497ms
node_modules/@prisma/engines: Running postinstall script, done in 278ms
node_modules/prisma: Running preinstall script, done in 28ms
node_modules/prisma: Running install script, done in 24ms
Progress: resolved 0, reused 4, downloaded 0, added 4, done
```

Then install only prod dependencies:

```
pnpm i --prod
```

```
Lockfile is up-to-date, resolution step is skipped
 ERROR  Cannot read properties of undefined (reading 'name')
```
