# Donovan Taylor
**Computer Science Professional & Cybersecurity Specialist**
[LinkedIn Profile Link] | [GitHub Profile Link] | dtaylor5269@gmail.com

---

## Professional Self-Assessment
Professional Self-Assessment
Completing the Computer Science program has been a transformative experience that has shaped not only my technical capabilities but also my core professional values. Throughout my coursework, I have developed a deep appreciation for the entire software development lifecycle, learning that true engineering goes beyond writing functional code. It requires an unwavering commitment to efficiency, scalability, and, above all, security. Developing this ePortfolio has allowed me to critically reflect on my growth and synthesize my diverse experiences into a cohesive professional identity: a software engineer who views every architectural decision through a security-first lens.

My technical foundation has been rigorously tested and refined through a variety of academic and practical challenges.

Collaborating in a Team Environment and Communicating with Stakeholders
Effective software engineering is fundamentally collaborative. During the creation of a comprehensive Software Design Document (SDD) for the Travlr Getaways web application, I gained vital experience translating complex technical architectures into clear, actionable requirements for diverse stakeholders. Furthermore, drafting incident analysis briefs for simulated enterprise data breaches taught me how to communicate critical technical risks and mitigation strategies to non-technical management, ensuring alignment between engineering teams and business objectives.

Data Structures and Algorithms
I approach problem-solving with a focus on computational efficiency. Beyond traditional sorting and searching implementations, I have applied advanced algorithmic principles in dynamic scenarios, such as developing a deep Q-learning model to train an intelligent agent to successfully navigate a complex maze. This experience reinforced my ability to select, implement, and optimize the precise algorithmic tools required for highly specialized computing problems.

Software Engineering and Database Management
My software engineering experience spans multiple paradigms and platforms. Developing a mobile application that utilized the Android SensorManager required strict adherence to mobile lifecycle management and robust software design patterns. In the realm of databases, I have learned to prioritize data integrity and normalization, ensuring that backend systems are structurally sound, scalable, and capable of supporting complex relational queries without compromising performance.

Security Mindset
Security is the cornerstone of my professional aspirations. My approach is deeply informed by industry standards, including the NIST Cybersecurity Framework and the core principles of the CIA triad (Confidentiality, Integrity, Availability). Designing a comprehensive Role-Based Access Control (RBAC) matrix for a simulated healthcare firm and developing actionable phishing incident response playbooks have instilled in me a proactive security posture. I do not view security as an afterthought; it is an integrated component of every line of code I write and every system I design.

ePortfolio Artifact Summary
The artifacts presented in this portfolio were carefully selected and enhanced to demonstrate a full spectrum of computer science competencies, functioning together to showcase a secure, efficient, and maintainable approach to software development.

Software Design and Engineering: The first artifact is an interactive 3D Still Life Scene built in C++ using OpenGL. I enhanced this project by migrating it from a procedural script to a robust Object-Oriented architecture. This demonstrates my ability to implement complex class hierarchies, manage memory safely using smart pointers, and design scalable, modular software that incorporates user interaction.

Algorithms and Data Structures: The second artifact is an Advising Assistance Course Planner. By replacing standard library sorting functions with a custom-built Binary Search Tree (BST), I optimized the application's data retrieval processes to run in linear time. This highlights my capability to manually engineer complex data structures to solve specific performance bottlenecks.

Databases: The final artifact is a data dashboard backend for an animal shelter. I completely re-architected this system from a flat NoSQL structure to a normalized SQLite relational database. By designing a secure, credential-free local connection and enforcing strict schema rules, this artifact serves as a practical demonstration of my ability to identify vulnerabilities and implement secure, structurally sound database solutions.

Together, these projects reflect my technical versatility and my readiness to contribute to a professional engineering team. I invite you to review these artifacts as a demonstration of my commitment to building software that is not only highly functional but structurally resilient and secure.

---

## Portfolio Artifacts

### 1. Software Design and Engineering: Interactive 3D Scene
**View Source Code:** [Insert Link to this specific GitHub Repository]

![Screenshot of 3D Scene](link_to_your_image.jpg) *(Note: Upload a screenshot of your scene to your repo and link it here)*

