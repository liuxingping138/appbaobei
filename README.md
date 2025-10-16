# Family Growth Moments - WeChat Mini Program

## Project Overview

This WeChat Mini Program is designed to help families document and share their child's growth moments. It provides a platform for all family members to participate in recording precious moments of the child's development.

## Features

1. **Family Circle** - Similar to WeChat Moments, allowing family members to share photos and videos
2. **Baby Profile Management** - Track baby's basic information, health, and interests
3. **Growth Assessment** - Visualize development with radar charts
4. **Family Travel Footprint** - Record and display family trips on a map
5. **Time Machine** - Auto-generated weekly/monthly videos of the child's growth
6. **Family Group Chat** - Real-time communication among family members
7. **Growth Reports** - Export comprehensive growth reports

## Technical Architecture

- **Frontend**: WeChat Mini Program native framework
- **UI Components**: weui-miniprogram
- **Backend**: WeChat Cloud Development (CloudBase)
- **Database**: Cloud database for storing user data, baby information, moments, etc.
- **Cloud Functions**: Serverless functions for business logic
- **Cloud Storage**: For storing media files (photos, videos)

## Project Structure

```
appbaby/
├── frontend/              # Frontend code
│   ├── components/        # Reusable components
│   ├── pages/             # Page files
│   ├── utils/             # Utility functions
│   ├── test/              # Test files
│   ├── app.js             # App entry point
│   ├── app.json           # App configuration
│   └── sitemap.json       # Sitemap configuration
├── backend/               # Backend services
│   ├── cloudfunctions/    # Cloud functions
│   ├── database/          # Database models and initialization
│   ├── services/          # Business logic services
│   └── utils/             # Backend utility functions
├── requirements.md        # Detailed requirements document
└── README.md              # This file
```

## Getting Started

### Prerequisites

- WeChat Developer Tool
- Node.js (for development dependencies)
- WeChat Account with Mini Program permissions

### Installation

1. Clone the repository:
   ```bash
   git clone <repository-url>
   ```

2. Open the project in WeChat Developer Tool:
   - Open the `frontend` directory as a Mini Program project
   - Configure the AppID in `app.json`

3. Install dependencies for frontend:
   ```bash
   cd frontend
   npm install
   ```

4. Install dependencies for backend:
   ```bash
   cd backend
   npm install
   ```

5. Set up cloud development:
   - Create a cloud development environment in WeChat Developer Tool
   - Update the environment ID in `app.js`

### Deployment

1. Upload the frontend code using WeChat Developer Tool
2. Deploy cloud functions:
   - Navigate to the `backend` directory
   - Deploy cloud functions through WeChat Developer Tool
3. Initialize the database:
   - Run the database initialization script in the cloud environment

## Development Guidelines

### Code Structure

- Follow component-based development for reusable UI elements
- Use async/await for cloud function calls
- Implement error handling for all user interactions
- Maintain consistent styling with weui-miniprogram components

### Testing

- Test on different device sizes
- Verify accessibility for elderly family members
- Ensure smooth performance on low-end devices
- Test all user flows with different user roles

## Contributing

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Contact

For support or queries, please contact the development team.