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

struct LoginView_Previews: PreviewProvider {
    static var previews: some View {
        LoginView()
    }
}


import SwiftUI

struct MenuView: View {
    var body: some View {
        NavigationView {
            List {
                NavigationLink(destination: ProfileView()) {
                    Text("Profile")
                }
                NavigationLink(destination: SettingsView()) {
                    Text("Settings")
                }
            }
            .navigationTitle("Menu")
        }
    }
}

struct MenuView_Previews: PreviewProvider {
    static var previews: some View {
        MenuView()
    }
}


Learning Journal

1. Tutorials, Courses, and Materials

This Week (9/16/24):

	•	Tutorial: SwiftUI Basics - Introduction to building user interfaces with SwiftUI.
	•	Course: iOS Development with Swift - Focused on building iOS apps using Swift.
	•	Material: Apple’s SwiftUI Documentation - Official documentation for SwiftUI components and usage.

2. Key Concepts or Tools Learned

	•	SwiftUI: Understanding of basic SwiftUI components like Text, Button, and VStack.
	•	Navigation: Implemented navigation between different views using NavigationView and NavigationLink.
	•	State Management: Learned to manage state with @State and @Binding properties in SwiftUI.

Challenges Faced:

	•	State Binding Issues: Encountered difficulties with binding state variables between views. Resolved by thoroughly understanding @Binding and using it appropriately.
	•	Navigation Implementation: Faced challenges in properly setting up NavigationView for seamless transitions between views. Overcame by consulting documentation and examples.

