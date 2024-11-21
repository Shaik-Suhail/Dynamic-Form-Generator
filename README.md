# Dynamic-Form-Generator

Here’s an updated `README.md` for your project:

---

# Dynamic Form Generator

This project allows users to create dynamic forms by providing a JSON schema. It generates a responsive form in real-time, including validation, error handling, and a JSON editor for schema modification.

## Features
- Real-time form generation from JSON schema.
- JSON editor with syntax highlighting and validation.
- Dynamic support for text, email, select, radio, and textarea fields.
- Real-time form validation and error handling.
- Mobile-responsive layout with adaptive form preview.
- Form submission logs data in the console.
- Unit tests (Jest) and E2E tests (Playwright) for functionality.

## Setup Instructions

### 1. Clone the repository:
```bash
git clone https://github.com/your-username/dynamic-form-generator.git
cd dynamic-form-generator
```

### 2. Install dependencies:
```bash
npm install
```

### 3. Start the development server:
```bash
npm start
```
Access the app at `http://localhost:3000`.

## Example JSON Schemas

### Example 1: Basic Form
```json
{
  "formTitle": "Contact Us",
  "formDescription": "Please fill out the form below to get in touch.",
  "fields": [
    { "id": "name", "type": "text", "label": "Full Name", "required": true, "placeholder": "Enter your name" },
    { "id": "email", "type": "email", "label": "Email", "required": true, "placeholder": "you@example.com" },
    { "id": "message", "type": "textarea", "label": "Message", "required": false, "placeholder": "Enter your message" }
  ]
}
```

### Example 2: Survey Form
```json
{
  "formTitle": "Project Requirements Survey",
  "formDescription": "Please provide details about your project.",
  "fields": [
    { "id": "company", "type": "text", "label": "Company Name", "required": true, "placeholder": "Enter company name" },
    { "id": "industry", "type": "select", "label": "Industry", "required": true, "options": [{ "value": "tech", "label": "Technology" }, { "value": "healthcare", "label": "Healthcare" }, { "value": "finance", "label": "Finance" }] },
    { "id": "comments", "type": "textarea", "label": "Additional Comments", "required": false, "placeholder": "Any additional details..." }
  ]
}
```

### Example 3: Feedback Form
```json
{
  "formTitle": "Feedback Form",
  "formDescription": "We appreciate your feedback.",
  "fields": [
    { "id": "rating", "type": "radio", "label": "How would you rate your experience?", "required": true, "options": [{ "value": "1", "label": "1 - Poor" }, { "value": "5", "label": "5 - Excellent" }] },
    { "id": "comments", "type": "textarea", "label": "Your Comments", "required": false, "placeholder": "Enter your comments" }
  ]
}
```

## Testing

### Running Tests
- **Unit Tests**: 
  ```bash
  npm test
  ```
- **End-to-End Tests (Playwright)**:
  ```bash
  npx playwright test
  ```

## Deployment

### Deploy Locally:
1. Build the application:
   ```bash
   npm run build
   ```

2. Serve the build:
   ```bash
   npm install -g serve
   serve -s build
   ```

3. Access the app at `http://localhost:5000`.

### Deployed Application
Access the live version at: [Vercel Deployment](https://dynamic-form-generator.vercel.app)

## License
MIT License

---

This template gives a detailed overview of the project, setup, example schemas, testing instructions, and deployment steps. You can update the repository URL and any other details specific to your project.
