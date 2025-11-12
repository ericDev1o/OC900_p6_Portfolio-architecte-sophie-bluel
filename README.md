# Portfolio-architecte-sophie-bluel

Code du projet 6 d'intégrateur web.

## Information pour le lancer le code

 - Lancer le backend depuis votre terminal en suivant les instruction du fichier ReadMe.
 - Si vous désirez afficher le code du backend et du frontend, faites le dans 2 instances de VSCode différentes pour éviter tout problème

### comment?
yarn start
si vous 
#### 1/2 veillez à ce que les paquets soient à jour et puis ...
 eric@eric-Aspire-TC-603:~/source/repos/OC/OC900_p6_Portfolio-architecte-sophie-bluel$ cd Backend/
eric@eric-Aspire-TC-603:~/source/repos/OC/OC900_p6_Portfolio-architecte-sophie-bluel/Backend$ ls
ReadMe.md  config       database.sqlite  middlewares  package.json  server.js
app.js     controllers  images           models       routes        swagger.yaml
eric@eric-Aspire-TC-603:~/source/repos/OC/OC900_p6_Portfolio-architecte-sophie-bluel/Backend$ node -v
v20.19.4
eric@eric-Aspire-TC-603:~/source/repos/OC/OC900_p6_Portfolio-architecte-sophie-bluel/Backend$ nvs use 25
PATH += ~/.nvs/node/25.2.0/x64/bin
eric@eric-Aspire-TC-603:~/source/repos/OC/OC900_p6_Portfolio-architecte-sophie-bluel/Backend$ yarn -v
1.22.22
eric@eric-Aspire-TC-603:~/source/repos/OC/OC900_p6_Portfolio-architecte-sophie-bluel/Backend$ corepack -v
0.34.2
eric@eric-Aspire-TC-603:~/source/repos/OC/OC900_p6_Portfolio-architecte-sophie-bluel/Backend$ corepack prepare yarn@4.11.0
Preparing yarn@4.11.0...
eric@eric-Aspire-TC-603:~/source/repos/OC/OC900_p6_Portfolio-architecte-sophie-bluel/Backend$ yarn install
yarn install v1.22.22
info No lockfile found.
[1/4] Resolving packages...
warning bcrypt > @mapbox/node-pre-gyp > npmlog@5.0.1: This package is no longer supported.
warning bcrypt > @mapbox/node-pre-gyp > rimraf@3.0.2: Rimraf versions prior to v4 are no longer supported
warning bcrypt > @mapbox/node-pre-gyp > npmlog > gauge@3.0.2: This package is no longer supported.
warning bcrypt > @mapbox/node-pre-gyp > npmlog > are-we-there-yet@2.0.0: This package is no longer supported.
warning bcrypt > @mapbox/node-pre-gyp > rimraf > glob@7.2.3: Glob versions prior to v9 are no longer supported
warning bcrypt > @mapbox/node-pre-gyp > rimraf > glob > inflight@1.0.6: This module is not supported, and leaks memory. Do not use it. Check out lru-cache if you want a good and tested way to coalesce async requests by a key value, which is much more comprehensive and powerful.
warning multer@1.4.4: Multer 1.x is affected by CVE-2022-24434. This is fixed in v1.4.4-lts.1 which drops support for versions of Node.js before 6. Please upgrade to at least Node.js 6 and version 1.4.4-lts.1 of Multer. If you need support for older versions of Node.js, we are open to accepting patches that would fix the CVE on the main 1.x release line, whilst maintaining compatibility with Node.js 0.10.
warning sqlite3 > node-gyp > glob@7.2.3: Glob versions prior to v9 are no longer supported
warning sqlite3 > node-gyp > npmlog@6.0.2: This package is no longer supported.
warning sqlite3 > node-gyp > rimraf@3.0.2: Rimraf versions prior to v4 are no longer supported
warning sqlite3 > node-gyp > npmlog > gauge@4.0.4: This package is no longer supported.
warning sqlite3 > node-gyp > npmlog > are-we-there-yet@3.0.1: This package is no longer supported.
warning sqlite3 > node-gyp > make-fetch-happen > cacache > glob@7.2.3: Glob versions prior to v9 are no longer supported
warning sqlite3 > node-gyp > make-fetch-happen > cacache > rimraf@3.0.2: Rimraf versions prior to v4 are no longer supported
warning sqlite3 > node-gyp > make-fetch-happen > cacache > @npmcli/move-file@1.1.2: This functionality has been moved to @npmcli/fs
warning sqlite3 > node-gyp > make-fetch-happen > cacache > @npmcli/move-file > rimraf@3.0.2: Rimraf versions prior to v4 are no longer supported
warning yamljs > glob@7.2.3: Glob versions prior to v9 are no longer supported
[2/4] Fetching packages...
[3/4] Linking dependencies...
[4/4] Building fresh packages...
success Saved lockfile.
Done in 14.16s.
eric@eric-Aspire-TC-603:~/source/repos/OC/OC900_p6_Portfolio-architecte-sophie-bluel/Backend$ corepack prepare yarn@4.11.0 --activate
Preparing yarn@4.11.0 for immediate activation...
eric@eric-Aspire-TC-603:~/source/repos/OC/OC900_p6_Portfolio-architecte-sophie-bluel/Backend$ corepack yarn -v
4.11.0
eric@eric-Aspire-TC-603:~/source/repos/OC/OC900_p6_Portfolio-architecte-sophie-bluel/Backend$ npm install bcrypt@latest

