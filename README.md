## how to run
npm start 

## Objective
Develop a simple email client application using React. (https://gist.githubusercontent.com/mrchenliang/9a08135afb75cc7c065f76bd921174ce/raw/d2e8156797de5cead73a131b79f3981b6f5b4b68/wireframe.png).

### React App Setup
1. Create a React Application: Set up a new React application using `npx create-react-app <project-name>`
2. Project Structure: Organize your components, services, and assets in a clean and manageable structure.

### Fetching and Displaying Emails
1. Data Fetching:
  * Fetch email data from this URL: `https://gist.githubusercontent.com/mrchenliang/15e1989583fd6e6e04e1c49287934c91/raw/ed03cfea1e2edb0303543d2908cd7429ed75580d/email.json`.
2. Load the data when the app initializes and lands on the homepage `/`

### Email Sidebar View:
1. Create a component to display the list of emails.
2. Show the `from`, `subject`, `address` and `timestamp` for each email.
3. Do not display the email's `message` in the Email Sidebar View.
4. Ensure the background of the emails within the Email Sidebar View are different based on their status (unread, read, active).
  * an email is unread when `read` is `false`
  * an email is read when `read` is `true`
  * an email is active when the message is being displayed in the Email Body View

### Email Body View:
1. It is blank when no email is selected (feel free to incorporate an icon or text as placeholder)
2. Display the email and its full content, including the message.

### Email Interaction:
1. When an email is clicked within the Email Sidebar View, mark it as read and show its full content in the Email Body View.

### State Management
1. React State:
  * Efficiently manage the state for email statuses (unread, read, active).
  * Ensure the UI reflects the current state accurately.
### CSS Styling:
1. Style your components using CSS. Ensure a clean and user-friendly UI.

### EXTA:
1. Implement 2 folders: deleted and inbox.  
  * The deleted folder should display emails with `deleted` being `true`
  * The inbox folder should display emails with `deleted` being `false`
1. Implement a search bar to filter the emails by `subject`
  * when an user types in the search bar, it would filter emails which includes the word in the `subject` of the email

### Reference:
https://gist.github.com/mrchenliang/9a08135afb75cc7c065f76bd921174ce
