# expo-apple-auth Build error
To replicate error upon upgrading XCode to iOS18.  The error is related to the [`expo-apple-authentication`](https://docs.expo.dev/versions/latest/sdk/apple-authentication/) package based on error:

> error: unexpected service error: The Xcode build system has crashed. Build again to continue.

```
❌  (node_modules/expo-apple-authentication/ios/AppleAuthenticationExceptions.swift:53:3)

  51 |
  52 | func exceptionForAuthorizationError(_ error: ASAuthorizationError) -> Exception {
> 53 |   switch error.code {
     |   ^ switch must be exhaustive
  54 |   case .unknown:
  55 |     return RequestUnknownException()
  56 |   case .canceled:
```

› Compiling expo Pods/Expo » Expo-dummy.m

## To run
- `yarn`
- `npx expo run:ios`

