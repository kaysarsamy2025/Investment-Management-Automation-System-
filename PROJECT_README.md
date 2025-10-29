# Investment Management Automation System (IMAS)

## 📋 Project Overview

IMAS is a comprehensive web-based platform designed to bridge the gap between entrepreneurs and investors, facilitating a more efficient and transparent funding process through AI-driven recommendations and automated investment management.

## 🎯 Key Features

### For Entrepreneurs
- **Project Management**: Create, manage, and track investment projects
- **Funding Progress**: Real-time monitoring of investment rounds
- **Investor Engagement**: Communicate with potential investors
- **Analytics Dashboard**: Track project performance and metrics

### For Investors
- **AI-Powered Recommendations**: Intelligent project matching using ZAI SDK
- **Project Discovery**: Advanced filtering and search capabilities
- **Portfolio Management**: Track and analyze investment performance
- **Market Insights**: Data-driven investment trends and analytics

### Platform Features
- **Real-time Communication**: Secure messaging via Socket.IO
- **Transaction Processing**: Integrated payment systems
- **Data Analytics**: Comprehensive reporting and insights
- **Responsive Design**: Mobile-first UI with Tailwind CSS

## 🛠 Technology Stack

### Frontend
- **Framework**: Next.js 15 with App Router
- **Language**: TypeScript 5
- **Styling**: Tailwind CSS 4
- **UI Components**: shadcn/ui (New York style)
- **Icons**: Lucide React
- **State Management**: Zustand
- **Data Fetching**: TanStack Query

### Backend
- **Database**: Prisma ORM with SQLite
- **Real-time**: Socket.IO
- **API**: Next.js API Routes
- **AI Integration**: ZAI Web Development SDK

### Development Tools
- **Package Manager**: npm
- **Linting**: ESLint
- **Type Checking**: TypeScript
- **Build Tool**: Next.js

## 📁 Project Structure

```
imas-project/
├── src/
│   ├── app/                    # Next.js App Router pages
│   │   ├── page.tsx           # Landing page
│   │   ├── entrepreneur/      # Entrepreneur dashboard
│   │   ├── investor/          # Investor dashboard
│   │   ├── api/               # API routes
│   │   └── layout.tsx         # Root layout
│   ├── components/            # React components
│   │   └── ui/                # shadcn/ui components
│   ├── lib/                   # Utility libraries
│   │   ├── db.ts              # Database client
│   │   ├── socket.ts          # Socket.IO configuration
│   │   └── utils.ts           # Helper functions
│   └── hooks/                 # Custom React hooks
├── prisma/
│   └── schema.prisma          # Database schema
├── public/                    # Static assets
├── package.json               # Dependencies and scripts
├── tsconfig.json              # TypeScript configuration
├── tailwind.config.ts         # Tailwind CSS configuration
├── next.config.ts             # Next.js configuration
└── README.md                  # This file
```

## 🚀 Getting Started

### Prerequisites
- Node.js 18+ 
- npm or yarn

### Installation

1. **Extract the archive**
   ```bash
   tar -xzf imas-project.tar.gz
   cd imas-project
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Set up the database**
   ```bash
   npm run db:push
   ```

4. **Start the development server**
   ```bash
   npm run dev
   ```

5. **Open your browser**
   Navigate to `http://localhost:3000`

## 📊 Database Schema

The application uses Prisma ORM with SQLite and includes the following main models:

- **User**: Entrepreneurs, investors, and administrators
- **Project**: Investment projects and proposals
- **Investment**: Investment transactions and records
- **Message**: Real-time communication between users
- **Recommendation**: AI-powered investment recommendations

## 🔧 Configuration

### Environment Variables
Create a `.env.local` file in the root directory:

```env
# Database
DATABASE_URL="file:./dev.db"

# ZAI SDK (optional - for AI features)
ZAI_API_KEY="your-zai-api-key"

# NextAuth
NEXTAUTH_SECRET="your-secret-key"
NEXTAUTH_URL="http://localhost:3000"
```

### Database Configuration
The database schema is defined in `prisma/schema.prisma`. To modify:

1. Edit the schema file
2. Run `npm run db:push` to apply changes
3. Use `npm run db:studio` to open Prisma Studio

## 🎨 UI Components

The project uses shadcn/ui components located in `src/components/ui/`. These are pre-built, accessible components that follow modern design principles.

### Key Components Used
- Cards, Buttons, Forms
- Navigation, Sidebars
- Charts, Tables
- Dialogs, Modals
- Loading States, Skeletons

## 🤖 AI Integration

The platform integrates ZAI Web Development SDK for:
- **Project Recommendations**: AI-powered matching
- **Market Analysis**: Investment trend insights
- **Risk Assessment**: Project evaluation

## 📱 Features Overview

### Landing Page (`/`)
- Hero section with value proposition
- Real-time statistics
- Success stories
- Feature highlights

### Entrepreneur Dashboard (`/entrepreneur`)
- Project creation and management
- Funding progress tracking
- Investor communications
- Performance analytics

### Investor Dashboard (`/investor`)
- AI-powered recommendations
- Project discovery and filtering
- Portfolio management
- Market insights

## 🔒 Security Features

- Secure authentication with NextAuth.js
- Role-based access control
- Encrypted communications
- Safe transaction processing
- Data privacy protection

## 📈 Performance Optimizations

- Server-side rendering (SSR)
- Client-side caching
- Optimized database queries
- Lazy loading components
- Image optimization

## 🧪 Testing

The project includes comprehensive testing:
- Component testing
- API endpoint testing
- Database integration testing
- E2E testing setup

## 📚 API Documentation

### Authentication
- `/api/auth/*` - NextAuth.js endpoints

### Projects
- `GET /api/projects` - List all projects
- `POST /api/projects` - Create new project
- `GET /api/projects/[id]` - Get project details
- `PUT /api/projects/[id]` - Update project

### AI Recommendations
- `GET /api/ai/recommendations` - Get AI-powered recommendations

### Analytics
- `GET /api/analytics` - Get platform analytics

## 🚀 Deployment

### Production Build
```bash
npm run build
npm start
```

### Environment Setup
1. Set production environment variables
2. Configure production database
3. Set up SSL certificates
4. Configure domain and DNS

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Run tests and linting
5. Submit a pull request

## 📄 License

This project is part of an undergraduate thesis for the Investment Management Automation System (IMAS).

## 📞 Support

For questions or support regarding this project, please refer to the project documentation or contact the development team.

---

**Project ID**: 223311241  
**Course**: CSE 418 - Project or Thesis with Seminar Part I  
**University**: Varendra University  
**Department**: Computer Science and Engineering  
**Submission Date**: August 24, 2025