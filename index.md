# Donovan Taylor
**Computer Science Professional & Cybersecurity Specialist**
[LinkedIn Profile Link] | [[GitHub Profile]](https://github.com/Tiabkcilc) | dtaylor5269@gmail.com

---

## Professional Self-Assessment

Completing the Computer Science program has been a transformative experience that has shaped not only my technical capabilities but also my core professional values. Throughout my coursework, I have developed a deep appreciation for the entire software development lifecycle, learning that true engineering goes beyond writing functional code. It requires an unwavering commitment to efficiency, scalability, and, above all, security. Developing this ePortfolio has allowed me to critically reflect on my growth and synthesize my diverse experiences into a cohesive professional identity: a software engineer who views every architectural decision through a security-first lens.

My technical foundation has been rigorously tested and refined through a variety of academic and practical challenges.

**Collaborating in a Team Environment and Communicating with Stakeholders**
Effective software engineering is fundamentally collaborative. During the creation of a comprehensive Software Design Document (SDD) for the Travlr Getaways web application, I gained vital experience translating complex technical architectures into clear, actionable requirements for diverse stakeholders. Furthermore, drafting incident analysis briefs for simulated enterprise data breaches taught me how to communicate critical technical risks and mitigation strategies to non-technical management, ensuring alignment between engineering teams and business objectives.

**Data Structures and Algorithms**
I approach problem-solving with a focus on computational efficiency. Beyond traditional sorting and searching implementations, I have applied advanced algorithmic principles in dynamic scenarios, such as developing a deep Q-learning model to train an intelligent agent to successfully navigate a complex maze. This experience reinforced my ability to select, implement, and optimize the precise algorithmic tools required for highly specialized computing problems.

**Software Engineering and Database Management**
My software engineering experience spans multiple paradigms and platforms. Developing a mobile application that utilized the Android `SensorManager` required strict adherence to mobile lifecycle management and robust software design patterns. In the realm of databases, I have learned to prioritize data integrity and normalization, ensuring that backend systems are structurally sound, scalable, and capable of supporting complex relational queries without compromising performance.

**Security Mindset**
Security is the cornerstone of my professional aspirations. My approach is deeply informed by industry standards, including the NIST Cybersecurity Framework and the core principles of the CIA triad (Confidentiality, Integrity, Availability). 



Designing a comprehensive Role-Based Access Control (RBAC) matrix for a simulated healthcare firm and developing actionable phishing incident response playbooks have instilled in me a proactive security posture. I do not view security as an afterthought; it is an integrated component of every line of code I write and every system I design.

**ePortfolio Artifact Summary**
The artifacts presented in this portfolio were carefully selected and enhanced to demonstrate a full spectrum of computer science competencies, functioning together to showcase a secure, efficient, and maintainable approach to software development.

* **Software Design and Engineering:** The first artifact is an interactive 3D Still Life Scene built in `C++` using `OpenGL`. I enhanced this project by migrating it from a procedural script to a robust Object-Oriented architecture. This demonstrates my ability to implement complex class hierarchies, manage memory safely using smart pointers, and design scalable, modular software that incorporates user interaction.
* **Algorithms and Data Structures:** The second artifact is an Advising Assistance Course Planner. By replacing standard library sorting functions with a custom-built Binary Search Tree (`BST`), I optimized the application's data retrieval processes to run in linear time. This highlights my capability to manually engineer complex data structures to solve specific performance bottlenecks.
* **Databases:** The final artifact is a data dashboard backend for an animal shelter. I completely re-architected this system from a flat `NoSQL` structure to a normalized `SQLite` relational database. By designing a secure, credential-free local connection and enforcing strict schema rules, this artifact serves as a practical demonstration of my ability to identify vulnerabilities and implement secure, structurally sound database solutions.

Together, these projects reflect my technical versatility and my readiness to contribute to a professional engineering team. I invite you to review these artifacts as a demonstration of my commitment to building software that is not only highly functional but structurally resilient and secure.

---

## Portfolio Artifacts

### 1. Software Design and Engineering: Interactive 3D Scene
**View Source Code:** [Insert Link to this specific GitHub Repository]

![Screenshot of 3D Scene](link_to_your_image.jpg) *(Note: Upload a screenshot of your scene to your repo and link it here)*

### Software Design and Engineering Narrative

**Artifact Description**
The artifact selected for the Software Design and Engineering category is a 3D Still-Life Scene originally created for CS 330: Computational Graphics and Visualization. Written in C++ using the OpenGL library (utilizing GLEW and GLFW), the application renders a complex 3D scene consisting of a table, a bowl, and various fruits. The original iteration of the software was functionally sound but architecturally fragile; it relied on a monolithic, procedural design where all rendering logic was hardcoded directly into the main render loop.

**Justification for Inclusion**
I selected this artifact because it presented a prime opportunity to demonstrate Refactoring and Software Architecture skills. In the industry, developers rarely write code from scratch; they more often inherit legacy codebases that need to be modernized.
* **Skills Showcased:** By refactoring this artifact, I demonstrated proficiency in Object-Oriented Programming (OOP), specifically polymorphism, encapsulation, and inheritance. I also showcased modern C++ memory management by migrating from raw pointers to smart pointers (`std::shared_ptr`), ensuring resource safety.
* **Improvements:** The most significant improvement was the transition from a procedural script to a modular class hierarchy. I created an abstract `Shape` base class with derived implementations for specific meshes (`MeshCube`, `MeshSphere`, etc.). The scene manager was updated to hold a dynamic vector of these shape objects, allowing the scene to be scalable. If I want to add 100 apples now, I simply instantiate them and add them to the vector, rather than writing 100 blocks of rendering code.

**Course Outcomes Analysis**
With this enhancement, I successfully met the course outcome regarding "Design and evaluate computing solutions that solve a given problem using algorithmic principles and computer science practices."
* **Evaluation:** I evaluated the trade-offs between the original procedural approach (which was faster to write initially but impossible to scale) and the new OOP approach (which required more initial setup but offers long-term maintainability).
* **Outcome Updates:** My original plan focused heavily on just the visual aspect. However, during development, I expanded the scope to include User Interaction (Outcome 4: Innovative Techniques). I implemented an event listener that allows users to toggle the visual state of specific objects using keyboard inputs ('1', '2', '3'), transforming the artifact from a static image into an interactive application.

**Reflection on the Process**
Refactoring this code was a lesson in the complexity of dependency management and the "hidden costs" of software development.
* **Challenges:** The biggest challenge I faced was environmental configuration. Because the original project relied on external libraries linked via relative paths that no longer existed, I encountered significant "Linker Errors" and "File Not Found" exceptions. I had to investigate the directory structure to locate the missing `ShapeMeshes` and `ShaderManager` dependency files and manually relocate them to the source directory where the solution file was expecting them.
* **Debugging:** I also encountered a critical runtime error (Access Violation code `-1073741819`) caused by an uninitialized pointer in my new `SceneManager` constructor. This reinforced the importance of Defensive Programming, ensuring all objects are properly instantiated before usage.
* **Key Takeaway:** Through this process, I learned that clean code is not just about readability; it is about safety. By encapsulating the drawing logic inside the `Shape` classes, I prevented the main loop from accidentally corrupting the state of an individual object, significantly increasing the robustness of the application.

---
### 2. Algorithms and Data Structures: Course Planner (BST)
**View Source Code:** [Insert Link to this specific GitHub Repository]

![Screenshot of Terminal Output](link_to_your_image.jpg) *(Note: Take a screenshot of the console printing the sorted courses)*

### Algorithms and Data Structures Narrative

**Artifact Description**
The artifact selected for the Algorithms and Data Structures category is the "ABCU Advising Assistance Program," a console-based application originally developed in CS 260: Data Structures and Algorithms. Written in C++, the program is designed to load university course data from a CSV file and allow users to either print a sorted alphanumeric list of courses or search for specific course details and prerequisites.

**Justification for Inclusion**
I selected this artifact because it demonstrates the critical difference between using a library and understanding the underlying logic of data organization. In the original iteration, the application relied heavily on standard libraries (`std::vector` and `std::sort`) to organize data. While functional, this approach masked the computational cost of sorting.
* **Skills Showcased:** By refactoring this artifact, I demonstrated the ability to implement complex data structures manually. Specifically, I replaced the linear containers with a custom Binary Search Tree (BST). This required advanced C++ skills, including direct memory management, pointer manipulation, and recursive algorithm design.
* **Improvements:** The transition to a BST significantly improved the theoretical efficiency of the application. The original program required an $O(N \log N)$ sorting operation every time the user requested a course list. The enhanced BST version sorts data naturally upon insertion; this means the data is always sorted, allowing the "Print List" feature to run in linear $O(N)$ time via an in-order traversal.



**Course Outcomes Analysis**
With this enhancement, I have fully met the course outcome to design and evaluate computing solutions that solve a given problem using algorithmic principles and computer science practices and standards appropriate to its solution, while managing the trade-offs involved in design choices.
* **Evaluation:** I successfully evaluated the trade-off between implementation time and runtime efficiency. While the `std::sort` method was faster to write, the BST implementation is more efficient for large datasets where the list is accessed frequently.
* **Outcome Updates:** My plan for this outcome remained consistent throughout the development process. The successful implementation of the BST confirms that I can apply algorithmic principles to optimize software performance, fulfilling the core requirements of this module.

**Reflection on the Process**
Enhancing this artifact highlighted the precision required when working with memory-managed languages like C++.
* **Challenges:** The primary challenge I faced was managing the pointers within the `Node` structure. Unlike the standard vector which handles memory automatically, building a BST required me to manually allocate and link nodes. Debugging the recursive logic for the `Insert` and `InOrderTraversal` functions was difficult; specifically, ensuring that the base cases were correct to prevent infinite recursion or null pointer exceptions.
* **Learning:** This process reinforced my understanding of "Big O" notation in a practical setting. Seeing the list print instantly without a sort function call validated the theoretical efficiency of the tree structure. It also emphasized the importance of encapsulation, by hiding the complex tree logic behind a clean public API (`tree->Insert()`), I kept the `main()` function clean and readable, adhering to good software engineering practices.

---

### 3. Databases: Secure Animal Shelter Dashboard
**View Source Code:** [Insert Link to this specific GitHub Repository]

![Screenshot of Database Schema or Dashboard](link_to_your_image.jpg) *(Note: A screenshot of the dashboard running or your SQLite table structure)*

### Database Design and Security Narrative

**Artifact Description**
The artifact selected for the Database category is the "Grazioso Salvare Dashboard" backend, originally developed in CS 340: Client/Server Development. This artifact is a Python-based `CRUD` (Create, Read, Update, Delete) module designed to interface with a database of animal shelter records. Originally, the application was built using `MongoDB` (a NoSQL document store) and relied on the `pymongo` driver to manage flat, JSON-like records for a web-based dashboard.

**Justification for Inclusion**
I selected this artifact because it provided the clearest opportunity to demonstrate Security Mindset and Relational Database Design. In its original state, the application contained significant security vulnerabilities, specifically hardcoded credentials, and utilized a flat data structure that resulted in data redundancy.
* **Skills Showcased:** By refactoring this artifact, I demonstrated the ability to migrate a backend system from a `NoSQL` architecture to a Relational (`SQL`) architecture using `SQLite`. This required designing a normalized schema (`3NF`) that separates data into logical tables (`Animals`, `Breeds`, `Shelters`) rather than storing everything in a single document. 



* **Improvements:** The most critical improvement was Security. I removed the hardcoded username and password strings that were embedded in the original source code, replacing them with a local, file-based `SQLite` connection that does not require exposed credentials in the script. Additionally, implementing a normalized schema improved data integrity; for example, breed names are now stored once in a lookup table rather than being repeated thousands of times across individual animal records.

**Course Outcomes Analysis**
With this enhancement, I have successfully met the course outcome to develop a security mindset that anticipates adversarial exploits in software architecture and designs to expose potential vulnerabilities, mitigate design flaws, and ensure privacy and enhanced security of data and resources.
* **Evaluation:** By identifying the hardcoded credentials as a critical vulnerability and re-architecting the application to eliminate them, I directly addressed the security outcome.
* **Outcome Updates:** Additionally, I met the outcome regarding "Innovative Techniques" in database management. Migrating from a schematic-less `MongoDB` setup to a strictly typed `SQL` schema required me to define constraints and foreign keys, ensuring that invalid data (such as an animal belonging to a non-existent shelter) cannot be entered into the system.

**Reflection on the Process**
The process of enhancing this artifact emphasized the trade-offs between flexibility (`NoSQL`) and structure (`SQL`).
* **Challenges:** A major challenge I faced during this enhancement was the lack of the original dataset. Since I no longer had access to the original CSV source file, I had to write a custom Python script to generate synthetic mock data. This required me to reverse-engineer what the data should look like based on the dashboard's requirements and programmatically insert valid relationships between the new tables.
* **Learning:** This experience reinforced the importance of normalization. In the original `MongoDB` version, updating a breed name would have required updating thousands of documents. In my enhanced `SQLite` version, I only need to update a single row in the `Breeds` table. This efficiency, combined with the removal of hardcoded secrets, highlighted how architectural choices made early in development dictate the long-term maintainability and security of a product.
---
*Created for CS 499: Computer Science Capstone*
