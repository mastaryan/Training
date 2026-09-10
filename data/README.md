# Data layer (platform contract)

Weeks, profiles, tenants, and assignments live here as JSON.
The athlete UI (`today.html`) reads these files. Logs stay in the browser
until a real backend exists (`localStorage` key `platform_logs_v1`).

| File | Purpose |
|---|---|
| `tenant-demo.json` | White-label skin + catalog (demo) |
| `profile-caynan.json` | Athlete profile, tests, maxes, entitlements |
| `assignment-caynan.json` | Which week is live |
| `week-4.json` | Custom week as data (source of Today) |

Demo video URLs are public Summers/Vimeo examples. Production tenants replace the library.
Custom weeks are coach-written. Templates are buy-and-run.
Athlete keeps logs if they leave; they do not keep program IP unless the tenant sells buyout/subscription.

Dummy logins remain in `toohey-app.html` until go-live auth.
Parent view: `today.html?view=parent`
