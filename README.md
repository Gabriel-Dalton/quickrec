# QuickRec - Recommendation Letter Platform

QuickRec is a web-based platform that allows employees to generate a recommendation letter draft on their behalf, which can be sent to their supervisor/CEO for review and approval. This saves both parties time by automating the creation process while still giving the supervisor the opportunity to make adjustments and sign off on the final letter.

## 🚀 Features
- **Employee Input:** Employees can input their details, job role, key achievements, and their supervisor's details.
- **Automatic Letter Generation:** Generates a recommendation letter from the perspective of the supervisor.
- **Email Integration:** Sends the letter to the supervisor for approval using EmailJS.
- **Tailwind CSS:** Fully styled with Tailwind CSS for a responsive and modern UI.

## 🛠️ Technologies Used
- **HTML** for structure
- **Tailwind CSS** for styling
- **JavaScript** for logic
- **EmailJS** for email sending integration

## 📋 Prerequisites
Before you begin, ensure you have met the following requirements:
- A web browser (Google Chrome, Firefox, etc.)
- An EmailJS account. [Sign up for EmailJS](https://www.emailjs.com/)
- Basic knowledge of HTML, JavaScript, and Tailwind CSS

## 📦 Setup & Installation
1. **Clone the repository:**
   ```bash
   git clone https://github.com/Gabriel-Dalton/quickrec.git
   ```
2. **Navigate to the project folder:**
   ```bash
   cd quickrec
   ```
3. **Open the project:**
   Open the `index.html` file in your web browser.

## 🔧 Configuration
1. **Set up EmailJS:**
   - Sign up or log in to [EmailJS](https://www.emailjs.com/).
   - Create a new email service and template.
   - Add your `service_id`, `template_id`, and `user_id` to the script in `index.html`.

   ```javascript
   emailjs.init("YOUR_USER_ID"); // Replace with your EmailJS User ID
   ```

2. **Modify the JavaScript:**
   - Ensure your `service_id` and `template_id` in the `script.js` file match the values in your EmailJS account.

## 📄 Usage
1. Open the `index.html` file in your browser.
2. Fill out the form with your details, job role, achievements, and supervisor's information.
3. Click "Generate & Send for Approval" to send the recommendation letter to your supervisor for review.

## 🎨 Customization
You can modify the HTML, CSS, and JavaScript files to change:
- The template and design (Tailwind CSS is used for styling).
- The email structure and content.

## 🤖 Example Email Template
When setting up your template in EmailJS, use the following example:

```html
<p>Hello {{to_name}},</p>

<p>You have received a recommendation letter request from {{employee_name}} for their role as a {{job_role}}:</p>

<p style="padding: 12px; border-left: 4px solid #d0d0d0; font-style: italic; white-space: pre-wrap;">
  {{letter_content}}
</p>

<p>Please review the letter and let us know if you approve.</p>

<p>Best regards,<br>QuickRec Team</p>

```

## 🔗 Links
- [Tailwind CSS Documentation](https://tailwindcss.com/docs)
- [EmailJS Documentation](https://www.emailjs.com/docs/)

## 🤝 Contributing
Contributions are welcome! Feel free to open an issue or submit a pull request with improvements or bug fixes.

## ⚖️ License
This project is licensed under the MIT License .
