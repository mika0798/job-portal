<h1>Job Application Management System</h1>
<p>
A web-based job application platform built with <strong>Spring Boot MVC</strong> and <strong>Thymeleaf</strong>, 
allowing recruiters to post jobs and manage candidates, while job seekers can search, apply for jobs, 
and manage their profiles.
</p>

<h2>Table of Contents</h2>
<ul>
  <li><a href="#introduction">Introduction</a></li>
  <li><a href="#features">Features</a></li>
  <li><a href="#gallery">Gallery</a></li>
  <li><a href="#technology-stack">Technology Stack</a></li>
  <li><a href="#project-structure">Project Structure</a></li>
  <li><a href="#database-erd">Database ERD</a></li>
  <li><a href="#entity-diagram">Entity Diagram</a></li>
</ul>

<h2 id="introduction">1. Introduction</h2>
<p>
This project is a <strong>Job Application Management System</strong> developed using 
<strong>Spring Boot MVC</strong> and <strong>Thymeleaf</strong>.  
The system supports two main roles: <strong>Recruiter</strong> and <strong>Candidate</strong>.
Recruiters can post jobs and manage applicants, while candidates can search and apply for jobs, 
upload résumés, and track application status.
</p>

<h2 id="features">2. Features</h2>
<ul>
  <li><strong>User Authentication</strong>: Register, Login, Logout with role-based access (Recruiter / Candidate)</li>
  <li><strong>Recruiter Features</strong>:
    <ul>
      <li>Post new job listings</li>
      <li>View and manage posted jobs</li>
      <li>View list of candidates who applied for each job</li>
      <li>Edit recruiter profile and upload profile photo</li>
    </ul>
  </li>
  <li><strong>Candidate Features</strong>:
    <ul>
      <li>Search for jobs by keyword and location</li>
      <li>Apply for jobs</li>
      <li>View list of applied jobs</li>
      <li>Edit candidate profile and upload profile photo</li>
      <li>Upload résumé / CV</li>
    </ul>
  </li>
  <li><strong>Job & Location Management</strong></li>
  <li><strong>Server-side Rendering</strong> using Thymeleaf</li>
</ul>

<h2 id="gallery">3. Gallery</h2>
<div align="center">
<img src="images/home.png" width="100%" alt="Home Page">
<details>
    <summary><h3>More images</h3></summary>
    <div align="center">
        <img src="images/recruiter-dashboard.png" width="90%" alt="Recruiter Dashboard">
        <img src="images/candidate-dashboard.png" width="90%" alt="Candidate Dashboard">
    </div>
</details>
</div>

<h2 id="technology-stack">4. Technology Stack</h2>

<h3>Backend</h3>
<ul>
  <li><strong>Framework</strong>: Spring Boot</li>
  <li><strong>Java Version</strong>: Java 21</li>
  <li><strong>Build Tool</strong>: Maven</li>
  <li><strong>Database</strong>:
    <ul>
      <li>MySQL (Production)</li>
      <li>H2 Database (Development / Testing)</li>
    </ul>
  </li>
  <li><strong>Dependencies</strong>:
    <ul>
      <li>Spring Web MVC</li>
      <li>Thymeleaf</li>
      <li>Spring Data JPA (Hibernate)</li>
      <li>Spring Security</li>
      <li>Lombok</li>
      <li>Spring Validation</li>
      <li>Spring Boot Actuator</li>
    </ul>
  </li>
</ul>

<h3>Frontend</h3>
<ul>
  <li>Thymeleaf</li>
  <li>Web Jars</li>
  <li>Boostrap</li>
  <li>jQuery</li>
  <li>Locator</li>
  <li>Font-awesome</li>
</ul>

<h2 id="project-structure">5. Project Structure</h2>
<pre><code>
src
 └── main
     ├── java
     │   └── com.example.jobportal
     │       ├── controller
     │       │   ├── HomeController.java
     │       │   ├── UsersController.java
     │       │   ├── JobPostActivityController.java
     │       │   ├── JobLocationController.java
     │       │   ├── JobSeekerApplyController.java
     │       │   ├── JobSeekerProfileController.java
     │       │   ├── JobSeekerSaveController.java
     │       │   └── RecruiterProfileController.java
     │       ├── model
     │       ├── repository
     │       ├── service
     │       └── security
     └── resources
         ├── templates
         ├── static
         └── application.yml
</code></pre>

<h2 id="database-erd">6. Database ERD</h2>
<div align="center">
<img src="images/database-erd.png" width="80%" alt="Database ERD">
</div>

<h2 id="entity-diagram">7. Entity Diagram</h2>
<div align="center">
<img src="images/entity-diagram.png" width="80%" alt="POJO ERD">
</div>
