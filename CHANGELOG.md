# Change Log
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/)
and this project adheres to [Semantic Versioning](http://semver.org/).

## [1.4.0] - 2026-10-12
### Added
- Added authenticated profile (`GET /me`) and password change (`POST /change-password`).
- Added paginated movement search (`GET /account-entries`). Existing list endpoints remain available.
- Added dashboard summary, category totals and monthly totals.
- Defined inclusive UTC dates, ownership scope, pagination limits and signed-amount statistics in OpenAPI.
- Wallet balances use exact decimals instead of float.
- Password changes use the dedicated endpoint; `/updateUser` rejects nonempty password fields.
- All existing tokens must be renewed when deploying the updated microservice. Subsequent password changes invalidate all previously issued tokens.
- Movement creation and editing normalize type 1 as income and type 2 as expense; editing supports date and all optional references while keeping the wallet fixed.

## [1.3.1] - 2025-08-05
### Bugfix
- Publish compiled Angular package from dist folder

## [1.3.0] - 2025-08-05
### Added
- Auth endpoint

## [1.2.0] - 2025-05-26
### Added
- Added new fields to support wallet, category, store brand management functionality

## [1.1.0] - 2025-05-22
### Added
- Added new fields to support role management functionality

## [1.0.1] - 2025-05-21
### Added
- Added missing `id` field to `Role`
### Removed
- Removed invalid date-time field

## [1.0.0] - 2025-05-21
### Added
- Initial structure of calls to the different API endpoints
