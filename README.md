# Learning Management System (LMS)

Welcome to SciNet Learning, a powerful Learning Management System designed to enhance the educational experience for both users and administrators. Developed by Martin Lubowa (martinlubowa@outlook.com), SciNet Learning is built using Node.js, TypeScript, Redis, MongoDB, and Next.js.

Live Demo: [https://africanscienceresearchacademy.netlify.app/](https://africanscienceresearchacademy.netlify.app/)

## Table of Contents

- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
- [Features](#features)
  - [User Features](#user-features)
  - [Admin Features](#admin-features)
- [Usage](#usage)
  - [User Roles](#user-roles)
  - [Creating an Account](#creating-an-account)
  - [Enrolling in Courses](#enrolling-in-courses)
  - [Taking Quizzes](#taking-quizzes)
  - [Providing Course Reviews](#providing-course-reviews)
  - [Watching Lessons](#watching-lessons)
  - [Making Payments](#making-payments)
  - [Admin Dashboard](#admin-dashboard)
- [Contributing](#contributing)
- [License](#license)

## Screenshots
![image]("images/e1.png")
![image]("images/e_2.png")
![image]("images/e_3.png")
![image]("images/e5.png")
![image]("images/e6.png")
![image]("images/e7.png")

## Getting Started


### Prerequisites

Before you begin, ensure you have the following installed:

- [Node.js](https://nodejs.org/) - v14.x or later
- [MongoDB](https://www.mongodb.com/) - A NoSQL database
- [Redis](https://redis.io/) - An in-memory data structure store
- [Next.js](https://nextjs.org/) - A React framework for building server-rendered applications

### Installation

1. **Clone the repository:**

   ```bash
   git clone https://github.com/your-username/lms.git
   cd lms
   ```

2. **Install dependencies:**

   ```bash
   # Install backend dependencies
   cd backend
   npm install

   # Install frontend dependencies
   cd ../frontend
   npm install
   ```

3. **Configure environment variables:**

   - Create a `.env` file in the `backend` directory with the necessary configuration variables. Sample:

     ```env
     PORT=3000
     MONGODB_URI=mongodb://localhost:27017/lms
     REDIS_URL=redis://localhost:6379
     ```

     Update the variables based on your environment.

   - Create a `.env.local` file in the `frontend` directory with the necessary configuration variables for the frontend. Sample:

     ```env
     NEXT_PUBLIC_API_URL=http://localhost:3000/api
     ```

     Update the variable based on your backend API URL.

4. **Run the application:**

   ```bash
   # Run the backend server
   cd backend
   npm run dev

   # Run the frontend development server
   cd ../frontend
   npm run dev
   ```

   The LMS should now be accessible at [http://localhost:3000](http://localhost:3000).

## Features

### User Features

1. **Sign In and Sign Out:**
   - Users can create accounts, sign in, and sign out securely.

2. **Enrollment in Courses:**
   - Users can browse available courses and enroll in their preferred courses.

3. **Quizzes:**
   - Users can take quizzes associated with each course to assess their understanding.

4. **Course Reviews:**
   - Users can provide reviews and feedback on courses they have completed.

5. **Lesson Videos:**
   - Users can watch video lessons associated with each course.

6. **Payment Processing:**
   - Users can make secure payments for paid courses.

### Admin Features

1. **Team Role Management:**
   - Admins can manage team roles and permissions.

2. **Create Courses:**
   - Admins can create new courses, including adding lessons, quizzes, and setting pricing.

3. **Analytics Dashboard:**
   - Admins have access to an analytics dashboard to track user engagement and course popularity.

4. **Invoice Management:**
   - Admins can manage and track invoices for paid courses.

5. **Course Categories:**
   - Admins can create and manage course categories for better organization.

6. **User Activity Tracking:**
   - Admins can view and track user activity within the system.

## Usage

### User Roles

- **Student:**
  - Enrolls in courses
  - Takes quizzes
  - Provides course reviews
  - Watches lessons

- **Instructor:**
  - Creates and manages courses
  - Adds lessons, quizzes, and content

- **Admin:**
  - Manages team roles and permissions
  - Accesses analytics dashboard
  - Manages invoices and user activity
  - Creates course categories

### Creating an Account

1. Navigate to the [Sign-Up](http://localhost:3000/signup) page.

2. Fill in the required information to create a new account.

### Enrolling in Courses

1. Browse the available courses on the [Courses](http://localhost:3000/courses) page.

2. Click on a course to view details.

3. Enroll in the course if interested.

### Taking Quizzes

1. Access the enrolled course from the [My Courses](http://localhost:3000/my-courses) page.

2. Navigate to the quizzes section.

3. Take the quizzes associated with the course.

### Providing Course Reviews

1. Access the completed course from the [My Courses](http://localhost:3000/my-courses) page.

2. Provide a review and feedback on the course.

### Watching Lessons

1. Access the enrolled course from the [My Courses](http://localhost:3000/my-courses) page.

2. Navigate to the lessons section.

3. Watch the video lessons associated with the course.

### Making Payments

1. Access the desired paid course from the [Courses](http://

localhost:3000/courses) page.

2. Proceed to payment and complete the transaction securely.

### Admin Dashboard

1. Access the admin dashboard from [Admin Dashboard](http://localhost:3000/admin/dashboard).

2. Explore team role management, analytics, invoice management, and user activity tracking.

## Contributing

If you'd like to contribute to the project, please follow the [Contribution Guidelines](CONTRIBUTING.md).

## License

This project is licensed under the [MIT License](LICENSE).