# Sms Sending Website

The **Send SmS** website is a simple web application that allows users to send SMS messages containing their current geographic location. This functionality is powered by the Twilio API, and the website is designed with a minimalistic user interface for ease of use.

# Features
- **Send Location via SMS**: Users can click a button to send their current GPS coordinates via SMS.
- **Twilio Integration**: The app uses Twilio's REST API to send SMS messages.
- **Responsive Design**: The website is designed to be responsive and user-friendly on various screen sizes.

# Prerequisites
- Node.js and npm (for running the local server)
- A Twilio account with an active phone number
- Basic knowledge of HTML, CSS, and JavaScript

# Setup and Installation

### 1.  Clone the Repository
```bash
git clone https://github.com/yourusername/sendsms.git
cd sendsms
```

### 2. Install Dependencies
Make sure you have Node.js and npm installed. Run the following command to install the necessary dependencies:
```bash
npm install
```

### 3. Configure Twilio Credentials
In the `scriptSmS.js` file, replace the following placeholders with your Twilio credentials and phone numbers:
```javascript
const accountSid = 'your_twilio_account_sid';
const authToken = 'your_twilio_auth_token';
const fromNumber = 'your_twilio_phone_number';
const toNumber = 'recipient_phone_number';
```
Replace `your_twilio_account_sid`, `your_twilio_auth_token`, `your_twilio_phone_number`, and `recipient_phone_number` with the actual values from your Twilio account.

### 4. Run the Server
To start the local server, run:
```bash
npm start
```
This will start the server on `http://localhost:3000`.

### 5. Access the Website
Open your web browser and navigate to `http://localhost:3000` to access the Send SmS website.

## File Structure

- **indexSmS.html**: The main HTML file that contains the structure of the web page.
- **stylesSmS.css**: Contains the styles and layout of the web page.
- **scriptSmS.js**: JavaScript file handling the SMS sending functionality and integration with the Twilio API.
- **server.js**: Node.js server file that serves the website.
