# IFQ636--Wedding-Guest-Manager

## Live Deployment URL 
- **AWS EC2 Public URL:** http://3.107.198.58/

## Setup and Local Execution
1. Clone the repository: `git clone https://github.com`
2. Open 'index.html' directly in any web browser, or via Python: 'sudo python3 -m http.server 80'

## Architecture Summary 
- **Frontend:** Single HTML page, CSS and JavaScript application presenting the Guest RSVP form ('IA1-3', 'IA1-7') and Host Dashboard ('IA1-5') aligned with the Figma prototype created
- **Hosting:** Deployed on AWS EC2 Ubuntu instance serving static web assets

## Known Limitations 
- **Unified Single-Page layout:** Both the Guest RSVP form and the Host Dashboard are rendered simultaneously on the same page rather than separate pages shown on the Figma prototype
- **RSVP Form Submission and Validation:** While the RSVP input fields and dashboard layout are implemented, the form submission handler and empty-field validation alerts are not yet wired dynamically to append entries to the Guest List table or update the Guest count
- **Lacking backend database:** No backend database is connected in this sample prototype; the data displayed represents static sample records.
- **Mock Dashboard Controls:** The PDF/CSV export buttons are mocked UI elements aligned with the Figma prototype
- **Unimplemented Row Editing:** The edit button, which allows the host to manually modify guest information in the guest list, is not included because the table displays static sample data without backend persistence.
- **Guest Capacity:** The web application is designed for a small capacity of 150 maximum of people, and therefore automated blocking of submissions will be implemented
