<h1 align="center">📚 StudySpace - Social Networking for Students</h1>

---

## 📝 Description

I have built a new social networking website called **StudySpace**. It's a study forum where users can ask questions, share knowledge, and connect with others to learn and clear their doubts across various academic and professional subjects.

The website offers six distinct subject forums:

1. Mathematics and Engineering  
2. Science and Technology  
3. Humanities and Social Sciences  
4. Business and Economics  
5. Health and Wellness  
6. Arts, Media, and Entertainment  

When users click on any of these subject categories, they are redirected to the specific chat forum where they can post their doubts, seek answers from other users, or contribute by answering questions.  
This feature encourages interaction and knowledge-sharing within a focused community of learners.

The website operates entirely on a **single HTML page**, using JavaScript to dynamically update content.  
It has five main pages:

- Home Page  
- Register Page  
- Login Page  
- Forum Page  
- Friends Page

---

## 🔧 Technologies used to create the website

- **Front-end**: HTML, CSS, JavaScript  
- **Back-end**: Node.js, Express.js  
- **Database**: MongoDB Compass  
- **Communication**: AJAX for seamless interaction between the client and server
---
 

## 🚀 Walk-through of the Platform

<h3>Home page:</h3>  
The Home Page serves as the entry point to the website where users can register or log in to access other features. Without logging in, users cannot view or interact with the Forum Page or Friends Page, ensuring that only registered users can participate in discussions and networking.  
<br></br>
<div align="center">
<img src="https://i.imgur.com/9b9E9Ut.png" width="80%" alt="StudySpace Home Page"/>
</div>

<br/>

<h3>Register and Login page:</h3>  
During registration users must provide a username, password, and email, all of which
undergoes validation. The username must be at least 6 characters long, while the email is
validated against a robust pattern to ensure proper formatting. Passwords must be at least 6
characters long and include both letters and numbers. Additionally, the system prevents
duplicate accounts by checking for existing usernames or email addresses before creating a
new account. After successfully registering the user is then redirected to the login page.
<br></br>
Error handling during registration is comprehensive with clear error messages provided for
missing fields, invalid email format, weak passwords, and duplicate credentials. This ensures
that users receive immediate feedback and can correct issues before proceeding.
<br></br>
<div align="center">
<img src="https://i.imgur.com/Lhd7dbX.png" width="80%" alt="Register page"/>
<img src="https://i.imgur.com/vrZNUuC.png" width="80%" alt="Login page"/>
</div>

<br/>

<h3>Home page after logging in:</h3>  
Once a user logs in, they are directed to the authenticated Home Page, which serves as the central hub for navigation. From here, users can access the Forum Page to post or view questions, visit the Friends Page to manage follow/unfollow interactions, or log out securely.
<br></br>
The logout functionality is securely implemented — destroying the session and clearing session cookies upon logout. This ensures that users are completely logged out and prevents any unauthorized access. Additionally, the system includes error handling to notify users in case any issue occurs during the logout process.
<br></br>
<div align="center">
<img src="https://i.imgur.com/7TzuQTY.png" width="80%" alt="Home page after logging in"/>
</div>

<br/>

<h3>Forum Page:</h3>  
The Forum Page is the core of StudySpace, featuring six distinct subject categories. When a user clicks on a subject, they are redirected to its dedicated chat forum where they can:

- **Post questions or answer other users' questions.**

- **Upload files or images** to provide additional context or explanations for their posts.  
  A **"Remove File"** button allows users to delete any file mistakenly selected.

- **Use the Search Bar** to filter through discussions.  
  The search feature dynamically matches the user’s query with existing posts, displaying relevant results.  
  If no match is found, a message is shown saying **“No discussion found.”**

- **Sort discussions using the Sort Button:**  
  → When the button says **“Sort by Latest”**, clicking it will arrange posts from newest to oldest.  
  → When it says **“Sort by Oldest”**, clicking will organize discussions from oldest to newest.
<br></br>
<div align="center">
<img src="https://i.imgur.com/lwZTiP8.png" width="80%" alt="Forum page"/>
<img src="https://i.imgur.com/39h62Io.png" width="80%" alt="Forum Page"/>
<img src="https://i.imgur.com/T79wIiK.png" width="80%" alt="Forum page"/>
<img src="https://i.imgur.com/MTTLer7.png" width="80%" alt="Forum page"/>
<img src="https://i.imgur.com/yoE7XyT.png" width="80%" alt="Question input box in forum page"/>
</div>

<br/>


<h3>Friends page:</h3>
The Friends Page enables users to build their network by following or unfollowing other users. Key features include:

- **Follow/Unfollow Functionality:**  
  Users can follow others, and the action is reflected in both the **Following** and **Followers** counters.  
  These counters dynamically update to show the correct numbers for both the user and the person being followed or unfollowed.

- **Search Bar:**  
  Users can search for other registered users to follow by typing their names in the search bar.
<br></br>
<div align="center">
<img src="https://i.imgur.com/KxozKzG.png" width="80%" alt="Friends page"/>
</div>


<br/>

<h3>Advanced feature:</h3> 
I have also implemented an advanced feature when a user tries to highlight a word with their
mouse cursor a pop-up box appears showing the word’s meaning and synonyms. This
functionality is made possible using the Free Dictionary API.
<br></br>
<div align="center">
<img src="https://i.imgur.com/MS1lRyH.png" width="80%" alt="Question input box"/>
</div>

<br/>

<h3>Web scraping for weather data:</h3> 
The StudySpace website features real-time weather updates displayed on the navigation bar
using data fetched from the Open-Meteo API. When the page loads a request is made to fetch
the current weather information for a specific city (Dubai, in this case). The API provides
details such as temperature and weather conditions (e.g., clear sky, rain, etc.).
If the data is not available or outdated the website fetches new weather information from the
Open-Meteo API which is a free and reliable service for weather forecasts. The weather data is
then saved in MongoDB to ensure the website does not repeatedly make external API requests
optimizing performance.
<br></br>
The weather data is cached in MongoDB with a timestamp, so it is only fetched from the API
again if the existing data is older than one hour. This caching mechanism helps to improve
response time and reduce unnecessary API calls. The updated weather information is displayed
on the navbar for the user to view easily.
<br></br>
<div align="center">
<img src="https://i.imgur.com/n1AjoMr.png" width="80%" alt="Question input box"/>
</div>

---

## **🔒 Full source code available in a private repository. Please contact me for access.**

