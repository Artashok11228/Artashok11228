# Lil iLL

Backend developer at **Directam**.

I work with PHP and Laravel. Here are a few personal projects that show how I write APIs and keep concurrent requests safe.

## Projects

### [appointment](https://github.com/Artashok11228/appointment)

JSON API for booking appointments.

- Laravel, Sanctum, OpenAPI
- Bookings run in a database transaction with `lockForUpdate` on the service row to prevent double booking
- Unique index on active slots as a final safety net
- Tests run on GitHub Actions

### [Url-Shortener](https://github.com/Artashok11228/Url-Shortener)

URL shortener with a public redirect path and a Sanctum API.

- Laravel, Redis cache, queued click tracking
- Soft delete, expiry, and ownership policies
- OpenAPI docs and CI tests

### [appointment-front-end](https://github.com/Artashok11228/appointment-front-end)

React frontend for the appointment API.