added 1 package, removed 10 packages, changed 2 packages, and audited 282 packages in 3s

31 packages are looking for funding
  run `npm fund` for details

6 high severity vulnerabilities

To address issues that do not require attention, run:
  npm audit fix

To address all issues (including breaking changes), run:
  npm audit fix --force

Run `npm audit` for details.
eric@eric-Aspire-TC-603:~/source/repos/OC/OC900_p6_Portfolio-architecte-sophie-bluel/Backend$ npm audit fix

changed 1 package, and audited 282 packages in 2s

31 packages are looking for funding
  run `npm fund` for details

# npm audit report

dicer  *
Severity: high
Crash in HeaderParser in dicer - https://github.com/advisories/GHSA-wm7h-9275-46v2
fix available via `npm audit fix --force`
Will install multer@2.0.2, which is a breaking change
node_modules/dicer
  busboy  <=0.3.1
  Depends on vulnerable versions of dicer
  node_modules/busboy
    multer  <=2.0.1
    Depends on vulnerable versions of busboy
    node_modules/multer


semver  7.0.0 - 7.5.1
Severity: high
semver vulnerable to Regular Expression Denial of Service - https://github.com/advisories/GHSA-c2qf-rxjj-qqgw
fix available via `npm audit fix`
node_modules/simple-update-notifier/node_modules/semver
  simple-update-notifier  1.0.7 - 1.1.0
  Depends on vulnerable versions of semver
  node_modules/simple-update-notifier
    nodemon  2.0.19 - 2.0.22
    Depends on vulnerable versions of simple-update-notifier
    node_modules/nodemon

6 high severity vulnerabilities

To address issues that do not require attention, run:
  npm audit fix

To address all issues (including breaking changes), run:
  npm audit fix --force
eric@eric-Aspire-TC-603:~/source/repos/OC/OC900_p6_Portfolio-architecte-sophie-bluel/Backend$ yarn add multer@latest
yarn add v1.22.22
warning package-lock.json found. Your project contains lock files generated by tools other than Yarn. It is advised not to mix package managers in order to avoid resolution inconsistencies caused by unsynchronized lock files. To clear this warning, remove package-lock.json.
[1/4] Resolving packages...
[2/4] Fetching packages...
[3/4] Linking dependencies...
[4/4] Building fresh packages...
success Saved lockfile.
success Saved 5 new dependencies.
info Direct dependencies
└─ multer@2.0.2
info All dependencies
├─ busboy@1.6.0
├─ concat-stream@2.0.0
├─ multer@2.0.2
├─ streamsearch@1.1.0
└─ xtend@4.0.2
Done in 25.76s.
eric@eric-Aspire-TC-603:~/source/repos/OC/OC900_p6_Portfolio-architecte-sophie-bluel/Backend$ npm install yarn@latest

added 5 packages, removed 4 packages, changed 1 package, and audited 271 packages in 2s

31 packages are looking for funding
  run `npm fund` for details

3 high severity vulnerabilities

To address all issues, run:
  npm audit fix

Run `npm audit` for details.
eric@eric-Aspire-TC-603:~/source/repos/OC/OC900_p6_Portfolio-architecte-sophie-bluel/Backend$ npm install -g yarn@latest

