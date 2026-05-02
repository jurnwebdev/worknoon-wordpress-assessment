# worknoon-wordpress-assessment

## Overview

This project is a responsive landing page built using WordPress and Elementor as part of the Worknoon assessment. The goal was to deliver a clean, modern, and responsive layout while maintaining scalability, performance awareness, and SEO readiness.

---

## Features

* Hero section with strong call-to-action (CTA)
* Services section showcasing offerings
* Testimonials section for social proof
* Contact form integration
* Fully responsive across mobile, tablet, and desktop

---

## System Architecture Overview

The project is built using a containerized WordPress environment to ensure consistency and portability.

* **Frontend**: WordPress + Elementor (visual builder)
* **Backend**: PHP (WordPress core)
* **Database**: MySQL
* **Environment**: Docker
* **Version Control**: GitHub repository

This setup ensures the project can be easily reproduced and deployed across different environments.

---

## Tools & Technologies Used

* **WordPress**: Content management system for rapid development
* **Elementor**: Visual page builder for responsive UI design
* **JetFormBuilder**: Contact form handling
* **LiteSpeed Cache**: Performance optimization (caching, minification)
* **Google Site Kit**: Analytics and performance insights
* **Docker**: Containerized development environment for consistency

---

## Setup Instructions

### Option 1: Using Duplicator (Recommended)

#### Requirements

* PHP 7.4+
* MySQL / MariaDB
* Local server (XAMPP, MAMP, Laragon) OR Docker

#### Steps

1. Clone this repository
2. Place files in your server directory (e.g., `htdocs/` or `www/`)
3. Create a new empty database
4. Visit:

   ```
   http://localhost/your-folder-name/installer.php
   ```
5. Enter database credentials and run deployment
6. Access WordPress dashboard:

   ```
   http://localhost/your-folder-name/wp-admin
   ```

---

## Challenges Encountered & Solutions

### 1. Docker Environment Conflicts

* **Issue**: Running multiple WordPress instances caused port conflicts
* **Solution**: Assigned unique ports and container names for each instance

### 2. Data Persistence Issues

* **Issue**: Containers resetting caused loss of WordPress data
* **Solution**: Implemented volume mapping to persist files and database

### 3. "Bad Request" Header Error

* **Issue**: Browser cookies exceeded header size limits
* **Solution**: Cleared browser cookies and ensured isolated environments per project

### 4. File Access for Version Control

* **Issue**: WordPress files were initially stored inside Docker volumes
* **Solution**: Mapped WordPress directory to local project folder for GitHub tracking

---

## SEO & Schema Considerations

* Structured content hierarchy (H1, H2, H3) for clarity
* Clean section-based layout for crawlability
* Mobile responsiveness to meet Google indexing requirements
* Performance optimization via caching and minimized assets

---

## Design & Responsiveness

The layout was built using a modular approach to ensure:

* Reusability of sections
* Easy scalability into a multi-page website
* Consistent spacing, typography, and alignment

Responsive design was tested across:

* Mobile devices
* Tablets
* Desktop screens

---

## Notes for Reviewers

* This project focuses on layout structure, responsiveness, and system thinking
* Built with scalability and SEO readiness in mind
* Demonstrates practical use of WordPress in a containerized environment

---

## Plugins

* Elementor (UI/UX design)
* JetFormBuilder (forms)
* LiteSpeed Cache (performance)
* Google Site Kit (analytics)

---

## Admin Access

```
URL: /wp-admin
Username: tobi
Password: worknoon
```

---

## Author

**Tobi John**
Frontend Developer & WordPress Specialist
Portfolio: [https://tobijohn.com](https://tobijohn.com)
