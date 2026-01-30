# PROBLEM - Setup Guide

## Prerequisites
- Modern web browser (Chrome, Firefox, Safari, or Edge)
- Google API Key (for Google services)
- MongoDB Atlas account and connection string
- (Optional) Local web server for development (e.g., Python's http.server or Node.js http-server)

## Installation Steps

1. Clone the repository
```bash
git clone https://github.com/Bsoumyaranjan32/PROBLEM.git
cd PROBLEM
```

2. Configure environment variables
- Copy `.env.example` to `.env`
```bash
cp .env.example .env
```
- Edit `.env` and add your actual credentials:
  - `GOOGLE_API_KEY`: Your Google API key from Google Cloud Console
  - `MONGO_URI`: Your MongoDB connection string from MongoDB Atlas

3. Run the application
```bash
# Navigate to the Minions-master directory
cd Minions-master

# Option 1: Open directly in browser
# Simply open index.html in your web browser

# Option 2: Run with a local web server (recommended for testing)
# Using Python 3:
python3 -m http.server 8000
# Then open http://localhost:8000 in your browser

# Using Python 2:
python -m SimpleHTTPServer 8000

# Using Node.js (if you have http-server installed):
npx http-server -p 8000
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
