# PROBLEM - Setup Guide

## Prerequisites
- Node.js installed
- Google API Key (for Google services)
- MongoDB Atlas account and connection string

## Installation Steps

1. Clone the repository
```bash
git clone https://github.com/Bsoumyaranjan32/PROBLEM.git
cd PROBLEM
```

2. Install dependencies (if using Node.js)
```bash
npm install
```

3. Configure environment variables
- Copy `.env.example` to `.env`
```bash
cp .env.example .env
```
- Edit `.env` and add your actual credentials:
  - `GOOGLE_API_KEY`: Your Google API key from Google Cloud Console
  - `MONGO_URI`: Your MongoDB connection string from MongoDB Atlas

4. Run the application
```bash
# Navigate to the Minions-master directory
cd Minions-master

# Open index.html in your browser or run with a local server
# If using Node.js with a server:
node app.js
```

## Security Notes
⚠️ **IMPORTANT**: Never commit your `.env` file to the repository. It contains sensitive credentials.

- The `.env` file is ignored by git (listed in `.gitignore`)
- Use `.env.example` as a template
- Regenerate your API keys if they have been exposed

## Configuration

### Google API Key
Get your API key from [Google Cloud Console](https://console.cloud.google.com/)

### MongoDB URI
Get your connection string from [MongoDB Atlas](https://www.mongodb.com/cloud/atlas)

## Troubleshooting
- Ensure your `.env` file exists and contains valid credentials
- Check that your MongoDB connection string is correct
- Verify your Google API key has the necessary permissions
