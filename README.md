# Advanced HTML5 Elements and Forms

## Objectives
Implement HTML5 images, lists, tables, forms and input types.
Use form validation attributes.
Apply multimedia elements such as audio and video.

## Instructions

- Create an index.html file.
- Add an ordered list with roman numerals
- Add an external image from pexels.com
- Add a table of 5 contacts with; name, address, mobile and emails
- Add a registration form

>[!NOTE]
>  The registration form should have:
>- Name, email, password, and date fields.
>- A dropdown, radio buttons, and checkboxes.
>- Proper labels and placeholders.
>- Required fields and validation attributes.
>- Ensure proper indentation and commenting.
 
# Tasks
- Create a well-structured HTML5 document.
- Ensure semantic correctness.

Happy Coding! 💻✨



<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Advanced HTML5 Elements and Forms</title>
  <style>
    table, th, td {
      border: 1px solid #ccc;
      border-collapse: collapse;
      padding: 8px;
      text-align: left;
    }
    body {
      font-family: Arial, sans-serif;
    }
    h1, h2 {
      color: #333;
    }
  </style>
</head>
<body>

  <!-- Page Title -->
  <h1>Welcome to My HTML5 Page</h1>

  <!-- Ordered List with Roman Numerals -->
  <h2>Steps to Register</h2>
  <ol type="I">
    <li>Fill in personal details</li>
    <li>Select your preferences</li>
    <li>Agree to terms</li>
    <li>Submit the form</li>
  </ol>

  <!-- External Image from Pexels -->
  <h2>Sample Image</h2>
  <img src="https://images.pexels.com/photos/414171/pexels-photo-414171.jpeg" alt="Scenic landscape from Pexels" width="500">

  <!-- Table of Contacts -->
  <h2>Contact List</h2>
  <table>
    <thead>
      <tr>
        <th>Name</th>
        <th>Address</th>
        <th>Mobile</th>
        <th>Email</th>
      </tr>
    </thead>
    <tbody>
      <!-- Contact 1 -->
      <tr><td>Jane Doe</td><td>123 Main St</td><td>555-1234</td><td>jane@example.com</td></tr>
      <!-- Contact 2 -->
      <tr><td>John Smith</td><td>456 Oak Ave</td><td>555-5678</td><td>john@example.com</td></tr>
      <!-- Contact 3 -->
      <tr><td>Emily Davis</td><td>789 Pine Rd</td><td>555-8765</td><td>emily@example.com</td></tr>
      <!-- Contact 4 -->
      <tr><td>Michael Brown</td><td>321 Elm St</td><td>555-4321</td><td>michael@example.com</td></tr>
      <!-- Contact 5 -->
      <tr><td>Linda White</td><td>654 Cedar Ln</td><td>555-1111</td><td>linda@example.com</td></tr>
    </tbody>
  </table>

  <!-- Registration Form -->
  <h2>Registration Form</h2>
  <form action="/submit-registration" method="POST">
    
    <!-- Name -->
    <label for="name">Full Name:</label><br>
    <input type="text" id="name" name="name" placeholder="Jane Doe" required><br><br>

    <!-- Email -->
    <label for="email">Email:</label><br>
    <input type="email" id="email" name="email" placeholder="jane@example.com" required><br><br>

    <!-- Password -->
    <label for="password">Password:</label><br>
    <input type="password" id="password" name="password" placeholder="••••••••" minlength="6" required><br><br>

    <!-- Date -->
    <label for="dob">Date of Birth:</label><br>
    <input type="date" id="dob" name="dob" required><br><br>

    <!-- Dropdown (Country) -->
    <label for="country">Country:</label><br>
    <select id="country" name="country" required>
      <option value="">Select Country</option>
      <option value="usa">United States</option>
      <option value="uk">United Kingdom</option>
      <option value="canada">Canada</option>
      <option value="other">Other</option>
    </select><br><br>

    <!-- Radio Buttons (Gender) -->
    <label>Gender:</label><br>
    <input type="radio" id="female" name="gender" value="female" required>
    <label for="female">Female</label>
    <input type="radio" id="male" name="gender" value="male" required>
    <label for="male">Male</label>
    <input type="radio" id="other" name="gender" value="other" required>
    <label for="other">Other</label><br><br>

    <!-- Checkboxes (Interests) -->
    <label>Interests:</label><br>
    <input type="checkbox" id="coding" name="interests" value="coding">
    <label for="coding">Coding</label>
    <input type="checkbox" id="music" name="interests" value="music">
    <label for="music">Music</label>
    <input type="checkbox" id="travel" name="interests" value="travel">
    <label for="travel">Travel</label><br><br>

    <!-- Submit Button -->
    <button type="submit">Register</button>
  </form>

  <!-- Multimedia Section -->

  <!-- Video -->
  <h2>Featured Video</h2>
  <video controls width="500" poster="https://images.pexels.com/photos/414171/pexels-photo-414171.jpeg">
    <source src="https://www.w3schools.com/html/mov_bbb.mp4" type="video/mp4">
    Your browser does not support the video tag.
  </video>

  <!-- Audio -->
  <h2>Background Audio</h2>
  <audio controls loop>
    <source src="https://www.w3schools.com/html/horse.mp3" type="audio/mpeg">
    Your browser does not support the audio element.
  </audio>

</body>
</html>

