---
updated: 2026-08-06
---
# Vendor Billing App
- Idea to build a billing app for local vendors, with a friend
- User and friend have strong existing contacts with local vendors
- Those vendors currently do billing and records on paper books
- Concept: app gets molded to each vendor's needs, all data stored in cloud
- Plans to vibe code it
- "Molded" means 10-15 premade templates picked via setup questions, not per-vendor custom builds
- Believes the main pain with existing apps is having to type everything manually
- Planned flow: barcode photo scan (OpenCV Python script running locally) pulls product data, vendor enters price/discount, bill auto-generates and goes to the customer on WhatsApp
- Plans to use collected customer numbers so vendors can promote products directly on WhatsApp
- Scope includes both B2B and B2C management for the vendor
- Clarified the B2B side means upstream: vendors also track pending payments and inventory with their distributors
- Chose invoice-OCR (photograph the distributor's printed invoice) over onboarding distributors onto the app, since distributors already have their own systems
- App to be built in Expo, must run smoothly on low-end devices with no lag
- UI to ship in both Hindi and English
- PRD drafted (v1 scope: billing, distributor invoice OCR, unified ledger)
