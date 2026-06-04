ArtComm will be a Python-Flask-based Progressive Web Application (PWA) that allows users to:
* Register and log in securely.
* Private message between artist and customers.
* Record the transactions of orders.
* Manage and track the orders directly.
* Set up personal profile, commission menu, TOS, prices.

***Key Features***
The key features of ArtComm are:
* Functional:
	* User authentication, Secure transaction, Promoting commissions, Personal profile, Manage Orders.
* Performance: 
	* Fast load times, responsive user interface, offline access via service workers.
	* 
- Security
	- Password hashing, input validation, session management, protection against SQL injection.
- Privacy
	- Compliance with the Australian Privacy Act 1988.
	- Competition and Consumer Act 2010 (cth).

***User Experience***
Users are guided in detail for each section, such as registration, login, how to purchase, how to pay, how to edit their profile, Terms of Service, and where to manage orders. Users will be able to access the application from any device, with offline functionality enabled through PWA caching. Additionally, users will be notified via email of any unexpected events such as problematic transactions, artist/customer accounts being flagged as spam, or signs of fraud.

***Technologies***
ArtComm will be based on the following 3rd-part technologies:
- Backend: Python, Flask
- Frontend: HTML5, CSS3, JavaScript
- Database: SQLite
- Authentication: Flask-Login
- Offline support: Service Workers, Web App Manifest
