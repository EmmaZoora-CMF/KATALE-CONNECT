# Katale Connect

## Project Title

Katale Connect: A Mobile-First Web Directory for Informal Vendors in Kampala

## Abstract

Katale Connect is a coursework web prototype designed to improve the online visibility of informal vendors in Kampala. The system provides a lightweight, mobile-first directory that allows users to discover vendors by category, location, and keyword search. The solution is implemented as a static website using HTML and CSS, and is deployed through Firebase Hosting. This approach demonstrates how low-cost web technologies can support market sellers, tailors, repair technicians, food vendors, and other small businesses that commonly rely on walk-in traffic and word of mouth.

## 1. Introduction

Informal businesses are a major part of Kampala's local economy, but many of these vendors are difficult to discover online. Customers often spend time asking for directions or recommendations before finding suitable products and services. Katale Connect addresses this gap by offering a simple digital directory that can be accessed from any modern browser without the need to install a mobile application.

## 2. Problem Statement

Many informal vendors have limited digital presence, resulting in:

- Reduced customer reach
- Dependence on physical traffic and referrals
- Difficulty for customers to quickly locate trusted local services

## 3. Project Aim and Objectives

### Aim

To design and implement a mobile-first web directory that improves visibility and discoverability of informal vendors in Kampala.

### Specific Objectives

1. Provide vendor discovery through category, location, and keyword search paths.
2. Demonstrate vendor profile information such as business type, operating area, contacts, and status.
3. Include a listing submission flow for vendors who want to be added to the directory.
4. Deploy the solution using Firebase Hosting to validate web delivery of a static prototype.

## 4. Scope of the Project

The current implementation covers front-end pages and static sample content only. It demonstrates user navigation flows and content structure, but does not include a production backend database, authentication, or live moderation pipeline.

## 5. Methodology and System Design

The project follows a prototype-driven development approach:

1. Identify key user journeys (find vendor, compare vendor, contact vendor).
2. Build static page templates for each journey.
3. Apply a shared stylesheet for consistency and mobile-first presentation.
4. Configure Firebase Hosting for deployment with clean URLs.

### Core User Flow

1. User lands on the home page.
2. User navigates by search, category, or location.
3. User opens a vendor profile to view details.
4. User contacts vendor via provided channels.

## 6. Technologies Used

- HTML5 for semantic page structure
- CSS3 for layout and responsive styling
- Firebase Hosting for deployment and static site hosting

## 7. Project Structure

- firebase.json: Firebase Hosting configuration
- public/: Website source files
- public/assets/: Images and static media
- public/styles.css: Global stylesheet

### Main Pages

- public/index.html: Landing page and search entry
- public/categories.html: Category browsing page
- public/category.html: Single category listing view
- public/locations.html: Location browsing page
- public/search.html: Search results page
- public/vendor.html: Vendor profile page
- public/list-business.html: Business listing submission form
- public/submitted.html: Submission confirmation page
- public/about.html: About and process explanation
- public/contact.html: Contact and support form
- public/faq.html: Frequently asked questions
- public/privacy.html: Privacy policy page
- public/terms.html: Terms of use page
- public/404.html: Not found page

## 8. Implementation and Deployment

### Local Testing

This project can be tested locally using a static file server.

Option A: VS Code Live Server

1. Open the project in VS Code.
2. Right-click public/index.html.
3. Select Open with Live Server.

Option B: Python HTTP Server

1. Open a terminal in the project root.
2. Run:

   python -m http.server 8000 --directory public

3. Open http://localhost:8000 in a browser.

### Firebase Hosting Deployment

Current configuration in firebase.json:

- public directory: public
- cleanUrls: true
- trailingSlash: false

Deployment steps:

1. Install Firebase CLI:

   npm install -g firebase-tools

2. Authenticate:

   firebase login

3. Initialize hosting (if required):

   firebase init hosting

4. Deploy:

   firebase deploy

## 9. Results and Expected Impact

The prototype demonstrates that a simple web directory can make informal vendors easier to find. By providing structured listing pages and direct contact information, the platform can reduce customer search time and potentially improve business visibility for small-scale operators.

## 10. Limitations

- Static sample data only (no live data persistence)
- No authentication or role-based administration
- No automated verification workflow for submitted documents
- Placeholder contact details in prototype content

## 11. Recommendations for Future Work

1. Integrate a database (for example, Firebase Firestore) for dynamic listings.
2. Add an admin moderation dashboard for listing approval and verification.
3. Implement vendor self-service account management.
4. Add analytics to monitor search behavior and listing engagement.
5. Improve multilingual support and accessibility testing coverage.

## 12. Conclusion

Katale Connect provides a practical demonstration of how a mobile-first static web solution can address discoverability challenges for informal vendors in Kampala. Although currently a prototype, the project establishes a clear foundation for future expansion into a full production system with dynamic data and moderation workflows.

## References

- Firebase Hosting Documentation: https://firebase.google.com/docs/hosting
- HTML Living Standard: https://html.spec.whatwg.org/
- MDN Web Docs (HTML/CSS): https://developer.mozilla.org/
- HTML/CSS: https://www.w3schools.com/html/default.asp

## License

This project is intended for coursework and educational use.
