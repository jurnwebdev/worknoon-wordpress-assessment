# System Thinking & Project Reflection

## 1. Problem Overview

The task was to design and build a responsive landing page that includes a hero section with a clear call-to-action, services, testimonials, and a contact form. Although the scope was limited to a single page, the objective extended beyond visual design to include usability, responsiveness, and a structure that could support future scalability.

---

## 2. Approach (Architecture, Tools, Plugins)

I approached the solution using WordPress within a Docker environment to ensure isolation, and ease of setup. This allows the project to be easily shared and run consistently across without needing a server to work on.

For the frontend, I used a visual page builder (Elementor) to rapidly prototype and implement a responsive layout. This enabled efficient iteration on design while maintaining flexibility.

For functionality:

* JetFormBuilder plugin was used to create the contact form to handle user submissions
* Basic SEO considerations were included in structure, images naming, alt  and description.
* The layout was designed with reusable sections to allow expansion into a multi-page site if needed

---

## 3. Key Decisions and Why

* **WordPress over custom code**: Chosen for speed of development, ease of content management, and industry relevance
* **Docker setup**: Ensures environment consistency and avoids conflicts with existing local setups
* **Elementor (or page builder)**: Enabled rapid UI development and responsiveness without spending time on low-level styling

---

## 4. Tradeoffs Considered

* **Speed vs Flexibility**: Using a page builder introduces some performance overhead but significantly reduces development time
* **Plugins vs Custom Development**: Few Plugins were used for faster implementation, though custom development could offer better optimization
* **Simplicity vs Scalability**: While the page is simple, the structure was designed to support future expansion into a full website.
* **Site Kit Setup**: Couldn't setup the google analytics because I was working from a local server which google didn't support.

---

## 5. Challenges Encountered and Solutions

* **Docker configuration and port conflicts**: Running multiple WordPress instances required careful port management and container naming to avoid conflicts
* **Request header size error (Bad Request)**: This was resolved by clearing browser cookies and ensuring no conflicts between multiple local environments
* **File management for version control**: Adjusted volume mapping to ensure WordPress files were accessible locally for GitHub versioning

---

## 6. Affiliate Tracking / Onboarding System (Proposed Approach)

Although not implemented in this task, an onboarding or affiliate system could be integrated by:

* Creating a user registration flow using JetFormBuilder or any WordPress forms and custom post types for storing user meta data
* Tracking referrals via URL parameters and storing them in the database
* Integrating with tools like FirstPromoter or similar platforms via API or plugin
* Building a dashboard for users to track referrals and conversions

---

## 7. Experience with Tools like FirstPromoter

While FirstPromoter was not directly used in this project, I understand its role in managing affiliate tracking, referral attribution, and performance analytics. Integration into WordPress would involve connecting user actions (signups, purchases) to referral sources and ensuring accurate tracking through scripts or API connections.

---

## 8. What I Would Improve

If rebuilding the project, I would:

* Optimize performance by reducing reliance on heavy plugins and improving asset loading
* Implement advanced SEO features such as structured data (schema markup)
* Improve accessibility
* Build on a live server so that I would be able to setup google analytics properly