changed 1 package in 639ms
eric@eric-Aspire-TC-603:~/source/repos/OC/OC900_p6_Portfolio-architecte-sophie-bluel/Backend$ yarn -v
1.22.22
eric@eric-Aspire-TC-603:~/source/repos/OC/OC900_p6_Portfolio-architecte-sophie-bluel/Backend$ yarn set version stable
➤ YN0000: You don't seem to have Corepack enabled; we'll have to rely on yarnPath instead
➤ YN0000: Downloading https://repo.yarnpkg.com/4.11.0/packages/yarnpkg-cli/bin/yarn.js
➤ YN0000: Saving the new release in .yarn/releases/yarn-4.11.0.cjs
➤ YN0000: Done with warnings in 0s 189ms
eric@eric-Aspire-TC-603:~/source/repos/OC/OC900_p6_Portfolio-architecte-sophie-bluel/Backend$ corepack enable
Internal Error: EACCES: permission denied, unlink '/usr/local/bin/yarn'
    at async Object.unlink (node:internal/fs/promises:1068:10)
    at async EnableCommand.generatePosixLink (/usr/local/lib/node_modules/corepack/dist/lib/corepack.cjs:23158:9)
    at async Promise.all (index 2)
    at async EnableCommand.execute (/usr/local/lib/node_modules/corepack/dist/lib/corepack.cjs:23146:5)
    at async EnableCommand.validateAndExecute (/usr/local/lib/node_modules/corepack/dist/lib/corepack.cjs:20252:22)
    at async _Cli.run (/usr/local/lib/node_modules/corepack/dist/lib/corepack.cjs:21189:18)
    at async Object.runMain (/usr/local/lib/node_modules/corepack/dist/lib/corepack.cjs:23649:19)
eric@eric-Aspire-TC-603:~/source/repos/OC/OC900_p6_Portfolio-architecte-sophie-bluel/Backend$ sudo npm install -g yarn@latest
[sudo: authenticate] Password: 

changed 1 package in 2s
eric@eric-Aspire-TC-603:~/source/repos/OC/OC900_p6_Portfolio-architecte-sophie-bluel/Backend$ yarn -v
4.11.0
eric@eric-Aspire-TC-603:~/source/repos/OC/OC900_p6_Portfolio-architecte-sophie-bluel/Backend$ corepack yarn -v
4.11.0
eric@eric-Aspire-TC-603:~/source/repos/OC/OC900_p6_Portfolio-architecte-sophie-bluel/Backend$ yarn install
➤ YN0087: Migrated your project to the latest Yarn version 🚀

➤ YN0000: · Yarn 4.11.0
➤ YN0000: ┌ Resolution step
➤ YN0085: │ + bcrypt@npm:6.0.0, cors@npm:2.8.5, dotenv@npm:16.6.1, and 323 more.
➤ YN0000: └ Completed in 1s 313ms
➤ YN0000: ┌ Fetch step
➤ YN0013: │ 50 packages were added to the project (+ 33.2 MiB).
➤ YN0000: └ Completed in 4s 172ms
➤ YN0000: ┌ Link step
➤ YN0007: │ bcrypt@npm:6.0.0 must be built because it never has been before or the last one failed
➤ YN0007: │ sqlite3@npm:5.1.7 [235d8] must be built because it never has been before or the last one failed
➤ YN0007: │ yarn@npm:1.22.22 must be built because it never has been before or the last one failed
➤ YN0007: │ @scarf/scarf@npm:1.4.0 must be built because it never has been before or the last one failed
➤ YN0000: └ Completed in 6s 552ms
➤ YN0000: · Done in 12s 138ms
eric@eric-Aspire-TC-603:~/source/repos/OC/OC900_p6_Portfolio-architecte-sophie-bluel/Backend$ yarn -v
4.11.0
eric@eric-Aspire-TC-603:~/source/repos/OC/OC900_p6_Portfolio-architecte-sophie-bluel/Backend$ npm audit fix

added 4 packages, removed 88 packages, changed 22 packages, and audited 271 packages in 2s

31 packages are looking for funding
  run `npm fund` for details

# npm audit report

semver  7.0.0 - 7.5.1
Severity: high
semver vulnerable to Regular Expression Denial of Service - https://github.com/advisories/GHSA-c2qf-rxjj-qqgw
fix available via `npm audit fix`
node_modules/simple-update-notifier/node_modules/semver
  simple-update-notifier  1.0.7 - 1.1.0
  Depends on vulnerable versions of semver
  node_modules/simple-update-notifier
    nodemon  2.0.19 - 2.0.22
    Depends on vulnerable versions of simple-update-notifier
    node_modules/nodemon

