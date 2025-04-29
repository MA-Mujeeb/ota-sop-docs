# Standard Operating Procedure (SOP)

## Title: Flight Booking Process – Online Travel Agency (OTA)

### 1. Purpose
To outline the step-by-step procedure for booking flight tickets through the OTA platform, ensuring consistency, accuracy, and customer satisfaction.

### 2. Scope
This SOP applies to all customer support agents, travel consultants, and booking engine operations teams of the OTA.

### 3. Responsibility
- **Customer Support Team:** Assist customers during booking.
- **Technical Team:** Maintain API integrations with GDS/NDC systems.
- **Product Team:** Ensure UI/UX flow supports smooth bookings.

### 4. Tools/Systems
- OTA Website / Mobile App
- GDS/NDC API (Amadeus, Sabre, Travelport)
- Payment Gateway (Stripe, Razorpay, PayTabs, etc.)
- CRM & Ticketing Tools (Freshdesk, Zendesk)

### 5. Procedure

#### Step 1: Search Flights
- User enters origin, destination, dates, and passenger count.
- System fetches flights via GDS/NDC APIs.
- Results displayed sorted by price or airline.

#### Step 2: Select Flight
- User selects preferred flight(s).
- Fare rules, baggage details, cancellation policy displayed.

#### Step 3: Enter Passenger Details
- Passenger names, gender, date of birth.
- Contact details and special service requests.

#### Step 4: Payment
- User selects payment method.
- System initiates payment gateway transaction.
- On success, booking confirmation triggered.

#### Step 5: PNR Generation & Ticket Issuance
- System issues PNR via GDS/NDC.
- E-ticket emailed to user.
- Data pushed to CRM and analytics dashboards.

### 6. Exceptions
- Payment failure → Booking not confirmed.
- API timeout → Retry or switch GDS fallback.
- Seat unavailability → Alert and suggest alternatives.

### 7. Documentation and Logs
- Booking logs stored in database for 30 days.
- Payment logs stored per PCI-DSS compliance.
- Support tickets logged in CRM.

---

### ✅ Revision History

| Version | Date       | Description         | Author         |
|---------|------------|---------------------|----------------|
| 1.0     | 2025-04-29 | Initial SOP created | OTA Team       |

