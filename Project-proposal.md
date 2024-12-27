   **Project Proposal: Pet Social Network**
   
**Description**
 * Pet lovers often lack a dedicated space to share their experiences and connect with like-minded individuals. This project aims to create a vibrant social networking platform where pet owners can celebrate their passion for animals. The app will allow users to create profiles for their pets, share photos, interact with other pet enthusiasts, and discover local pet events and news.
________________________________________
**Stack**
 * ***Frontend*** : React, JavaScript, HTML, CSS
 * ***Backend*** : Node.js, Express
 * ***Database*** : Postgresql
 * ***Additional Tools*** : pet news/event APIs
________________________________________
**Focus**
 * This will be an evenly focused **full-stack** application:
   * _Backend_: Manage user accounts, pet profiles, posts, comments, and integrations with external APIs.
   * _Frontend_: Provide an engaging and intuitive interface for users to explore and interact with the community.
________________________________________
**Type**
 * ***Web application***, with mobile responsiveness to ensure accessibility across devices.
________________________________________
**Goal**
 * To provide a fun and engaging platform for pet enthusiasts to:
   1. Share updates and photos of their pets.
   2. Discover local pet-related events and news.
   3. Connect with a supportive community of like-minded individuals.
________________________________________
**Users**
 * ***Primary Audience*** : Pet owners and animal lovers looking for a dedicated platform to celebrate their pets.
 * ***Secondary Audience*** : Pet service providers (e.g., vets, trainers) who might use the platform to connect with pet owners.
________________________________________
**Data**
 * ***Sources*** : Integrate external APIs for pet news and events (e.g., Google Calendar API for scheduling pet events, or a dedicated pet news API(NewsCatcher API)).
 * ***Collection Methods***:
   * User-generated data (pet profiles, posts, comments).
   * API requests to fetch and display news/events.
   * Internal database to store user, pet, and interaction data.
________________________________________
**Approach**
  **Database Schema**
   * **Users**: id, username, email, password, profile_picture
   * **Pets**: id, user_id, name, type, age, profile_picture, bio
   * **Posts**: id, user_id, content, image_url, timestamp
   * **Comments**: id, post_id, user_id, content, timestamp
   * **Events**: id, title, description, location, start_time, end_time, created_by
   * **Likes**: id, post_id, user_id
________________________________________
  **API Issues**
   * External APIs: Handling rate limits and authentication for pet news/event APIs.
   * Data Quality: Ensuring consistency in formatting fetched data for display.
________________________________________
  **Sensitive Information**
   * Encrypt passwords using bcrypt.
   * Use secure communication protocols (HTTPS) and secure tokens for API interactions.
   * Implement access control to prevent unauthorized data access.
________________________________________
**Functionality**
 1.	**Pet Profiles**: Users can create profiles for their pets, complete with images, names, and bios.
 2.	**Posts & Interactions**: Users can post updates, comment on posts, and like/dislike posts.
 3.	**Events Section**: Users can browse and RSVP to local pet-related events.
 4.	**Discovery Page**: Explore trending posts and featured pets.
 5.	**Notifications**: Receive updates about events, comments, and new followers.
________________________________________
**User Flow**
 * Sign-Up/Login: Users create an account with email and password.
 * Create Pet Profile: Add pets with pictures and details.
 * Engage with Community: Post updates, interact with other pet profiles, and comment on posts.
 * Discover Events: Find pet-friendly events or news relevant to their location.
 * Notifications: Stay updated with reminders and new activities on the platform.
________________________________________
