# CapacitorGoogleAuth
Capacitor plugin for Google Auth.

> ⚠️ This is fork original plugin [@codetrix-studio/capacitor-google-auth](https://github.com/CodetrixStudio/CapacitorGoogleAuth) as temporally solution for support **Capacitor 3**

fork features:
  - support **Capacitor 3** (tested only **ios** and **web**)
  - [#102](https://github.com/CodetrixStudio/CapacitorGoogleAuth/pull/102) lazy loading with manual `init` hook
  - [#103](https://github.com/CodetrixStudio/CapacitorGoogleAuth/pull/103) updated deps
  - [#104](https://github.com/CodetrixStudio/CapacitorGoogleAuth/pull/104) debug info if `GoogleService-Info.plist` not found


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
#### Example Vue 3
```ts
import { defineComponent, onMounted } from 'vue'
import { GoogleAuth } from '@reslear/capacitor-google-auth'

export default defineComponent({
  setup() {
    onMounted(() => {
      GoogleAuth.init()
    })
    
    const logIn = async () => {
      const response = await GoogleAuth.signIn()
      console.log(response)
    }
    
    return {
      logIn
    }
  }
})
```

### Config, IOS, ANDROID and etc..

see originally instruction [CodetrixStudio/CapacitorGoogleAuth](https://github.com/CodetrixStudio/CapacitorGoogleAuth)
