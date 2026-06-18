# Complete Admin CMS & UI Redesign Prompt

You are working on the **MicroTech Solutions** website.

## 1. Fix Existing Backend Errors

Investigate and resolve all backend API errors.

Current issues:

* `/api/settings` returns 500
* `/api/projects` returns 500
* `/api/products` returns 500
* `/api/team?visible=true` returns 500

Tasks:

* Check API routes.
* Check database connection.
* Verify environment variables.
* Add proper error handling.
* Return meaningful JSON errors instead of generic 500 responses.
* Ensure every endpoint works correctly with GET, POST, PUT, PATCH, and DELETE where appropriate.

---

## 2. Remove Cloudflare Script

The project is trying to load:

`/cdn-cgi/challenge-platform/scripts/jsd/main.js`

This returns 404.

Remove every reference to this script because the site is not using Cloudflare Bot Protection.

There should be no request to `/cdn-cgi/*`.

---

## 3. Build a Complete Admin CMS

The admin panel should control **EVERY SINGLE ITEM** on the landing page without touching code.

The admin dashboard should include:

### Hero Section

Editable:

* Main heading
* Subheading
* Description
* CTA button text
* CTA button link
* Hero image
* Background image
* Background overlay
* Statistics
* Badges

---

### Navigation

Editable:

* Logo
* Company name
* Menu items
* Order
* Links
* CTA button

---

### About Section

Editable:

* Title
* Subtitle
* Description
* Images
* Company statistics
* Features
* Timeline
* Vision
* Mission

---

### Services

Admin should be able to:

* Add service
* Edit service
* Delete service
* Change icons
* Change images
* Change descriptions
* Reorder services

---

### Products

Admin should be able to:

* Add products
* Edit products
* Delete products
* Upload product images
* Set prices
* Set categories
* Set featured products
* Hide/show products

---

### Projects / Portfolio

Admin should be able to:

* Add projects
* Edit projects
* Delete projects
* Upload multiple images
* Change categories
* Change completion dates
* Add technologies used
* Add client names
* Add project descriptions

---

### Team

Admin should be able to:

* Add members
* Edit members
* Delete members
* Upload profile photos
* Set position
* Set social media links
* Hide/show members

---

### Testimonials

Editable:

* Customer name
* Position
* Company
* Rating
* Testimonial
* Customer photo

---

### FAQ

Admin should be able to:

* Add FAQ
* Edit FAQ
* Delete FAQ
* Reorder FAQ

---

### Contact Section

Editable:

* Phone
* Email
* Address
* Google Map
* Contact form recipient email
* WhatsApp number

---

### Footer

Editable:

* Logo
* Copyright
* Links
* Social media
* Newsletter
* Company description

---

### Global Website Settings

Admin should be able to manage:

* Company name
* Logo
* Favicon
* SEO title
* SEO description
* Keywords
* Google Analytics ID
* Meta tags
* Open Graph tags
* Social links
* Contact information

---

## 4. Media Library

Create a media manager.

Features:

* Upload images
* Upload videos
* Delete files
* Replace files
* Search files
* Folder organization
* Image optimization

---

## 5. Rich Text Editor

Every text field should support formatting:

* Bold
* Italic
* Underline
* Lists
* Tables
* Links
* Images
* Code blocks
* Headings

---

## 6. Live Preview

Every edit should have:

* Save Draft
* Publish
* Live Preview
* Auto Save

---

## 7. Authentication

Secure admin panel.

Features:

* Login
* Logout
* Password hashing
* Session management
* JWT or secure cookies
* Protected API routes
* CSRF protection
* Rate limiting

---

## 8. Remove Dark Mode

Completely remove Dark Mode.

Requirements:

* Remove dark theme toggle.
* Delete all dark mode CSS variables.
* Remove unused dark mode classes.
* Remove JavaScript controlling dark mode.
* Default to one professional light theme.

---

## 9. Redesign the UI

Current colors are too bright.

Replace them with a modern corporate palette.

Primary Colors:

* Light Blue: #4A90E2
* Smoke White: #F5F7FA
* White: #FFFFFF
* Black: #111111
* Dark Gray: #444444
* Border Gray: #E5E7EB

Guidelines:

* Soft gradients only.
* Minimal shadows.
* Plenty of white space.
* Rounded corners (10–14px).
* Smooth transitions.
* Professional appearance.
* Responsive across desktop, tablet, and mobile.

Avoid:

* Neon colors
* Oversaturated blues
* Bright cyan
* Bright backgrounds
* Excessive animations

---

## 10. Improve UX

Add:

* Skeleton loaders
* Toast notifications
* Empty states
* Loading indicators
* Confirmation dialogs
* Better error messages
* Responsive layouts
* Accessible forms
* Keyboard navigation
* ARIA labels

---

## 11. Code Quality

Refactor the project to use:

* Reusable components
* Clean folder structure
* Type safety (if using TypeScript)
* API validation
* Input sanitization
* Proper logging
* Consistent naming conventions
* Performance optimization
* Lazy loading
* Image optimization
* Caching where appropriate

---

## 12. Final Requirement

The final website should behave like a full Content Management System (CMS).

**Nothing on the landing page should require editing source code.**

Every visible element—including text, images, icons, buttons, links, colors (where appropriate), section visibility, order, and content—must be manageable from the admin dashboard through an intuitive interface.

The system should be production-ready, responsive, secure, maintainable, and visually polished with a clean, modern corporate design based on the Light Blue, Smoke White, White, and Black color palette.
