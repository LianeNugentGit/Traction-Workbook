# Traction Workbook - Vision Component Beta

This repository contains the beta version of the Traction workbook application, focusing on the Vision component of the Entrepreneurial Operating System (EOS) as described in Gino Wickman's book "Traction".

## Features

- **Complete Vision Component Implementation**
  - Core Values exercise
  - Core Focus exercise
  - 10-Year Target exercise
  - Marketing Strategy exercise
  - 3-Year Picture exercise
  - 1-Year Plan exercise
  - Quarterly Rocks exercise

- **AI Coaching Integration**
  - Directive guidance for each exercise
  - Context-aware tips and best practices
  - Interactive Q&A functionality

- **Output Generation**
  - PDF generation for Vision/Traction Organizer™ (V/TO™)
  - Interactive dashboards
  - Progress tracking

## Technology Stack

- **Frontend**: React with TypeScript
- **UI Framework**: Material-UI (MUI)
- **Database & Authentication**: Supabase
- **PDF Generation**: jsPDF
- **Deployment**: Vercel

## Deployment Instructions

### Prerequisites

1. A Supabase account and project
2. A GitHub account
3. A Vercel account

### Step 1: Clone and Configure

1. Clone this repository to your local machine
2. Create a `.env.local` file in the root directory with the following variables:
   ```
   NEXT_PUBLIC_SUPABASE_URL=https://your-supabase-project.supabase.co
   NEXT_PUBLIC_SUPABASE_ANON_KEY=your-supabase-anon-key
   ```
3. Replace the placeholder values with your actual Supabase project URL and anonymous key

### Step 2: Push to GitHub

1. Create a new GitHub repository
2. Initialize Git in the project directory:
   ```
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/yourusername/your-repo-name.git
   git push -u origin main
   ```

### Step 3: Deploy to Vercel

1. Log in to your Vercel account
2. Click "New Project"
3. Import your GitHub repository
4. Configure the project:
   - Framework Preset: Next.js
   - Root Directory: ./
   - Environment Variables:
     - NEXT_PUBLIC_SUPABASE_URL: Your Supabase project URL
     - NEXT_PUBLIC_SUPABASE_ANON_KEY: Your Supabase anonymous key
5. Click "Deploy"

## Supabase Setup

The application requires the following tables in your Supabase project:

- users
- companies
- core_values
- core_focus
- ten_year_target
- marketing_strategy
- three_year_picture
- one_year_plan
- quarterly_plan
- company_rocks
- individual_rocks
- team_members

The SQL schema for these tables is provided in the `supabase/schema.sql` file.

## Usage Instructions

1. Register a new account or log in
2. Create a company profile
3. Navigate to the Vision component
4. Complete each exercise in sequence:
   - Core Values
   - Core Focus
   - 10-Year Target
   - Marketing Strategy
   - 3-Year Picture
   - 1-Year Plan
   - Quarterly Rocks
5. Use the AI coaching feature for guidance
6. Generate PDF outputs or view interactive dashboards

## Feedback Collection

This beta version is designed to collect market feedback on the Vision component before expanding to other EOS components. Consider implementing:

1. A feedback form within the application
2. User testing sessions
3. Analytics to track feature usage and completion rates

## Next Steps

After validating the Vision component, future development could include:

1. People Component
2. Data Component
3. Issues Component
4. Process Component
5. Traction Component
6. Additional EOS tools

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- Based on the Entrepreneurial Operating System® by Gino Wickman
- EOS®, Entrepreneurial Operating System®, and Traction® are registered trademarks of EOS Worldwide
