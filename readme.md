# ContactManager Pro

A full-stack web application to manage your contacts, offering features like authentication, image uploads, dark mode, and more.

## Table of Contents
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Installation](#installation)
- [Usage](#usage)
- [Environment Variables](#environment-variables)
- [Contributing](#contributing)
- [License](#license)

## Features
- **Authentication:** Register and login with email and password.
- **Contact Management:** Add, update, delete contacts, and manage their display pictures.
- **Profile Links:** Manage profile links for each contact.
- **Image Upload:** Upload and update display pictures for contacts using Cloudinary.
- **Search Functionality:** Search contacts by name or profile links.
- **Toast Notifications:** Receive notifications using Sonner for actions like adding, updating, or deleting contacts.
- **Dark Mode:** Toggle between dark and light modes with local storage saving the preference.
- **Responsive Design:** Fully responsive UI for all screen sizes.

## Tech Stack
### Front-end
- **ReactJS:** Frontend framework for building user interfaces.
- **useState Hook & Props:** For state management and passing data between components.
- **React Router:** For routing and navigation within the application.
- **Semantic-UI with Custom CSS:** UI library for styling with additional customizations.
- **Sonner:** For toast notifications, replacing React Toast Notifications.
- **Vite:** Build tool for faster development and optimized builds.

### Back-end
- **Node.js:** JavaScript runtime environment.
- **Express.js:** Web framework for Node.js to build APIs.
- **MongoDB:** NoSQL database for storing document-based data.
- **Mongoose:** MongoDB object modeling for Node.js.
- **Cloudinary:** Service for image uploading and management.
- **JSON Web Token (JWT):** For securing and authenticating HTTP requests.
- **Bcrypt.js:** For hashing passwords securely.
- **Validator.js:** For validating JSON data.
- **Mongoose Unique Validator:** Plugin for error handling of unique fields in Mongoose schemas.
- **Dotenv:** For loading environment variables from a `.env` file.

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/contactmanager-pro.git
   cd contactmanager-pro
   ```

2. Install dependencies for the server and client:
   ```bash
   # Install server dependencies
   cd server
   npm install
   
   # Install client dependencies
   cd ../client
   npm install
   ```

3. Create a `.env` file in the `server` directory with the following variables:

   ```plaintext
   MONGO_URI=your_mongodb_connection_string
   JWT_SECRET=your_jwt_secret
   CLOUDINARY_CLOUD_NAME=your_cloudinary_cloud_name
   CLOUDINARY_API_KEY=your_cloudinary_api_key
   CLOUDINARY_API_SECRET=your_cloudinary_api_secret
   ```

4. Create a `.env` file in the `client` directory with the following variable:

   ```plaintext
   VITE_BACKEND_URL=http://localhost:5000
   ```

5. Start the development server:
   ```bash
   # Start the server
   cd server
   npm run dev

   # Start the client
   cd ../client
   npm run dev
   ```

## Usage
1. Register and log in with your email and password.
2. Add new contacts with display pictures and profile links.
3. Search for contacts by name or profile links.
4. Toggle between dark and light mode as per your preference.
5. Manage your contacts, including updating or deleting them.

## Environment Variables
Ensure you have the following environment variables set up:

### Server (`server/.env`)

```plaintext
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
CLOUDINARY_CLOUD_NAME=your_cloudinary_cloud_name
CLOUDINARY_API_KEY=your_cloudinary_api_key
CLOUDINARY_API_SECRET=your_cloudinary_api_secret
```

### Client (`client/.env`)

```plaintext
VITE_BACKEND_URL=http://localhost:5000
```

## Contributing
Feel free to contribute to this project by submitting a pull request. Please ensure your code follows the project's coding guidelines.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more information.