3 high severity vulnerabilities

To address all issues, run:
  npm audit fix
eric@eric-Aspire-TC-603:~/source/repos/OC/OC900_p6_Portfolio-architecte-sophie-bluel/Backend$ yarn add sqlite3@latest
➤ YN0000: · Yarn 4.11.0
➤ YN0000: ┌ Resolution step
➤ YN0085: │ + bcrypt@npm:6.0.0, cors@npm:2.8.5, dotenv@npm:16.6.1, and 323 more.
➤ YN0000: └ Completed in 0s 749ms
➤ YN0000: ┌ Fetch step
➤ YN0000: └ Completed in 0s 312ms
➤ YN0000: ┌ Link step
➤ YN0000: └ Completed in 0s 899ms
➤ YN0000: · Done in 2s 66ms
eric@eric-Aspire-TC-603:~/source/repos/OC/OC900_p6_Portfolio-architecte-sophie-bluel/Backend$ yarn install
➤ YN0000: · Yarn 4.11.0
➤ YN0000: ┌ Resolution step
➤ YN0085: │ + dotenv@npm:17.2.3, express@npm:5.1.0, helmet@npm:8.1.0, and 25 more.
➤ YN0085: │ - accepts@npm:1.3.8, array-flatten@npm:1.1.1, and 31 more.
➤ YN0000: └ Completed in 2s 309ms
➤ YN0000: ┌ Fetch step
➤ YN0013: │ 5 packages were added to the project (+ 1.11 MiB).
➤ YN0000: └ Completed in 4s 315ms
➤ YN0000: ┌ Link step
➤ YN0000: └ Completed in 2s 118ms
➤ YN0000: · Done in 8s 871ms
eric@eric-Aspire-TC-603:~/source/repos/OC/OC900_p6_Portfolio-architecte-sophie-bluel/Backend$ npm audit fix

added 12 packages, removed 91 packages, changed 31 packages, and audited 269 packages in 8s

33 packages are looking for funding
  run `npm fund` for details

found 0 vulnerabilities
eric@eric-Aspire-TC-603:~/source/repos/OC/OC900_p6_Portfolio-architecte-sophie-bluel/Backend$ 

#### 2/2 et que vous résolvez
eric@eric-Aspire-TC-603:~/source/repos/OC/OC900_p6_Portfolio-architecte-sophie-bluel/Backend$ yarn start
Internal Error: dwf-projet6-backend@workspace:.: This package doesn't seem to be present in your lockfile; run "yarn install" to update the lockfile
    at jR.getCandidates (/home/eric/source/repos/OC/OC900_p6_Portfolio-architecte-sophie-bluel/Backend/.yarn/releases/yarn-4.11.0.cjs:204:4607)
    at rm.getCandidates (/home/eric/source/repos/OC/OC900_p6_Portfolio-architecte-sophie-bluel/Backend/.yarn/releases/yarn-4.11.0.cjs:141:1311)
    at /home/eric/source/repos/OC/OC900_p6_Portfolio-architecte-sophie-bluel/Backend/.yarn/releases/yarn-4.11.0.cjs:209:8420
    at qE (/home/eric/source/repos/OC/OC900_p6_Portfolio-architecte-sophie-bluel/Backend/.yarn/releases/yarn-4.11.0.cjs:140:45054)
    at mt (/home/eric/source/repos/OC/OC900_p6_Portfolio-architecte-sophie-bluel/Backend/.yarn/releases/yarn-4.11.0.cjs:209:8400)
    at async Promise.allSettled (index 0)
    at async Uu (/home/eric/source/repos/OC/OC900_p6_Portfolio-architecte-sophie-bluel/Backend/.yarn/releases/yarn-4.11.0.cjs:140:44382)
    at async /home/eric/source/repos/OC/OC900_p6_Portfolio-architecte-sophie-bluel/Backend/.yarn/releases/yarn-4.11.0.cjs:209:9166
    at async ki.startProgressPromise (/home/eric/source/repos/OC/OC900_p6_Portfolio-architecte-sophie-bluel/Backend/.yarn/releases/yarn-4.11.0.cjs:140:129679)
    at async t.resolveEverything (/home/eric/source/repos/OC/OC900_p6_Portfolio-architecte-sophie-bluel/Backend/.yarn/releases/yarn-4.11.0.cjs:209:7138)
eric@eric-Aspire-TC-603:~/source/repos/OC/OC900_p6_Portfolio-architecte-sophie-bluel/Backend$ 
