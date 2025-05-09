# Airbnb Clone Backend

This is the backend implementation of the **Airbnb Clone** project. It covers the core functionalities of a rental marketplace, including user management, property listings, booking management, payment processing, and more.

---

## 🔑 Core Functionalities

### 1. User Management
- **User Registration**: Users can sign up as either guests or hosts.
- **Authentication**: Secure login with email/password using JWT. OAuth (e.g., Google, Facebook) support available.
- **Profile Management**: Users can update their profiles, including profile photo, contact information, and personal preferences.

### 2. Property Listings Management
- **Add Listings**: Hosts can add listings with title, description, location, price, amenities, and availability.
- **Edit/Delete Listings**: Hosts can update or remove listings.

### 3. Search and Filtering
- **Search Filters**:
  - Location
  - Price Range
  - Number of Guests
  - Amenities (e.g., Wi-Fi, pool, pet-friendly)
- **Pagination**: Efficient loading of large datasets.

### 4. Booking Management
- **Create Bookings**: Guests can book properties for specific dates.
- **Avoid Double Booking**: Date validations to prevent overlaps.
- **Cancel Bookings**: Guests or hosts can cancel bookings per the policy.
- **Booking Status**: Tracks statuses such as pending, confirmed, canceled, or completed.

### 5. Payment Integration
- **Secure Payments**: Guests make upfront payments using Stripe, PayPal, etc.
- **Host Payouts**: Hosts receive payments after completed bookings.
- **Multi-currency Support**: Payment in various currencies.

### 6. Reviews and Ratings
- Guests leave ratings and reviews for properties.
- Hosts can respond to reviews.
- Reviews are linked to bookings to prevent misuse.

### 7. Notifications System
- **Email and In-App Notifications**:
  - Booking confirmations
  - Cancellations
  - Payment updates

### 8. Admin Dashboard
- Admins can monitor and manage:
  - Users
  - Listings
  - Bookings
  - Payments

---

## 🛠️ Technical Requirements

### 1. Database Management
- **Database**: MySQL or PostgreSQL
- **Tables**:
  - Users
  - Properties
  - Bookings
  - Reviews
  - Payments

### 2. API Development
- **RESTful API** with:
  - `GET` – Retrieve data
  - `POST` – Create data
  - `PUT/PATCH` – Update data
  - `DELETE` – Remove data
- **Optional**: GraphQL support for complex queries

### 3. Authentication and Authorization
- **JWT** for user sessions.
- **RBAC**: Role-Based Access Control to separate permissions for guests, hosts, and admins.

### 4. File Storage
- Profile pictures and property images stored via local or cloud (e.g., AWS S3 or Cloudinary).

### 5. Third-Party Services
- Email services like **SendGrid** or **Mailgun** for email notifications.

### 6. Error Handling and Logging
- Global error handling for API routes.
- Structured logging for easier debugging and monitoring.

---

## 🚀 Non-Functional Requirements

### 1. Scalability
- Modular architecture for easy scaling.
- Load balancers for horizontal scalability.

### 2. Security
- Passwords and sensitive data are encrypted.
- Rate limiting and firewalls for protection.

### 3. Performance Optimization
- **Caching**: Redis for caching frequent queries.
- **Query Optimization**: Minimized DB load and efficient indexing.

### 4. Testing
- Unit and integration testing using **pytest** or equivalent.
- Automated API testing for endpoint validation.

---