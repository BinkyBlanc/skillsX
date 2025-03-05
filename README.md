# SkillsX
SkillsX is an app prototype that combines networking, knowledge-sharing, and personal growth into one seamless experience. 


# How it Works:

**1. Create a Profile:** Start by creating a personal profile that outlines your skills, interests, and background. The more detailed and up-to-date your profile is, the better you’ll connect with others who share similar or complementary expertise.

**2. Search and Connect:** Use the search function to find individuals who match your interests, skills, or career goals. You can easily send a message or start a conversation to explore potential collaboration opportunities or gain advice.

**3. Interact and Rate:** After engaging in a conversation or collaboration, rate the interaction using the star system. Your feedback helps others gauge the quality of connections, while also helping to build your own reputation in the community.

**4. Grow Your Network:** As you engage with others, skillsX recommends more potential connections based on the data from your interactions. This continuous cycle of connection and feedback ensures a rich, engaged community where people share and learn from each other.

**5. Update Your Profile:** Keep your profile up-to-date with your latest achievements, skills, or interests. This allows other users to see your growth and stay current on your expertise.

--------------------------------------------------------------------

# Software Architecture Design


<p align="center">
  <img src="https://github.com/user-attachments/assets/528d1eac-f899-406d-ac7b-0f87f4c5405c"/>
</p>

--------------------------------------------------------------------

# Database Design

<p align="center">
   <img src="https://github.com/user-attachments/assets/5063c01f-3d11-4bc5-9c26-23ed61b5f7c8"/>
"/>
</p>

--------------------------------------------------------------------

# Architecture Pattern 

<p align="center">
   <strong><img src = "https://github.com/user-attachments/assets/4b763ba4-3326-4cea-b6cb-e5305d58927d"/></strong>
</p>


# MVVM (Model-View-ViewModel)

**API**: Centralized API handling and Firebase integration.


**Models**: Defines data structures like user, chat, and message models.


**ViewModels**: Encapsulates business logic and manages app state for features like authentication, 
<p>chat messaging, filters, recommendations, profiles, and user ratings.</p>


**Views**: UI screens categorized into features (e.g., chat, filters, profile, recommendations.


**Widgets**: Reusable UI components to ensure consistency and reduce duplication.


**Helpers**: Utility functions for validation, constants, and the recommendation engine logic (cosine similarity).


**Main Files**: firebase_options.dart for Firebase configuration and main.dart as the app’s entry point.




