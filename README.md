# HTML-CSS-JS-Project.
#Design an Event Webpage using HTML and CSS and JavaScript
Creating an event webpage is an exciting way to showcase information about an event, including its schedule, speakers, and contact details.

What We’re Going to Create
We’ll create a webpage for a fictional event called "MyCompany 2025." This webpage will include

A header introducing the event.
Navigation links for different sections (About, Schedule, Speakers, and Contact).
A schedule table.
A contact form
Project Preview
<img width="1918" height="910" alt="image" src="https://github.com/user-attachments/assets/1d084d33-3d70-4459-8c15-67027d7a45c1" />
<img width="1900" height="898" alt="image" src="https://github.com/user-attachments/assets/ebd0a2fe-8a83-41b3-95e0-8f0819ac33ef" />
<img width="1900" height="885" alt="image" src="https://github.com/user-attachments/assets/4c8e06ab-b6a6-44cd-ac06-a4a1ca130fc9" />
#HTML CODE
<html>
<head></head>
<body>
    <link rel="stylesheet" href="registration.css">
    <script src="registration.js"></script>
    <header>
        <h1>Welcome to MyCompany 2025</h1>
        <p>The Ultimate Technology and Programming Conference</p>
    </header>
    <nav>
        <a href="#about">About</a> |
        <a href="#schedule">Schedule</a> |
        <a href="#speakers">Speakers</a> |
        <a href="#contact">Contact</a>
    </nav>
    <section id="about">
        <h2>About the Event</h2>
        <p>MyCompany Tech Summit 2025 is the premier gathering that unites leading minds in programming, cutting-edge technology, and innovation.<br><br>

Join us for an immersive day featuring:<br>

Insightful Talks: Hear from industry pioneers and thought leaders.<br>

Hands-on Workshops: Gain practical skills with deep-dive technical sessions.<br>

Networking Opportunities: Connect with fellow technology enthusiasts and professionals from around the world.<br>

Don't miss this chance to learn, collaborate, and shape the future of tech</p>
    </section>
    <section id="schedule">
        <h2>Event Schedule</h2>
        <style>
        /* CSS to add borders to the table */
        table {
            border-collapse: collapse; /* This makes the borders single-lined */
            width: 100%;
        }

        th, td {
            border: 1px solid black; /* Sets a 1-pixel solid black border */
            padding: 8px;           /* Adds space inside the cells */
            text-align: left;       /* Aligns text to the left */
        }

        th {
            background-color: #f2f2f2; /* Optional: Light grey background for headers */
        }
    </style>
        <table>
            <thead>
                <tr>
                    <th>Time</th>
                    <th>Session</th>
                    <th>Contest</th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td>9:00 AM</td>
                    <td>Opening Keynote</td>
                    <td>GeeksforGeeks Coding Plateform</td>
                </tr>
                <tr>
                    <td>10:30 AM</td>
                    <td>Understanding AI and Machine Learning</td>
                    <td>Mr. Arvind Kumar</td>
                </tr>
                <tr>
                    <td>1:00 PM</td>
                    <td>Lunch Break</td>
                    <td>-</td>
                </tr>
                <tr>
                    <td>2:00 PM</td>
                    <td>Exploring the Future of Cloud Computing</td>
                    <td>Ms. Neha Gupta</td>
                </tr>
            </tbody>
        </table>
    </section>
    <section id="speakers">
        <h2>Meet the Speakers</h2>
        <ul>
            <li><strong>Dr. Radhika Sharma:</strong> AI Expert and Researcher</li>
            <li><strong>Mr. Arvind Kumar:</strong> Senior Data Scientist at TechWave</li>
            <li><strong>Ms. Neha Gupta:</strong> Cloud Computing Specialist at CloudTech</li>
            <li><strong>Mr. Sandeep Reddy:</strong> Full Stack Developer and Open-Source Contributor</li>
        </ul>
    </section>
    <section id="contact">
        <h2>Contact Us</h2>
        <form>
            <style>
        /* Apply the font to the main elements */
        label, input, textarea, button {
            font-family: 'Lucida Console', Monaco, monospace;
        }

        /* Optional: Makes the input fields and button look uniform with the monospaced font */
        input[type="text"],
        input[type="email"],
        textarea,
        button {
            padding: 5px;
            border: 1px solid #ccc;
        }

        button {
            cursor: pointer;
            background-color: #f0f0f0;
        }
    </style>
        <label for="name">Name:</label><br>
        <input type="text" id="name" name="name">
        <span id="name-error" style="color: red; font-size: 0.9em;"></span><br><br>
        
        <label for="email">Email:</label><br>
        <input type="email" id="email" name="email">
        <span id="email-error" style="color: red; font-size: 0.9em;"></span><br><br>
        
        <label for="message">Message:</label><br>
        <textarea id="message" name="message" rows="4"></textarea><br><br>
        
        <button type="submit">Send</button>
        </form>
    </section>
</body>
</html>

