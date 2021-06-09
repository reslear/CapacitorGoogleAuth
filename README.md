# CapacitorGoogleAuth

Capacitor plugin for Google Auth.

> ⚠️ This is fork original plugin [@codetrix-studio/capacitor-google-auth](https://github.com/CodetrixStudio/CapacitorGoogleAuth) as temporally solution for support **Capacitor 3**

fork features:

- [ x ] feature

### Install

```sh
npm i -D @reslear/capacitor-google-auth

npx cap sync
```

### WEB

Register plugin and manually initialize

```ts
import { GoogleAuth } from '@reslear/capacitor-google-auth'

GoogleAuth.init()
```

Use it

```ts
GoogleAuth.signIn()
```

### Config, IOS, ANDROID and etc..

see originally instruction [CodetrixStudio/CapacitorGoogleAuth](https://github.com/CodetrixStudio/CapacitorGoogleAuth)
