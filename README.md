# Bank Sampah - Mata Kuliah Pemrograman Web 2

Bank Sampah is a Laravel web application developed as part of the course "Mata Kuliah Pemrograman Web 2." It provides features related to waste management and recycling. This document outlines the necessary steps to install and run the application locally.

## Requirements

- PHP >= 7.3
- Composer
- Node.js & npm
- MySQL or a compatible database system

## Installation Steps

Follow these steps to install and run the Bank Sampah project on your local machine.

### 1. Clone the Repository

Clone the repository to your local machine using Git.

\`\`\`bash
git clone https://github.com/yourusername/bank-sampah.git
cd bank-sampah
\`\`\`

### 2. Install Composer

If you haven't already installed Composer, you can download and install it using the instructions on the [official website](https://getcomposer.org/download/).

### 3. Install Project Dependencies

Run the following command to install the PHP dependencies:

\`\`\`bash
composer install
\`\`\`

### 4. Install Node.js Dependencies and Compile Assets

First, install the Node.js dependencies:

\`\`\`bash
npm install
\`\`\`

Then, compile the assets:

\`\`\`bash
npm run dev
\`\`\`

### 5. Set Up Environment Variables

Copy the example environment file and make any necessary adjustments to your local environment:

\`\`\`bash
cp .env.example .env
\`\`\`

### 6. Generate Application Key

Generate a unique application key:

\`\`\`bash
php artisan key:generate
\`\`\`

### 7. Configure Database

Ensure that your database connection settings are correctly configured in the \`.env\` file. Then, run the migrations to create the necessary tables:

\`\`\`bash
php artisan migrate
\`\`\`

### 8. Serve the Application

Finally, serve the application locally:

\`\`\`bash
php artisan serve
\`\`\`

The application should now be accessible at \`http://127.0.0.1:8000\`.
