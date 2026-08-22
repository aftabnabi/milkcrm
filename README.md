# milkcrm
**Fully working (from the base template):**
- Auth system: login, JWT/IdentityServer, roles, permissions, user management (Angular + backend)
- Settings, theming, notifications, i18n
- Database schema: `Customer`, `Order`, `OrderDetail`, `Product`, `ProductCategory` models with proper EF Core relationships, plus a migration already generated
-Generic repository pattern (`Repository<T>`) with full CRUD (Add/Update/Remove/Get/Find) already implemented and wired into a `UnitOfWork`
**Stubbed / unfinished (the actual CRM part):**
- `CustomerController` only has one real endpoint (`GET` all customers); the rest are leftover scaffold placeholders (`Post`, `Put`, `Delete` do nothing, `Get(id)` returns a literal string)
- No `OrderController` or `ProductController` exist at all, despite the ViewModels (`OrderViewModel`, `ProductViewModel`) and repositories already being scaffolded for them
 - `CustomerRepository.GetTopActiveCustomers()` throws `NotImplementedException`
 - Angular's Customers/Orders/Products pages are literal placeholders — Customers just renders a demo to-do widget, Orders/Products just show "-- Sample Page --" text. No API services, no data tables, no forms exist 
