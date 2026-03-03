## Sprint Status
 
| Sprint | Version | Status | Story Points | Key Deliverables |
|--------|---------|--------|--------------|------------------|
| Sprint 1 | v0.1.0-sprint1 | ✅ Complete | 42/42 | Backend foundation, MongoDB, Cloudinary, Email, Models, Category API |
| Sprint 2 | v0.2.0-sprint2 | ✅ Complete | 70/70 | Auth middleware, Services API, Providers API, Booking API, Docker |
| Sprint 3 | v0.3.0-sprint3 | ⬜ Upcoming | 0/TBD | Booking journey, Reviews, Profiles |
| Sprint 4 | v0.4.0-sprint4 | ⬜ Upcoming | 0/TBD | Dashboards, Notifications |
| Sprint 5 | v0.5.0-sprint5 | ⬜ Upcoming | 0/TBD | Payments, User Verification AI |
| Sprint 6 | v1.0.0         | ⬜ Upcoming | 0/TBD | Final polish, deployment |
 
## API Endpoints (Sprint 2)
 
### Public (no auth required)
| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | /health | Server health check |
| GET | /api/categories | List all categories |
| GET | /api/services | List/search services |
| GET | /api/services/:id | Get single service |
| GET | /api/providers | List all providers |
| GET | /api/providers/search | Search providers |
| GET | /api/providers/:id | Get single provider |
| GET | /api/profile/providers | List providers (profile view) |
| GET | /api/profile/provider/:id | Single provider profile |
 
### Protected (Bearer token required)
| Method | Endpoint | Role | Description |
|--------|----------|------|-------------|
| GET | /api/profile/me | any | Get current user profile |
| GET | /api/profile/users | any | List customers |
| GET | /api/profile/user/:id | any | Single user profile |
| POST | /api/services | provider | Create service |
| PUT | /api/services/:id | provider | Update service |
| DELETE | /api/services/:id | provider | Delete service |
| GET | /api/bookings | any | List my bookings |
| POST | /api/bookings | customer | Create booking |
| PUT | /api/bookings/:id/accept | provider | Accept booking |
| PUT | /api/bookings/:id/reject | provider | Reject booking |