#CSS CODE
<html>
<head>

    <title> MyCompany 2025</title>
    <style>
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            margin: 0;
            padding: 0;
            background-color: #f4f6f9;
            color: #444;
        }
        header {
            background-color: peachpuff;
            color: black;
            padding: 25px 0;
            text-align: center;
            box-shadow: 0 4px 6px rgba(156, 142, 152, 0.488);
        }
        header h1 {
            margin: 0;
            font-size: 2.5rem;
        }
        nav {
            background-color: rgb(173, 49, 49);
            /* Dark Gray */
            text-align: center;
            padding: 12px 0;
        }
        nav a {
            color: #ffffff;
            text-decoration: none;
            margin: 0 20px;
            font-weight: 600;
            font-size: 1.1rem;
            letter-spacing: 0.5px;
        }
        nav a:hover {
            color: #ff6347;
            /* Tomato */
            text-decoration: underline;
        }
        section {
            padding: 25px;
            margin: 20px auto;
            max-width: 900px;
            background-color: #ffffff;
            border-radius: 8px;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
            transition: box-shadow 0.3s ease;
        }
        section:hover {
            box-shadow: 0 6px 18px rgba(0, 0, 0, 0.15);
        }
        section h2 {
            color: #007bff;
            /* Bright Blue */
            font-size: 1.8rem;
            margin-bottom: 15px;
        }
        table {
            width: 100%;
            border-collapse: collapse;
            margin-top: 15px;
        }
        table th,
        table td {
            border: 1px solid #ddd;
            padding: 12px;
            text-align: left;
        }
        table th {
            background-color: #f1f1f1;
            font-weight: 600;
            color: #333;
        }
        table tr:nth-child(even) {
            background-color: #f9f9f9;
        }
        ul {
            list-style: none;
            padding: 0;
        }
        ul li {
            margin: 12px 0;
            font-size: 1.2rem;
        }
        ul li strong {
            color: #007bff;
        }
        form {
            max-width: 650px;
            margin: 25px auto;
        }
        form label {
            display: block;
            margin-bottom: 8px;
            font-weight: 600;
        }
        form input,
        form textarea,
        form button {
            width: 100%;
            padding: 14px;
            margin-bottom: 18px;
            border: 1px solid #ddd;
            border-radius: 8px;
            font-size: 1rem;
        }
        form input:focus,
        form textarea:focus {
            border-color: #007bff;
            outline: none;
        }
        form button {
            background-color: #007bff;
            color: white;
            font-size: 1.1rem;
            font-weight: 600;
            border: none;
            cursor: pointer;
            transition: background-color 0.3s ease;
        }
        form button:hover {
            background-color: #0056b3;
        }
        form button:active {
            background-color: #004085;
        }
    </style>
</head>
<body>
    <header>
        <h1>Welcome to MyCompany 2025</h1>
        <p>The Ultimate Technology and Programming Conference</p>
    </header>
    <nav>
        <a href="#about">About</a>
        <a href="#schedule">Schedule</a>
        <a href="#speakers">Speakers</a>
        <a href="#registration">Registration</a>
        <a href="#contact">Contact</a>
    </nav>
    <section id="about">
        <h2>About MyCompany 202
5</h2>

#JAVASCRIPT CODE
// Function to validate the form before submission
function validateForm(event) {
    // 1. Prevent the default form submission behavior (stops the page reload)
    event.preventDefault();

    // 2. Get the values from the input fields
    const nameInput = document.getElementById('name');
    const emailInput = document.getElementById('email');
    const messageInput = document.getElementById('message');

    const nameValue = nameInput.value.trim();
    const emailValue = emailInput.value.trim();
    
    // Clear any previous error messages
    document.getElementById('name-error').textContent = '';
    document.getElementById('email-error').textContent = '';
    
    let isValid = true; // Flag to track overall validity

    // --- Validation Checks ---

    // Check if Name is empty
    if (nameValue === "") {
        document.getElementById('name-error').textContent = 'Name is required.';
        nameInput.focus();
        isValid = false;
    }

    // Check if Email is empty
    if (emailValue === "") {
        document.getElementById('email-error').textContent = 'Email is required.';
        emailInput.focus();
        isValid = false;
    } 
    // Check for a basic email format using a simple Regular Expression (Regex)
    else if (!isValidEmail(emailValue)) {
        document.getElementById('email-error').textContent = 'Please enter a valid email address.';
        emailInput.focus();
        isValid = false;
    }

    // --- Final Action ---

    if (isValid) {
        // If all checks pass:
        alert('Form submitted successfully!\nName: ' + nameValue + '\nEmail: ' + emailValue + '\nMessage: ' + messageInput.value);
        
        // In a real application, you would send the data to a server here.
        // event.target.submit(); // Uncomment this line to submit the form normally
    }
}

// Helper function to check email format with Regex
function isValidEmail(email) {
    // Basic regex pattern: checks for text@text.domain
    const emailPattern = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
    return emailPattern.test(email);
}

// 3. Attach the validation function to the form's submit event
// (This must run AFTER the form is loaded, so putting the script at the end is best)
document.addEventListener('DOMContentLoaded', () => {
    const contactForm = document.querySelector('form');
    // Add an event listener for when the form attempts to submit
    contactForm.addEventListener('submit', validateForm);
});


