# Lil iLL

Backend developer at **Directam** · Isfahan, Iran

I build APIs with PHP and Laravel, with a focus on correctness under concurrent requests, queues, and caching. I work in Scrum teams.

**Stack:** PHP, Laravel, MySQL, Redis, Sanctum, Pest/PHPUnit

## Projects

### [appointment](https://github.com/Artashok11228/appointment)

JSON API for booking appointments, with queued email notifications and hourly scheduled jobs.

- Laravel, Sanctum, rate limiting, admin statistics
- Bookings run in a transaction with `lockForUpdate` on the service row to prevent double booking
- Concurrency test: two parallel processes book the same slot, exactly one wins

### [Url-Shortener](https://github.com/Artashok11228/Url-Shortener)

URL shortener with a public redirect path, a web dashboard, and a Sanctum API.

- Laravel, Redis cache, queued click tracking with retries
- Ownership policies, link expiry (`410`), OpenAPI docs, CI on GitHub Actions
- Removed N+1 queries on the dashboard (41 queries down to 2)

### [appointment-front-end](https://github.com/Artashok11228/appointment-front-end)

React client for the appointment API, built with AI assistance as a demo UI.
