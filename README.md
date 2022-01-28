# CapacitorGoogleAuth

Capacitor plugin for Google Auth.

> ⚠️ This is fork original plugin [@codetrix-studio/capacitor-google-auth](https://github.com/CodetrixStudio/CapacitorGoogleAuth) with new beta features, changes or experiments

### Install

```sh
npm i -D @reslear/capacitor-google-auth

npx cap sync
```

### WEB

Register plugin and manually initialize

```ts
import { GoogleAuth } from '@reslear/capacitor-google-auth';

GoogleAuth.initialize({
  client_id: 'xxxxxx-xxxxxxxxxxxxxxxxxx.apps.googleusercontent.com',
  scopes: ['profile', 'email'],
  grantOfflineAccess: true,
});
```

> see `initialize` method options - descriptions, examples, default values and types in `definition.ts`

Use it

```ts
GoogleAuth.signIn();
```

### Config, IOS, ANDROID and etc..

see originally instruction [CodetrixStudio/CapacitorGoogleAuth](https://github.com/CodetrixStudio/CapacitorGoogleAuth)
