## file structure
    socialapp/
    │
    ├── backend/                                   # Backend server files
    │   ├── nodejs/                                # Node.js backend
    │   │   ├── config/                            # Config files
    │   │   │   └── dbConfig.ts                    # MongoDB connection config
    │   │   ├── controllers/                       # Logic for handling requests
    │   │   │   ├── postController.ts        # Post-facing functions for handling HTTP requests
    │   │   │   ├── moderationController.ts        # -facing functions for handling HTTP requests
    │   │   │   ├── supportController.ts        # support-facing functions for handling HTTP requests
    │   │   │   ├── reportController.ts        # report-facing functions for handling HTTP requests
    │   │   │   ├── groupController.ts        # group-facing functions for handling HTTP requests
    │   │   │   ├── commentController.ts        # comment-facing functions for handling HTTP requests
    │   │   │   ├── userController.ts        # User-facing functions for handling HTTP requests
    │   │   │   └── authController.ts        # auth controller
    │   │   ├── models/                    # MongoDB models (schemas)
    │   │   │   ├── Post.ts       # Post document template
    │   │   │   ├── User.ts       # User document template
    │   │   │   ├── Support.ts       # Support document template
    │   │   │   ├── Report.ts       # Report document template
    │   │   │   ├── Group.ts       # Group document template
    │   │   │   └── Comment.ts       # Comment document template
    │   │   ├── routes/                        # API routes
    │   │   │   ├── postRoutes.ts             # Routes for posts
    │   │   │   ├── userRoutes.ts         # Routes for user
    │   │   │   ├── supportRoutes.ts         # Routes for support
    │   │   │   ├── reportRoutes.ts         # Routes for report
    │   │   │   ├── groupRoutes.ts         # Routes for group
    │   │   │   ├── commentRoutes.ts         # Routes for comment
    │   │   │   ├── moderationRoutes.ts       # Routes for AI moderation
    │   │   │   └── authRoutes.ts               # Authentication routes
    │   │   ├── middlewares/                   # Middleware for authentication, validation, 
    │   │   │   ├── logger.ts       # logger middleware
    │   │   │   └── authMiddleware.ts        # auth middleware
    │   │   ├── translations/        # 
    │   │   │   ├── de.json        # 
    │   │   │   ├── fi.json       # 
    │   │   │   ├── se.json       # 
    │   │   │   └── en.json        # 
    │   │   ├── utils/                    # Utility functions 
    │   │   │   ├── validation.ts         # Input validation logic
    │   │   │   ├── errorHandler.ts       # Custom error handling 
    │   │   │   └── jwtUtils.ts           # JWT for authentication
    │   │   ├── app.ts                    # Main entry point of the app, Express app config
    │   │   ├── tsconfig.json             # Backend TypeScript config
    │   │   ├── package.json              # Dependencies and scripts for backend 
    │   │   ├── package-lock.json         # backend TypeScript config
    │   │   ├── server.ts                 # Starts the Node.js server, Server entry point
    │   │   └── .env                      # Environment variables (DB connection, etc.)
    │   └── python/                       # Python-based content moderation
    │       ├── models/                   # Machine learning models for moderation
    │       │   └── content_moderation_model.pkl
    │       ├── scripts/                   # Python scripts for moderation tasks
    │       │   ├── content_moderation.py
    │       │   └── preprocess.py
    │       ├── api/               # Python Flask/FastAPI for serving AI moderation APIs
    │       │   └──moderation_api.py 
    │       └── requirements.txt                   # Python dependencies
    ├── frontend/                                  # Frontend application
    │   ├── node_modules/                 # Public static files
    │   ├── public/                 # Public static files
    │   │   ├── index.html            # Main HTML file
    │   │   ├── manifest.json
    │   │   ├── assets/         # 
    │   │   │   ├── img/      # Contains all the static image files for the application, grouped into subfolders
    │   │   │   │   ├── logo.png    # site logo
    │   │   │   │   ├── verified/           # 
    │   │   │   │   │   ├── admin-icon.png      # admin user profile badge, next to username
    │   │   │   │   │   ├── mod-icon.png        # mod user profile badge, next to username
    │   │   │   │   │   ├── blue-verified.png      # normal verified user badge, next to username
    │   │   │   │   │   ├── green-verified.png     # upper normal user badge, next to username
    │   │   │   │   │   ├── gray-verified.png     # government account badge, next to username
    │   │   │   │   │   ├── gold-verified.png     # business account badge, next to username
    │   │   │   │   │   └── red-verified.png     # high profile person badge, next to username
    │   │   │   │   ├── avatars/                # options for profile picture
    │   │   │   │   │   ├── default-avatar.png  # the basic profile picture when it hasnt changed
    │   │   │   │   │   ├── avatar.png      # option 1 to change profile picture
    │   │   │   │   │   ├── avatar1.png     # option 2 to change profile picture
    │   │   │   │   │   ├── avatar2.png     # option 3 to change profile picture
    │   │   │   │   │   ├── avatar3.png     # option 4 to change profile picture
    │   │   │   │   │   ├── avatar4.png     # option 5 to change profile picture
    │   │   │   │   │   ├── avatar5.png     # option 6 to change profile picture
    │   │   │   │   │   ├── avatar6.png     # option 7 to change profile picture
    │   │   │   │   │   ├── avatar7.png     # option 8 to change profile picture
    │   │   │   │   │   ├── avatar8.png     # option 9 to change profile picture
    │   │   │   │   │   ├── avatar9.png     # option 10 to change profile picture
    │   │   │   │   │   ├── avatar10.png      # option 11 to change profile picture
    │   │   │   │   │   ├── avatar11.png      # option 12 to change profile picture
    │   │   │   │   │   ├── avatar12.png      # option 13 to change profile picture
    │   │   │   │   │   ├── avatar13.png      # option 14 to change profile picture
    │   │   │   │   │   ├── avatar14.png      # option 15 to change profile picture
    │   │   │   │   │   ├── avatar15.png      # option 16 to change profile picture
    │   │   │   │   │   └── avatar16.png      # option 17 to change profile picture
    │   │   │   │   └── icons/                # icons
    │   │   │   │       ├── home-icon.png      # home button icon
    │   │   │   │       ├── like-icon.png      # like button icon
    │   │   │   │       ├── is-liked-icon.png   # is liked button icon
    │   │   │   │       └── user-icon.png      # (not in use)
    │   │   │   ├── fonts/                    # Custom fonts that your web app uses.
    │   │   │   │   ├── Roboto-Regular.ttf      # 
    │   │   │   │   └── OpenSans-Bold.ttf      # 
    │   │   │   ├── styles/                  # Global styles, theme files, and CSS/SCSS files.
    │   │   │   │   ├── global.css          # global css 
    │   │   │   │   ├── reset.css           # 
    │   │   │   │   └── themes/            # themes
    │   │   │   │       ├── dark-theme.css      # dark theme css 
    │   │   │   │       └── light-theme.css      # light theme css
    │   │   │   ├── ts/                      # Any custom TypeScript files that are not part of npm packages.
    │   │   │   │   └── custom-plugin.ts      # 
    │   │   │   ├── svg/                    # SVG icons and images for a lightweight, scalable UI.
    │   │   │   │   ├── logo-icon.png      # 
    │   │   │   │   ├── icon-menu.svg      # menu button icon
    │   │   │   │   └── icons/             # 
    │   │   │   │       └── search-icon.svg      # Search icon
    │   │   │   ├── favicon/            # Favicon and related image files for the browser tab.
    │   │   │   │   ├── favicon.ico      # App Favicon
    │   │   │   │   └── favicon.png      # 
    │   │   │   └── data/                 # Static data like JSON files for use in the application.
    │   │   │       ├── countries.json            # user options for country selection
    │   │   │       └── theme-settings.json      # theme settings
    │   │   └──locales/                 # locales
    │   │      ├── fi/                 # Finnish
    │   │      │   └── common.json      # Finnish translation
    │   │      ├── en/                 # English
    │   │      │   └── common.json      # English translation
    │   │      ├── de/                 # German
    │   │      │   └── common.json      # German translation
    │   │      └── se/                 # Swedish
    │   │           └── common.json      # Swedish translation
    │   ├── src/                     # React source files
    │   │   ├── components/          # Reusable React components
    │   │   │   ├── Navbar.tsx         # Navbar component, which appears on every page
    │   │   │   ├── Footer.tsx         # Footer component, which appears on every page
    │   │   │   ├── Bookmark.tsx           # Bookmark component, which appears on every post 
    │   │   │   ├── BookmarkList.tsx     # BookmarkList component, which appears on every post BookmarkList
    │   │   │   ├── FeedbackForm.tsx         # feedback form
    │   │   │   ├── PostCard.tsx            # PostCard component
    │   │   │   ├── NotFound.tsx          # 404 Page, if the page is not found on the page
    │   │   │   ├── PrivateRoutes.tsx        # a file that defines which pages users can access
    │   │   │   ├── LanguageSwitcher.tsx       # page language change element6
    │   │   │   └── Sidebar.tsx             # sidebar componet, which appears on every page, 
    │   │   ├── pages/                    # React pages
    │   │   │   ├── AdminPanel.tsx        # admin control panel from which you can manage the page and users
    │   │   │   ├── Home.tsx          # Homepage
    │   │   │   ├── Profile.tsx           # User profile page
    │   │   │   ├── PostDetails.tsx       # Single post page
    │   │   │   ├── Login.tsx             # Login page
    │   │   │   ├── Group.tsx             # groups page 
    │   │   │   ├── Create.tsx             # a page where you can create a group or publish a post
    │   │   │   ├── Support.tsx             # Support page recommendations page
    │   │   │   ├── Report.tsx             # Report page
    │   │   │   ├── Recommendations.tsx       # recommendations page
    │   │   │   ├── Account.tsx               # Account Page
    │   │   │   ├── Chat.tsx                # Chat Page all register users can chat in this site
    │   │   │   ├── Register.tsx          # Signup/Register page
    │   │   │   ├── Notifications.tsx       # Notifications page
    │   │   │   ├── Help.tsx              # Help page
    │   │   │   ├── Info.tsx              # Info page
    │   │   │   ├── Privacy.tsx           # Privacy page
    │   │   │   └── Settings.tsx          # User settings pag
    │   │   ├── context/                 # Global context/state management (e.g., AuthContext)
    │   │   │   ├── AuthContext.tsx             # defines the context related to user authentication
    │   │   │   ├── PostContext.tsx             # controls the space associated with posts
    │   │   │   └── ThemeContext.tsx            # controls theme-related settings
    │   │   ├── hooks/                    # Custom React hooks
    │   │   │   ├── useAuth.ts              # 
    │   │   │   ├── useFetch.ts            # 
    │   │   │   └── useForm              # 
    │   │   ├── services/                 # API service calls to backend
    │   │   │   ├── postService.js      # 
    │   │   │   ├── api.js           # 
    │   │   │   └── authService.js      # 
    │   │   ├── utils/                   # Utility functions
    │   │   │   ├── authUtils.ts    # authUtils, Help functions related to authentication
    │   │   │   ├── fetchUtils.ts      # fetchUtils, For handling API calls.
    │   │   │   ├── storageUtils.ts     # storageUtils, Data processing in local storage
    │   │   │   ├── validationUtils.ts    # validationUtils, For field input validation
    │   │   │   └── dateUtils.ts        # dateUtils, For processing and formatting dates and times.
    │   │   ├── App.tsx                        # Main React component
    │   │   ├── index.tsx                 # Entry point for React
    │   │   ├── i18n.ts             # 
    │   │   ├── ReportWebVitals.ts      # 
    │   │   └── styles/                   # CSS/SCSS files for styling
    │   │        ├── index.css      # index css
    │   │        ├── global.css      # global.css
    │   │        └── App.css      # App css
    │   ├── tsconfig.json             # TypeScript configuration
    │   ├── next.config.js            # supported languages
    │   ├── package.json               # Dependencies and scripts for Frontend 
    │   ├── package-lock.json          # Frontend TypeScript config
    │   └── .env                     # Frontend environment variables (API endpoints,)
    ├── database/                      # Database configuration and migration files
    │   └── seed.js                  # Script to seed the database with sample data
    ├── /logs               # Logs for tracking
    │   ├── errorlogs.txt      # Logs for error tracking
    │   ├── userlogs.txt       # Logs for user events tracking
    │   ├── supporrtlogs.txt       # Logs for support messages tracking
    │   └── .   
    ├── next.config.js              # supported languages, 
    ├── tsconfig.json               # Root-level TypeScript config
    ├── .gitignore                  # files that git ignores
    └── .env                        # Environment variables (DB_URI, API_KEYS,etc.)    
