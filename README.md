# Overview

This is a simple React-based project designed to collect project requirements from users. The form dynamically renders fields based on a JSON schema and submits the data, displaying it in the console.



##Setup Instructions
Follow these steps to set up and run the project locally:

Clone the repository:

bash
Copy code
git clone https://github.com/your-username/your-repository.git
cd your-repository
Install dependencies: Ensure you have npm n installed. Run the following command:


npm install
Start the development server:


This will start the development server at http://localhost:3000.








### Deployment

This section has moved here:https://form-dhiraj-s-projects.vercel.app/


###Json Schema

export const inputFormElement = [
  {
    "id": "name",
    "type": "text",
    "label": "Full Name",
    "required": true,
    "placeholder": "Enter your full name"
  },
  {
    "id": "email",
    "type": "email",
    "label": "Email Address",
    "required": true,
    "placeholder": "you@example.com",
    "validation": {
      "pattern": "^[^\\s@]+@[^\\s@]+\\.[^\\s@]+$",
      "message": "Please enter a valid email address"
    }
  },
  {
    "id": "companySize",
    "type": "select",
    "label": "Company Size",
    "required": true,
    "options": [
      { "value": "1-50", "label": "1-50 employees" },
      { "value": "51-200", "label": "51-200 employees" },
      { "value": "201-1000", "label": "201-1000 employees" },
      { "value": "1000+", "label": "1000+ employees" }
    ]
  },
  {
    "id": "industry",
    "type": "select",
    "label": "Industry",
    "required": true,
    "options": [
      { "value": "tech", "label": "Technology" },
      { "value": "healthcare", "label": "Healthcare" },
      { "value": "finance", "label": "Finance" },
      { "value": "retail", "label": "Retail" },
      { "value": "other", "label": "Other" }
    ]
  },
  {
    "id": "timeline",
    "type": "select",
    "label": "Project Timeline",
    "required": true,
    "options": [
      { "value": "immediate", "label": "Immediate (within 1 month)" },
      { "value": "short", "label": "Short-term (1-3 months)" },
      { "value": "medium", "label": "Medium-term (3-6 months)" },
      { "value": "long", "label": "Long-term (6+ months)" }
    ]
  },
  {
    "id": "comments",
    "type": "textarea",
    "label": "Additional Comments",
    "required": false,
    "placeholder": "Any other details you'd like to share..."
  }
];



###Features
Dynamic form generation based on JSON schema.
Support for different input types, including text, email, select dropdowns, and textarea.
Client-side validation for required fields.
Reset functionality to clear all fields.





