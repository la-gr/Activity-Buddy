# Activity-Buddy
Activity-Buddy  is a web application designed to connect users for specific activities. It allows individuals to create a simple profile and then find a partner based on the activity they want to do, with optional filters for personality, skills, and availability. The core feature is a weighted preference system that allows users to prioritize what matters most to them in a "buddy."

Core Features User Authentication: Secure sign-up and login functionality for new and returning users.

User Profiles: Simple profiles that capture essential information: nickname, pronouns, personality, and skills.

Activity-Based Matching: The primary function requires users to state what activity they want a buddy for.

Advanced Filtering: Users can refine their search with optional preferences:

Partner's Personality

Partner's Skills

Preferred Time Slot

Weighted Preference System: Users can adjust the importance level of the optional filters, giving them control over the matching algorithm's priorities.

User Workflow The application flow is designed to be simple and intuitive, consisting of the following pages and steps:

Page 1 & 2: Landing / Authentication Choice

A user first arrives at a landing page.

They are presented with two options: Log In or Sign Up.

If Log In is chosen: The user enters their email and password and is taken directly to the Final Matching Page.

If Sign Up is chosen: The user is directed to the Sign-Up Page.

Page 3: Sign-Up Page

New users create their profile by providing the following information:

Email

Password

Nickname

Pronouns

Personality (e.g., introvert, creative, analytical)

Your Skills (e.g., Python, guitar, public speaking)

Upon successful submission, the user is automatically logged in and directed to the Final Matching Page.

Page 4 & 5: The Final Matching Page

This is the main page of the application where the user can find a buddy.

Mandatory Field:

Enter activity that you want to do: The user must fill this in to proceed (e.g., "Study for chemistry exam," "Play tennis," "Practice a presentation").

Optional Filters with Importance Levels:

Partner's Personality: The user can specify a desired personality type.

Partner's Skill: The user can look for a buddy with a specific skill.

Preferred Time Slot: The user can select a desired day or time.

For each of these three optional filters, the user can adjust a slider or a setting to indicate its importance (e.g., Low, Medium, High).

When the user clicks "Match," the system searches for other users based on their criteria, prioritizing the filters marked as more important.

Clarifications & Design Considerations This section clarifies assumptions made from the initial description and highlights key questions to consider during development.

Personality & Skills Input: How will users input their personality and skills?

Option A: Free Text: Users type whatever they want. (Easy to implement, but hard to match accurately).

Option B: Tags/Dropdowns: Users select from a predefined list of options. (Better for matching, but less flexible).

Recommendation: Use a tag-based system where users can select multiple predefined tags.

The Matching Algorithm: The core logic of the app will depend on how the "importance level" translates into search results. We need to define how a high-importance filter for "Skill" will weigh against a low-importance filter for "Time Slot."

Displaying Results: What happens after a user clicks "Match"? A fifth page or a section on the current page should display a list of potential buddies, showing their relevant information.

Connecting Buddies: How do matched users contact each other? The application will need a simple messaging system or a way to share contact information securely.
