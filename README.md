[README.txt](https://github.com/user-attachments/files/23698247/README.txt)
# Passenger Profile Management (ABAP)

A SAP ABAP application for managing passenger profiles, updating personal data, and handling reservations. Designed for SAP MM and PtP environments, this program combines object-oriented ABAP, selection screens, ALV grids, and interactive popups.

---

## Features

- **Passenger Profile Management**
  - Update personal details: name, document type/number, email, phone, and password.
  - Real-time validation for emails and document formats.

- **Reservation Management**
  - View all reservations in ALV grid.
  - Cancel reservations directly from the grid with confirmation popup.

- **Data Validation**
  - Checks email format.
  - Validates ID card or passport number based on document type.

- **User Interaction**
  - Popup messages for errors, confirmations, and notifications.

---

## Technologies & SAP Components

- **ABAP Reports** – Classical dynpro report structure.
- **ABAP Objects** – Event handler class for ALV grid interaction (`LCL_EVENT_HANDLER`).
- **ALV Grid (`CL_GUI_ALV_GRID`)** – Display and manage reservations.
- **Custom Containers (`CL_GUI_CUSTOM_CONTAINER`)** – Embed ALV controls.
- **Custom DDIC Tables** – `ZZZ_PASS_TAB` (passenger data), `ZZZ_RESERVATIONS` (reservation data).
- **SAP Standard Functions** – `POPUP_TO_CONFIRM`, `POPUP_TO_DISPLAY_TEXT` for user feedback.
- **Selection Screens** – Interactive user input with field validation.

---

## 📄 How It Works

1. User logs in with passenger ID and password.
2. Passenger data is loaded and displayed on the selection screen.
3. Users can update their details and validate inputs.
4. Reservations are displayed in an ALV grid with options to cancel.
5. All actions provide immediate feedback via popups.

---

## Future Improvements

- Add password encryption and improved security.
- Expand reservation management with seat availability checks.
- Integrate with other SAP modules for full airline management workflows.

---
