# NeevaMind - Early Alzheimer's Detection Web App

NeevaMind is an AI-powered web application that helps detect early signs of Alzheimer's and cognitive decline through analysis of daily diary entries. Built with React.js, Node.js, and MySQL.

## Features

- **Secure Authentication**: JWT-based login/signup with bcrypt-encrypted passwords
- **Daily Diary Entries**: Write and store encrypted diary entries
- **AI-Powered Insights**: Cohere API integration for cognitive analysis
- **Visual Reports**: Weekly progress tracking with Chart.js visualizations
- **Privacy First**: All data encrypted and never shared
- **Responsive Design**: Works on desktop, tablet, and mobile

## Tech Stack

- **Frontend**: React.js, Vite, Chart.js
- **Backend**: Node.js, Express.js
- **Database**: MySQL (XAMPP)
- **AI**: Cohere API
- **Authentication**: JWT, bcrypt

## Setup Instructions

### 1. Database Setup

1. Install XAMPP and start MySQL
2. Create the database:
   ```sql
   mysql -u root -p < database/schema.sql
   ```

### 2. Backend Setup

```bash
cd backend
npm install
npm run dev
```

### 3. Frontend Setup

```bash
cd frontend
npm install
npm run dev
```

### 4. Environment Variables

Update `.env` file with your configuration:
- Database credentials
- Cohere API key
- JWT secret

## API Endpoints

- `POST /api/auth/register` - User registration
- `POST /api/auth/login` - User login
- `POST /api/diary/create` - Create diary entry
- `GET /api/diary/entries` - Get user's diary entries
- `POST /api/insights/generate` - Generate AI insights
- `GET /api/insights/today` - Get today's insights
- `GET /api/insights/weekly` - Get weekly report

## Usage

1. Register a new account or login
2. Write daily diary entries
3. View AI-generated insights
4. Track progress with weekly reports

## Privacy & Security

- All passwords are encrypted with bcrypt
- JWT tokens for secure authentication
- Diary entries and insights are encrypted
- No data sharing with third parties

## Development

- Frontend runs on `http://localhost:3000`
- Backend runs on `http://localhost:5000`
- MySQL runs on `http://localhost:3306`
