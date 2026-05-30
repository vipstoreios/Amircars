# امیر کارس

Premium dark/gold car marketplace for Kia cargo trucks, built with SwiftUI, a static admin dashboard, and a Supabase backend contract.

## What Is Included

- iOS SwiftUI app in `AmirCarsApp/`
- Static admin dashboard in `admin-dashboard/`
- Supabase schema, RLS policies, storage setup, and seed settings in `supabase/`
- Localization for Kurdish Badini, Kurdish Sorani, and Arabic
- Phone number login and OTP verification UI
- Kia Bongo / Kia K2700 listing flow with USD prices
- Listing status system: available, sold, installment
- Chat models, chat UI, and realtime-ready service boundaries
- Verification request flow with ID card, selfie, ID number, full name, and phone fields
- Admin moderation for users, listings, verification requests, and message overview

## Repository Layout

```text
AmirCarsApp/
  App/
  Models/
  Views/
  Components/
  ViewModels/
  Services/
  Localization/
  Assets/
  Utilities/
admin-dashboard/
  index.html
  src/
    components/
    pages/
    services/
    styles/
    assets/
supabase/
  schema.sql
  policies.sql
  storage.sql
  seed.sql
  README.md
```

## Notes

The app ships with local Kia cargo truck sample data for UI testing only. The code is structured so `AuthService`, `CarService`, `ChatService`, `FavoriteService`, `VerificationService`, and `UserService` can be switched to Supabase calls without changing the views.
