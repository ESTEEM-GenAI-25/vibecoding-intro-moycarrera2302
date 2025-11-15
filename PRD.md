# 📑 Product Requirements Document (PRD)

## 1. Project Overview
- **Summary:**  
A professional, single-page personal portfolio website for Moisés Alejandro Carrera Alcacio, an ESTEEM Master's student, with AI ability demonsteation
- **Context/Background:**  
The project was created to serve as a dynamic, modern, and comprehensive online resume. It replaces a traditional static CV with an engaging web experience. The inclusion of the "Personal Connection Engine" serves as a live proof-of-concept, highlighting practical skills in AI and product development
## 2. Goals and Objectives
- **Primary Goal(s):**  
To create a professional and polished online presence to share with recruiters, academic contacts, and potential collaborators.
- **Secondary Goal(s):**  
To create a responsive and accessible user experience for all visitors, regardless of their device.
## 3. Target Audience
- **Who are the users?**  
Recruiters, hiring managers, professional contacts in the tech and business industries, university faculty, and fellow students.
- **User Needs:**  
Learn how to apply actual UX into a UI with a practical case and an expert in the field.
## 4. Key Features / Requirements
- **Must-Have Features:**  
Single-Page Layout: All content is accessible on a single, scrollable page for ease of use.
Sticky Navigation: A header with smooth-scrolling links to all major sections (About, Projects, Interactive Demo, Education).
Dynamic Content Sections: Dedicated sections for a hero banner, personal motivations, projects/experience, and education/certifications.
Interactive AI Project ("Personal Connection Engine"):
An input form for order details (customer name, products, etc.).
A "Generate Message" button that calls the Gemini API.
A display area for the AI-generated text.
Functionality to copy and regenerate the message.
Clear loading and error states to manage user expectations.
Responsive Design: The layout is fully functional and aesthetically pleasing.

- **Nice-to-Have Features (Optional):**  
A photo gallery to add a more personal touch (a placeholder section for this currently exists).
A dedicated "Contact Me" section with links to LinkedIn, GitHub, or an email address.

## 5. Design & User Experience
Visual Style / Vibe:
Clean, professional, and modern, with a minimalist aesthetic that emphasizes readability and content.
Branding / Colors / Fonts:
Color Palette: A primarily neutral scheme (white, black, and shades of gray) with a bold indigo (#6366F1) accent color to draw attention to key elements.
Typography: Uses the 'Inter' sans-serif font for a clean and highly readable text experience.
Accessibility Considerations:
Use of semantic HTML tags (<header>, <section>, <nav>) for better structure.
Smooth scrolling for improved navigation experience.
Form inputs are correctly linked to their labels using htmlFor.

## 6. Content Requirements
Homepage (Hero Section)
About (Personal Motivations)
Projects & Experience
Interactive Project (Personal Connection Engine)
Education & Certifications
Footer
Specific Content to Include:
All professional and academic copy as detailed in the index.html file.
The fully functional React application for the interactive demo.

## 7. Technical Constraints
Frontend: HTML5, CSS3 (Tailwind CSS), and modern JavaScript (ESM).
JavaScript Library: React for the interactive project.
API: Google Gemini API via the @google/genai library.
Dependencies: All dependencies are loaded from a CDN (esm.sh), creating a self-contained, serverless application.
Hosting / Deployment:
The project is a single index.html file, making it perfectly suited for static site hosting platforms like GitHub Pages.
Performance / Security Requirements:
The site must be mobile-responsive.
Security Note: The Gemini API key is currently hardcoded in the frontend script. For a production environment, this key should be moved to a secure backend to prevent public exposure and unauthorized use.

## 8. Out of Scope
A backend server or database. The application is entirely client-side.
User accounts or authentication.
Saving or storing any generated messages.

## 9. Acceptance Criteria
The website loads successfully in all major modern browsers.
All navigation links scroll smoothly to the correct section on the page.
The interactive project successfully generates a message when valid inputs and a correct API key are provided.
The application displays clear loading indicators during API calls and provides user-friendly error messages if the API key is missing or an error occurs.
The entire layout is responsive and usable across mobile, tablet, and desktop screen sizes.
