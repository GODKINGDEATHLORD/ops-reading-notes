

# Computer Network - AAA (Authentication, Authorization and Accounting)
 ![Alt text](image.png)

1. **Explain each of the three A’s as you would to a non-technical family member. Use an analogy or a story.**
   "Think of AAA like a club with a strict entry policy. **Authentication** is like the bouncer at the door checking your ID to make sure you're on the guest list. **Authorization** is once you're inside, the areas you're allowed to enter—like VIP areas—are based on your status. And **Accounting** is like the club keeping a record of when you entered, what you had, and when you left."

2. **What should the administrator do if the ACS server fails to authenticate a user during AAA implementation?**
   "If the ACS (Access Control Server) fails, it's like if the bouncer's guest list got wet and names are unreadable. The administrator should have a backup, like a secondary list or a way to verify guests (users) against another source—typically a local database on the device itself."

3. **What is the role of the NAS in the AAA implementation using an ACS server? Use a diagram.**
   "NAS (Network Access Server) in AAA is like the club's front desk, which communicates with the bouncer (ACS). It checks if you should be allowed in (Authentication) and what you can do inside (Authorization)."

  
# RADIUS Concepts

1. **What are the benefits of using RADIUS for authentication and authorization?**
   "RADIUS centralizes the management of user data, so it's like having a single, secure list of all the people allowed in multiple clubs. It simplifies management and enhances security."

2. **What is RADIUS and what does it stand for?**
   "RADIUS stands for Remote Authentication Dial-In User Service. Think of it as a way for people to prove who they are and gain the right access remotely, similar to having a keycard that works for multiple buildings."

3. **Research: What encryption algorithms does RADIUS use?**
   "RADIUS typically uses the MD5 hashing algorithm for encrypting passwords, but since it's not the most secure method by today's standards, it's often used within more secure frameworks."
