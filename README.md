# SkillsX
SkillsX is an app prototype that combines networking, knowledge-sharing, and personal growth into one seamless experience. 

<p align="center">
   <strong>How it Works:</strong>
</p>

**1. Create a Profile:** Start by creating a personal profile that outlines your skills, interests, and background. The more detailed and up-to-date your profile is, the better you’ll connect with others who share similar or complementary expertise.

**2. Search and Connect:** Use the search function to find individuals who match your interests, skills, or career goals. You can easily send a message or start a conversation to explore potential collaboration opportunities or gain advice.

**3. Interact and Rate:** After engaging in a conversation or collaboration, rate the interaction using the star system. Your feedback helps others gauge the quality of connections, while also helping to build your own reputation in the community.

**4. Grow Your Network:** As you engage with others, skillsX recommends more potential connections based on the data from your interactions. This continuous cycle of connection and feedback ensures a rich, engaged community where people share and learn from each other.

**5. Update Your Profile:** Keep your profile up-to-date with your latest achievements, skills, or interests. This allows other users to see your growth and stay current on your expertise.

--------------------------------------------------------------------

<p align="center">
   <strong>Software Architecture Design</strong>
</p>


<p align="center">
  <img src="https://github.com/user-attachments/assets/97647304-7441-4c66-beb1-030cff6b0568"/>
</p>

--------------------------------------------------------------------

<p align="center">
   <strong>Database Design</strong>
</p>

<p align="center">
   <img src=""/>
</p>

--------------------------------------------------------------------

<p align="center">
<strong>Design Pattern</strong>

<p align="center">
   <strong><img src = "https://github.com/user-attachments/assets/46a48efa-aa88-4c50-af2d-9de33ae4405c"/></strong>
</p>


**MVVM (Model-View-ViewModel) architectural pattern**

api/:

Centralizes API logic, including Firebase connections and general API handling.

Ensures all network-related code resides in one place, making it reusable and easy to manage.

models/:

Contains data models like user_attribute, chat_user, and message, representing the structure and properties of the app’s data.

Simplifies data handling across the app by standardizing the way data is represented.

viewmodels/:

Houses application logic and state management for specific features like authentication, chat, filtering, recommendations, profiles, and ratings.

Separates the logic from UI, ensuring a clean and testable structure.

views/:

Organized into subfolders for different features (e.g., auth, chat, filters, etc.), containing individual screens like log_screen or chat_home.

Focuses purely on displaying data and interacting with the user.

widgets/:

Contains reusable UI components such as star_rating_widget and chat_bubble_widget.

Encourages consistency in design and reduces code duplication.

helpers/:

Includes utility files and helper functions like cosine_similarity (recommendation engine logic) and validator (input validation).

Keeps reusable logic separate from feature-specific code.

firebase_options.dart:

Manages Firebase configuration, typically generated when integrating Firebase into the app.

main.dart:

The entry point for the app, where the app is bootstrapped and the primary widget tree is defined.
