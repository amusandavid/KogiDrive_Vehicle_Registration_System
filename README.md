# KogiDrive — Kogi State Online Vehicle Registration Number System

A responsive frontend mini-project demonstrating a proposed online vehicle-registration application workflow for Kogi State.

## Important prototype notice

**KogiDrive is an educational frontend prototype. It is not an official Kogi State Government or Federal Road Safety Corps service.** It does not connect to government systems, verify vehicle ownership, allocate legally valid plate numbers, approve official registrations, or process payments.

Use fictional/sample information only. The admin page is a demonstration interface without secure authentication. Records are stored in the current browser's `localStorage`, so they are not shared across devices or users and can be modified by anyone with access to the browser.

## Features

- Responsive homepage with service overview and FAQs.
- Three-step vehicle registration form.
- Applicant and vehicle detail validation.
- Unique demonstration application reference generation.
- Browser-based application storage using `localStorage`.
- Application tracking by reference number.
- Demo admin dashboard with live statistics.
- Search and status filtering.
- Application detail view and status updates (Pending, Approved, Rejected).
- Rejection reason field.
- Seeded sample records for exploring the dashboard.
- Confirmed reset of demo records.

## Technology

- HTML5
- CSS3
- Vanilla JavaScript
- Browser `localStorage`

No framework, backend, database, payment gateway, or build process is required.

## Folder structure

```text
kogidrive/
├── index.html
├── register.html
├── track.html
├── admin.html
├── css/
│   └── style.css
├── js/
│   ├── main.js
│   ├── storage.js
│   ├── registration.js
│   ├── tracking.js
│   └── admin.js
└── README.md
```

## How to run

1. Extract the ZIP file.
2. Open the `kogidrive` folder.
3. Open `index.html` in a modern browser.

For the most consistent local development experience, use Visual Studio Code with the **Live Server** extension:
1. Open the extracted project folder in VS Code.
2. Right-click `index.html`.
3. Choose **Open with Live Server**.

Use the same browser and origin when testing registration, tracking, and admin pages. Browser storage is scoped to the origin; opening the files through different methods or paths may create separate storage areas.

## Suggested test workflow

1. Open `admin.html` and review the sample records.
2. Open `register.html` and submit a fictional application.
3. Copy the generated reference number.
4. Open `track.html` and look up the new reference.
5. Open `admin.html`, search for the reference, and open its details.
6. Change its status to Approved or Rejected.
7. Return to `track.html` and search again to see the updated status.
8. Use **Reset demo data** on the admin page to restore the original sample records.

## Data storage

Application records are stored in this browser key:

```text
kogidrive_applications_v1
```

Clearing browser site data may remove the saved records. The reset button removes the demo collection and restores the sample records.

## Responsive design

The interface adapts to mobile, tablet, and desktop widths. The navigation collapses on small screens, form fields stack vertically, and admin records become mobile-friendly cards.

## Future production considerations

A real public service would require, at minimum:
- A secure backend and database.
- Proper staff authentication, authorization, and audit logs.
- Server-side validation and protection against tampering.
- Privacy notices, data-retention rules, and secure handling of personal information.
- Integration and authorization from the relevant government and vehicle-registration authorities.
- Official verification, payment, and plate-allocation workflows where applicable.

These capabilities are intentionally outside this HTML/CSS/JavaScript prototype.
