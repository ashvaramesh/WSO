# Learning Journal for Waukegan Symphony Orchestra Website Project

## Week 3: Learning Web Dev

### Tutorials, Articles, or Videos Completed:
- [The Odin Project: Introduction to HTML and CSS](https://www.theodinproject.com/paths/foundations/courses/foundations/lessons/html-foundations)
- [Traversy Media: HTML Crash Course](https://www.youtube.com/watch?v=UB1O30fR-EE)

### Key Takeaways:
- Learned how to create a basic HTML structure and apply CSS for styling.
- Key concepts: tags, elements, selectors, properties, and basic layout using Flexbox.
  
### Challenges Faced:
- Struggled with responsive design when trying to use media queries for different screen sizes.
  
### How This Knowledge Will Apply:
- I will use this to ensure the Waukegan Symphony Orchestra homepage and ticket purchasing system are fully responsive.

### Code Snippets/Prototypes:
- coming soon.

import SwiftUI

struct LoginView: View {
    @State private var username: String = ""
    @State private var password: String = ""

    var body: some View {
        VStack {
            TextField("Username", text: $username)
                .padding()
                .textFieldStyle(RoundedBorderTextFieldStyle())

            SecureField("Password", text: $password)
                .padding()
                .textFieldStyle(RoundedBorderTextFieldStyle())

            Button(action: {
                // Handle login action
            }) {
                Text("Login")
                    .padding()
                    .background(Color.blue)
                    .foregroundColor(.white)
                    .cornerRadius(8)
            }
        }
        .padding()
    }
}

This Week (9/16/24):

	•	Tutorial: HTML & CSS Basics - A guide on structuring content with HTML and styling it using CSS.
	•	Course: Responsive Web Design Principles - Focused on learning how to create responsive websites that adjust to different screen sizes and devices.
	•	Material: Bootstrap Documentation - A framework for designing responsive and mobile-first websites quickly and easily.

2. Key Concepts or Tools Learned

	•	HTML & CSS: Developed a deeper understanding of HTML tags for structuring web content (such as div, header, nav, and footer), and learned how to style these elements using CSS for colors, fonts, and layouts.
	•	Responsive Design: Gained insights into how to make a website adjust seamlessly across various screen sizes using media queries in CSS and responsive design frameworks like Bootstrap.
	•	Navigation Bar: Learned how to create a responsive navigation bar that adjusts based on the device’s screen width, making the site more user-friendly for mobile users.

Challenges Faced

	•	Cross-Browser Compatibility: Faced challenges ensuring that the website looks consistent across different web browsers (Chrome, Firefox, Safari). Learned to use browser developer tools to identify discrepancies and adjust CSS to fix layout issues.
	•	Responsive Design Issues: Implementing the layout for mobile devices proved tricky, especially when ensuring that all elements were correctly aligned. I resolved this by using Bootstrap’s grid system and media queries.
	•	CSS Flexbox & Grid: While attempting to organize the concert schedule section, it was difficult to align multiple elements dynamically. Overcame this by using Flexbox for the alignment of the schedule items and Grid for laying out the event details.

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
    <title>Waukegan Symphony Orchestra</title>
</head>
<body>
    <nav class="navbar navbar-expand-lg navbar-light bg-light">
        <a class="navbar-brand" href="#">WSO</a>
        <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarNav">
            <ul class="navbar-nav ml-auto">
                <li class="nav-item">
                    <a class="nav-link" href="#home">Home</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="#about">About</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="#concerts">Concerts</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="#contact">Contact</a>
                </li>
            </ul>
        </div>
    </nav>
</body>
</html>

<section id="concerts" class="container mt-5">
    <h2 class="text-center">Upcoming Concerts</h2>
    <div class="d-flex justify-content-around flex-wrap">
        <div class="card" style="width: 18rem;">
            <div class="card-body">
                <h5 class="card-title">Spring Concert</h5>
                <p class="card-text">March 25, 2024 - 7:00 PM</p>
                <a href="#" class="btn btn-primary">Get Tickets</a>
            </div>
        </div>
        <div class="card" style="width: 18rem;">
            <div class="card-body">
                <h5 class="card-title">Summer Gala</h5>
                <p class="card-text">June 15, 2024 - 6:00 PM</p>
                <a href="#" class="btn btn-primary">Get Tickets</a>
            </div>
        </div>
    </div>
</section>
