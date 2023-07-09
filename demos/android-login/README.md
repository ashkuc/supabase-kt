# Android Login Demo

This is a demo of an android app using Google OneTap/Native Sign-In & WebView for authentication

**Available platforms:** Android

**Modules used:** GoTrue

https://user-images.githubusercontent.com/26686035/235766941-6a62c415-e07e-4d18-9706-0a246e6821eb.mp4

# Configuration

Then you need to specify your supabase url and key in [supabaseModule.kt](https://github.com/supabase-community/supabase-kt/blob/master/demos/android-login/common/src/commonMain/kotlin/io/github/jan/supabase/common/di/supabaseModule.kt)

### Google Sign In

Create an OAuth-Client Id for web application following [Supabase guide](https://supabase.com/docs/guides/auth/social-login/auth-google#configuration-web)

Create an OAuth-Client Id for android application with the packageName `io.github.jan.supabase.android` and your SHA1 fingerprint

SHA1 fingerprint can be obtained by running gradle task `signingReport`

Put in the **web client id** in `supabaseModule.kt` (not the android one)

### Spotify Sign In

For Spotify login you obviously need to enable that in the Supabase Dashboard, but you can replace that with any provider you want

# Running

Use the IDE to run the app.
