# FUNPLAY

FUNPLAY is a Flutter + Supabase social, chat and games MVP branded with the FUNPLAY/SACHIN gaming emblem.

## Included
- Email signup/login/logout
- User profiles
- Image posts
- Feed with refresh
- Like/unlike with counts
- Comments
- Public chat rooms
- Realtime room messages
- Quiz game
- Bottom navigation
- FUNPLAY logo asset
- Basic validation and user-friendly error states

## Setup
1. Install Flutter and Android Studio.
2. Create a Supabase project.
3. Run `supabase/database.sql` in Supabase SQL Editor.
4. Create a public Storage bucket named `posts`.
5. Enable Realtime for the `messages` table.
6. Run:

```bash
flutter pub get
flutter run --dart-define=SUPABASE_URL=YOUR_URL --dart-define=SUPABASE_ANON_KEY=YOUR_ANON_KEY
```

For a release build:

```bash
flutter build appbundle --release --dart-define=SUPABASE_URL=YOUR_URL --dart-define=SUPABASE_ANON_KEY=YOUR_ANON_KEY
```

The AAB is normally produced at `build/app/outputs/bundle/release/app-release.aab`.

## Important
This package is a strengthened MVP source package, not a verified Play Store submission. A real release still needs Android signing, package/application ID configuration, production Supabase configuration, privacy policy, store listing assets, device testing, and Play Console review.

Never put a Supabase service-role key in the app. Use only the publishable/anon client key on the client.
