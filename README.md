# BZ Audio

Cinematic music-technology storefront and platform.

## Supabase platform foundation
Project: `cgakpcvptyhxwfujzqoe` (us-west-2)

Includes Auth, role-aware profiles, products, product files, collections, coupons, orders, order items, licenses, downloads, homepage sections, analytics events, audit logs, RLS policies, and storage buckets for public artwork/previews plus private product files.

The storefront now loads published products from Supabase and includes BZ Account sign-up/sign-in, a customer Library view, admin-gated command center, product publishing controls, search, and a persistent shopping bag.

## Security
Authorization uses `app_metadata.role`, not editable `user_metadata`. Supabase service-role and Stripe secret keys must remain server-side.

## Remaining production connection
Stripe must be connected for live checkout, webhook fulfillment and payment/refund flows. A server-side signed-download endpoint and admin upload UI should then be added.
