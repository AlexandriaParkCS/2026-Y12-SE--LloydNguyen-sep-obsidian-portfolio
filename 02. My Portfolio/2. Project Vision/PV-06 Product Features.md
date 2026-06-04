## Core Features

- **User Authentication:** Secure login and registration using hashed passwords, email, and choose their own username.
- **Transaction Recording:** Add, edit and delete payment methods. Bill for transferring and receiving money (Amount, recipient and sender account details, order details).
- **Promoting Commissions:** Upload the commission template (Price for Style Tiers: Chibi, Anime, Semi-realistic,...; Coverage Tiers: Headshot/Icon, Bust/Thigh-up, Full Body; Finish Tiers: Rough Sketch, Line, Flat Colours, Fully Rendered; Sample: examples of how they will look like).
- **Personal Profile:** Upload and pin commission menu. Add, edit and remove profile picture, name, biographic, other social media link.
- **Manage Orders:** The public timeline on personal profile - Show the number of order artist received and the process of the order (sketch, colour,... already done and gave it to the customer). 

## Supporting Features 

* **Responsive Interface:** Works across desktop and mobile devices.
* **Data Validation:** Ensures accuracy and prevents invalid entries.
* **Secure Storage:** All user data stored in a protected SQL database.
* **Error Messaging:** Clear instruction for invalid inputs or failed actions.
* **Report:** Allow users to report content that is inappropriate, or lacks warnings, contains AI content.
* **Feedback:** Let users to send feedback straight to allow users to send feedback directly to the developer's email – regarding bugs, new features, and areas for improvement.


## Constraints

- The system must use secure password hashing (e.g., bcrypt).
* The database must ensure the integrity and confidentiality of the relationship between artists and clients, transactions, and received orders.
- The interface must remain simple and accessible for new users.
- The application must operate within the capabilities of standard web browsers.

## Assumptions

- Users have basic digital literacy and access to an internet‑enabled device.
- Users will present their drawing skills and techniques in the most detailed and truthful way possible.
- Users must carefully consider whether the price they set for their artwork is appropriate for their skill level.
- The system will be implemented in a small context, targeting individuals interested in art, with quick online transactions.
- Future enhancements (e.g., recurring transactions, notifications, security upgrades) may be added without major architectural changes.
