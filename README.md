# Ionic standalone components + Angular 17 with SSR

This repo describes the issue, which occures only when the hydration is enabled.

## Steps to reproduce:
1. `ionic start modern-app blank --type angular`
2. [Add SSR support](https://github.com/playerx/ionic-angular-ssr-issue/commit/454a742e1e2f3c9a607ca1835a9c89a24af3c832)

Workaround:
* [Disable Hydration](https://github.com/playerx/ionic-angular-ssr-issue/commit/ff1f73bddfb3c5281448ddc5939daa79494561fd)


## Issue
Project breaks when enabling Hydration on this line:

https://github.com/playerx/ionic-angular-ssr-issue/blob/main/src/app/app.config.ts#L20