Milestone Two: Software Design and Engineering Narrative
Artifact Description The artifact selected for the Software Design and Engineering category is a 3D Still-Life Scene originally created for CS 330: Computational Graphics and Visualization. Written in C++ using the OpenGL library (utilizing GLEW and GLFW), the application renders a complex 3D scene consisting of a table, a bowl, and various fruits. The original iteration of the software was functionally sound but architecturally fragile; it relied on a monolithic, procedural design where all rendering logic was hardcoded directly into the main render loop.
Justification for Inclusion I selected this artifact because it presented a prime opportunity to demonstrate Refactoring and Software Architecture skills. In the industry, developers rarely write code from scratch; they more often inherit legacy codebases that need to be modernized.
Skills Showcased: By refactoring this artifact, I demonstrated proficiency in Object-Oriented Programming (OOP), specifically polymorphism, encapsulation, and inheritance. I also showcased modern C++ memory management by migrating from raw pointers to smart pointers (std::shared_ptr), ensuring resource safety.
Improvements: The most significant improvement was the transition from a procedural script to a modular class hierarchy. I created an abstract Shape base class with derived implementations for specific meshes (MeshCube, MeshSphere, etc.). The scene manager was updated to hold a dynamic vector of these shape objects, allowing the scene to be scalable. If I want to add 100 apples now, I simply instantiate them and add them to the vector, rather than writing 100 blocks of rendering code.
Course Outcomes Analysis With this enhancement, I successfully met the course outcome regarding "Design and evaluate computing solutions that solve a given problem using algorithmic principles and computer science practices."
Evaluation: I evaluated the trade-offs between the original procedural approach (which was faster to write initially but impossible to scale) and the new OOP approach (which required more initial setup but offers long-term maintainability).
Outcome Updates: My original plan focused heavily on just the visual aspect. However, during development, I expanded the scope to include User Interaction (Outcome 4: Innovative Techniques). I implemented an event listener that allows users to toggle the visual state of specific objects using keyboard inputs ('1', '2', '3'), transforming the artifact from a static image into an interactive application.
Reflection on the Process Refactoring this code was a lesson in the complexity of dependency management and the "hidden costs" of software development.
Challenges: The biggest challenge I faced was environmental configuration. Because the original project relied on external libraries linked via relative paths that no longer existed, I encountered significant "Linker Errors" and "File Not Found" exceptions. I had to investigate the directory structure to locate the missing ShapeMeshes and ShaderManager dependency files and manually relocate them to the source directory where the solution file was expecting them.
Debugging: I also encountered a critical runtime error (Access Violation code -1073741819) caused by an uninitialized pointer in my new SceneManager constructor. This reinforced the importance of Defensive Programming, ensuring all objects are properly instantiated before usage.
Key Takeaway: Through this process, I learned that clean code is not just about readability; it is about safety. By encapsulating the drawing logic inside the Shape classes, I prevented the main loop from accidentally corrupting the state of an individual object, significantly increasing the robustness of the application.



---

### 2. Algorithms and Data Structures: Course Planner (BST)
**View Source Code:** [Insert Link to this specific GitHub Repository]

![Screenshot of Terminal Output](link_to_your_image.jpg) *(Note: Take a screenshot of the console printing the sorted courses)*

**Artifact Description**
[PASTE THE "Artifact Description" PARAGRAPH FROM YOUR ALGORITHMS NARRATIVE]

**Justification for Inclusion**
[PASTE THE "Justification for Inclusion" PARAGRAPH]

**Course Outcomes Analysis**
[PASTE THE "Course Outcomes Analysis" PARAGRAPH]

**Reflection on the Process**
[PASTE THE "Reflection on the Process" PARAGRAPH]

---

### 3. Databases: Secure Animal Shelter Dashboard
**View Source Code:** [Insert Link to this specific GitHub Repository]

![Screenshot of Database Schema or Dashboard](link_to_your_image.jpg) *(Note: A screenshot of the dashboard running or your SQLite table structure)*

**Artifact Description**
[PASTE THE "Artifact Description" PARAGRAPH FROM YOUR DATABASES NARRATIVE]

**Justification for Inclusion**
[PASTE THE "Justification for Inclusion" PARAGRAPH]

**Course Outcomes Analysis**
[PASTE THE "Course Outcomes Analysis" PARAGRAPH]

**Reflection on the Process**
[PASTE THE "Reflection on the Process" PARAGRAPH]

---
*Created for CS 499: Computer Science Capstone*
