# Dream Competitive Circle

An advanced, full-stack online examination platform for competitive exam preparation with real-time analytics, performance tracking, and comprehensive exam management.

## Features

### Student Features
- **User Authentication**: Secure email/password authentication with Supabase
- **Personalized Dashboard**: Performance stats, exam history, and progress tracking
- **Exam Taking Interface**:
  - Timer-based MCQ exams with auto-submit
  - Question navigation palette
  - Mark for review functionality
  - Real-time timer
- **Results & Analytics**:
  - Detailed score breakdown
  - Answer key with explanations
  - Performance metrics and accuracy tracking
- **Leaderboard**: Compare performance with other students
- **Dark Mode**: Toggle between light and dark themes
- **Anti-Cheating**: Tab switch detection and fullscreen mode enforcement

### Admin Features
- **Admin Dashboard**: Overview of students, exams, and performance metrics
- **Exam Management**:
  - Create, edit, and delete exams
  - Set duration, marks, negative marking, and passing criteria
  - Activate/deactivate exams
- **Question Management**:
  - Add, edit, and delete MCQ questions
  - Set correct answers and explanations
  - Organize by topics
- **Student Monitoring**: View all student attempts and performance

## Tech Stack

- **Frontend**: React 18 + TypeScript + Vite
- **Styling**: Tailwind CSS with dark mode support
- **Database**: Supabase (PostgreSQL)
- **Authentication**: Supabase Auth
- **Routing**: React Router v6
- **Icons**: Lucide React
- **Animations**: Framer Motion

## Getting Started

### Prerequisites
- Node.js 18+ installed
- Supabase account (database is already configured)

### Installation

1. Install dependencies:
```bash
npm install
```

2. Environment variables are already configured in `.env`

3. Run the development server:
```bash
npm run dev
```

4. Build for production:
```bash
npm run build
```

## Usage

### For Students

1. **Register**: Create an account using email and password
2. **Login**: Access your personalized dashboard
3. **Browse Exams**: View all available exams with filters
4. **Take Exam**:
   - Read instructions carefully
   - Click "Start Exam" to begin
   - Answer questions within the time limit
   - Use the question palette to navigate
   - Mark questions for review
   - Submit when done or wait for auto-submit
5. **View Results**: See detailed results with answer key and explanations
6. **Track Progress**: Monitor your performance on the dashboard
7. **Leaderboard**: Check your rank against other students

### For Admins

1. **Admin Access**: Register and contact existing admin for approval
2. **Create Exams**:
   - Go to Admin Dashboard
   - Click "Create New Exam"
   - Fill in exam details (title, duration, marks, etc.)
   - Add questions to the exam
3. **Manage Questions**:
   - Add MCQ questions with 4 options
   - Set the correct answer
   - Add explanations (optional)
   - Organize by topics
4. **Monitor Students**: View all exam attempts and performance metrics

## Database Schema

The platform uses the following main tables:

- **profiles**: Extended user information with roles
- **exams**: Exam configurations and settings
- **questions**: MCQ questions for each exam
- **exam_attempts**: Student exam attempt records
- **notifications**: User notification system
- **admin_requests**: Admin role approval system

All tables have Row Level Security (RLS) enabled for data protection.

## Security Features

- **Authentication**: JWT-based authentication with Supabase
- **Row Level Security**: Database-level access control
- **Role-Based Access**: Separate student and admin permissions
- **Anti-Cheating**: Tab switch tracking and fullscreen enforcement
- **Input Validation**: Client and server-side validation

## Deployment

The application is ready for deployment on:

- **Vercel** (recommended)
- **Netlify**
- **AWS Amplify**
- Any static hosting service

Simply connect your repository and deploy. Environment variables are already configured.

## API Routes

The application uses Supabase's auto-generated API endpoints for all database operations.

## Contributing

This is a production-ready examination platform. Feel free to extend it with additional features like:

- AI-based question suggestions
- Certificate generation
- Payment gateway integration
- Mobile app version
- Video proctoring
- Discussion forums

## License

MIT License

## Support

For issues or questions, please contact the development team.

---

Built with modern web technologies for optimal performance and user experience.
