# TechVue- AI-mock-Interview
To access the project, visit the
https://ai-mock-interview-chi-sage.vercel.app/





# WorkFlow of The AI-mock-Interview



1. When you click the link, you'll be directed to the homepage.


<img width="1872" height="937" alt="Screenshot 2025-08-29 094412" src="https://github.com/user-attachments/assets/c2aa87a8-a7b2-4afc-bd41-541355c517e8" />




User logs in with Google Authentication (Clerk) → data securely stored in Convex Database.



<img width="1379" height="781" alt="Screenshot 2025-08-29 114646" src="https://github.com/user-attachments/assets/a6a02c12-cb23-4776-8647-844d7aa613da" />



On the Upload Page, the user uploads their resume (PDF/Docx).


<img width="1669" height="795" alt="Screenshot 2025-08-29 094619" src="https://github.com/user-attachments/assets/93b2bd59-38c2-4989-91fa-c3c35152a1f6" />


Resume data is processed by the n8n workflow + custom AI model to generate interview questions. Thats the Flow of genrating the Questions from Pdf

<img width="1503" height="758" alt="Screenshot 2025-08-22 052532" src="https://github.com/user-attachments/assets/5370d0f3-8d7e-4fde-8061-7b55ebf21b5c" />

After generating the questions, they are stored in the Convex database.

<img width="1920" height="1080" alt="Screenshot 2025-08-27 002011" src="https://github.com/user-attachments/assets/390f21b2-523d-4e61-b5d0-dd2d72ab46b3" />

Once the interview begins, the system pushes the questions—each tagged with a unique ID—to the AI Avatar. The Avatar then generates realistic voice and lip-sync responses, simulating a live mock interview experience.

<img width="1386" height="762" alt="Screenshot 2025-08-29 101415" src="https://github.com/user-attachments/assets/79e07ec9-cb99-4a10-889a-3a283600e843" />




The AI Avatar (voice-enabled) conducts the mock interview in real time.



<img width="3640" height="2098" alt="Ai-interview" src="https://github.com/user-attachments/assets/0b08119c-b4c0-4499-9820-87406262f268" />


User can alternatively input a job title + description, and n8n regenerates questions based on the new role.


<img width="1623" height="772" alt="Screenshot 2025-08-27 002922" src="https://github.com/user-attachments/assets/02dbe7fd-42af-4c4b-9cb7-7902260fff8d" />



After the session, personalized feedback (strengths, weaknesses, improvement areas) is generated and exported as a PDF.
The process can be repeated for multiple job roles and store all the records in updated Dashboard


