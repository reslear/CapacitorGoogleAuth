# CapacitorGoogleAuth

Capacitor plugin for Google Auth.

> ⚠️ This is fork original plugin [@codetrix-studio/capacitor-google-auth](https://github.com/CodetrixStudio/CapacitorGoogleAuth) with new beta features, changes or experiments

fork changes:

- [ x ] [#112](https://github.com/CodetrixStudio/CapacitorGoogleAuth/pull/112) - bump deps, init peer dependencies
- [ x ] [#113](https://github.com/CodetrixStudio/CapacitorGoogleAuth/pull/113) - protect add duplicate script
- [ x ] [#114](https://github.com/CodetrixStudio/CapacitorGoogleAuth/pull/114) - add support `.ts` and `.js` config

### Install

```sh
npm i -D @reslear/capacitor-google-auth

npx cap sync
```

### WEB

Register plugin and manually initialize

```ts
import { GoogleAuth } from '@reslear/capacitor-google-auth'

GoogleAuth.init({
  scopes: ["profile", "email"],
  offline: true
})
```
> see `init` method options - descriptions, examples, default values and types in `definition.ts`

Use it

```ts
GoogleAuth.signIn()
```

### Config, IOS, ANDROID and etc..

see originally instruction [CodetrixStudio/CapacitorGoogleAuth](https://github.com/CodetrixStudio/CapacitorGoogleAuth)
