# Frontpage 

index.md

# Login Page (login.html)
The login page allows users to authenticate by entering their User ID and Password. Upon submitting the form, the provided credentials are sent to a backend server for authentication. If the login is successful, the user is redirected to the database page. If there is an error, it is logged in the console.

# Create User (createuser.html)

This page allows new users to sign up by entering their User ID, Password, and Full Name.

The form is centered on the page with a clean, modern look. Inputs and buttons have a consistent design with padding and rounded corners. Form elements are styled for readability and ease of use.

Users fill in their details and click "Create User" to submit the form. The form data is sent to a backend server for user creation and storage in the user database (SQLite). On success, users are redirected to the login page.

This page allows users to create and customize button designs interactively.

# Create Design (createDesign.html)

Layout
- Slider Container: Left section for customizing button properties.
- Button Container: Right section for previewing the button.
- Popup: Form for entering design details (name, description, type).

Customization Options
- Sliders and color pickers to adjust button width, height, button color, text color, border color, and border width.
- Real-time button preview

Animation
- Canvas for drawing animation paths.
- Preview and generate CSS animation code.
Popup Form
- Upon opening of page
- Collects design name, description, and type (public/private).
- Submits design details to the server
## JavaScript
Event Listeners
- Update button preview on input changes
- Handle drawing on the canvas for animations
Fetch Requests
- Send design data to the server to save & store the design in database

# Search for Designs (search.html)

This HTML page provides a search interface with toggle buttons to filter results between public and private designs. It includes a search bar, toggle buttons, and a results table. Users can like or dislike designs directly from the table.

Key Features
- Search Bar: Users can input search terms to find specific designs
- Toggle Buttons: Users can switch between "Public" and "Private" designs to search for
- Results Table: Displays the filtered search results in HTML table with columns for name, content, description, likes, dislikes, and type
- Like/Dislike Functionality: Buttons to like or dislike each design, with counts displayed
JavaScript Functions
- toggleButtons(activeButtonId): Highlights the selected toggle button
- checkButton(): Determines which button is active and fetches the appropriate designs
- getPublic() and getPrivate(): Fetch public or private designs from the server using GET and PUT respectively
- displayDataInTable(data): Displays the search results in a table, filtered through for name and content by the search term
- toggleLike(button, name) and toggleDislike(button, name): Handle liking and disliking designs

# Edit User Profile (editprofile.html)

This HTML page provides a user interface for editing a profile, including updating the username, password, and profile picture. The page contains input fields for entering a new name and password, as well as an option to upload a new profile picture. The user can also retrieve their current profile picture.

Key Features
- Form Fields: Allows users to input a new name and password.
- Image Upload: Users can upload a new profile picture.
- Retrieve Profile Picture: Displays the current profile picture.
Styling
- Basic CSS styles for form elements, buttons, and general layout.
