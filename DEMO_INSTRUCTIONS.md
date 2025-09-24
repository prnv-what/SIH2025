# CivicReport Demo Mode Instructions

This application is now running in **DEMO MODE** with all backend functionality replaced by demo data. No actual database or backend services are required.

## Demo Login Credentials

### Citizen Account
- **Email:** `citizen@demo.com`
- **Password:** `demo123`

### Admin Account
- **Email:** `admin@demo.com`
- **Password:** `admin123`

### Additional Citizen Account
- **Email:** `jane@demo.com`
- **Password:** `demo123`

## Features Available in Demo Mode

### For Citizens:
1. **Login/Register** - Use the demo credentials above or create new accounts
2. **Report Issues** - Submit new civic issues with photos and location data
3. **View My Reports** - See all your submitted reports with status updates
4. **View Issue Map** - See all reported issues on an interactive map
5. **Profile Management** - Update your profile information

### For Admins:
1. **Admin Dashboard** - Overview of all issues and analytics
2. **All Issues Management** - View, filter, and manage all reported issues
3. **Analytics** - Detailed analytics and reporting
4. **Issue Status Updates** - Update issue status and add comments
5. **Admin Settings** - System configuration and settings

## Demo Data

The application includes pre-populated sample data:
- 6 sample issues across different categories
- 3 demo user accounts
- Sample analytics and reporting data
- Mock file uploads and location data

## How to Test

1. **Start the application** - Run `npm run dev` and open http://localhost:5173
2. **Login as Citizen** - Use `citizen@demo.com` / `demo123` to test citizen features
3. **Login as Admin** - Use `admin@demo.com` / `admin123` to test admin features
4. **Test Issue Reporting** - Submit new issues and see them appear in the system
5. **Test Status Updates** - As admin, update issue statuses and add comments

## Technical Notes

- All Supabase backend calls have been commented out
- Demo authentication system handles login/logout
- Demo data helpers simulate database operations
- File uploads return mock URLs
- Real-time updates are simulated (no actual real-time functionality)

## Switching Back to Production

To restore backend functionality:
1. Uncomment the Supabase imports in `src/App.tsx`
2. Comment out the demo imports
3. Restore the original authentication handlers
4. Update component imports to use `../lib/supabase` instead of `../lib/demo-data-helpers`

The demo mode is perfect for testing, demonstrations, and development without requiring backend setup.
