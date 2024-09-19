## Users database schema 
        {
        "users": [
            {
                "user_id": "64e09a1f9a8c2b3f3a5d60a9",          # unique id       
                "username": "",                           # unique username, i.e. there can only be one user with the same time
                "password": "",                       # user email
                "email": "",                          # user password
                "display_name": "",                  # display name
                "lastlogindate": "2024-08-22 12:39:22.397803",          # when last logged in
                "accontcreatedate": "2024-08-22 12:39:22.397803",       # when is the user registration for the application
                "info": "tämä on",                # the user's ifno box that is visible to other users
                "bio": "",                # the user's bio box that is visible to other users
                "follower_count": 892,          # how many followers the user has
                "verification_code": "981142",   # if you don't remember the password, the settings page shows a hidden text with this 6-character code      
                "account_status": "loggedin",      # account status whether banned, logged in or logged out or terminated  
                "deactivate_account": false,        # whether the account has been suspended
                "user_role": "user",                     # user role i.e. is it normal user (user),system administrator (admin) or moderator (mod)
                "Verified": false,               # is a Verified user (true/false)
                "profile_picture_link": "",         # internet link to the image
                "country": "DE",               # countries.json, there are options in the file
                "group_whereis": [                  # in which groups user are
                    {
                        "group_id": "64e789a129c2b3f3a5d60a9",
                        "group_name": "Hiking Enthusiasts"
                    }
                ],
                "follow": [         # who the user follows
                    {
                        "user_id": "",      # who the user follows id
                        "username":""      # who the user follows username
                    }
                ],
                "followers": [      # who follows the user
                    {
                        "user_id": "",      # follower id
                        "username":""      # follower username
                    }
                ],
                "friends": [      # the user's friends
                    {
                        "user_id": "",      # user friend id
                        "username":""      # user friend username
                    }
                ],
                "bookmarks": [      # user post bookmarks
                    {
                        "post_id": "64e09a129c2b3f3a5d60a9"      # post_id what is in the bookmarks
                    }
                ],
                "liked_posts": [      # user liked posts
                    {
                        "post_id": "64e039a129c2b3f3a5d60a9",      # post_id
                        "like_date": "2024-08-22 14:05:00"      # when the post has been liked
                    }
                ],
                "commented_posts": [      # user commented posts
                    {
                        "post_id": "64e039a129c2b3f3a5d60a9",      # post id
                        "comment_id": "64e09a1239c2b3f3a5d60a9",      # comment id
                        "comment_date": "2024-08-22 14:10:00"      # when comment date lefted
                    }
                ],
                "settings": [                   # user-specific settings that the user can change freely
                    {
                        "profile_visibility": "private",    # means whether the user's profile is private or public, by default public
                        "last_time_changed_username": "2024-08-15",     # 
                        "language_settings": {
                            "default_language": "en",               # the application is bilingual, the default is English 
                            "additional_languages": ["fi", "sv", "de"]  # other languages
                        },   
                        "appearance_settings": {
                           "theme": "dark",         # whether dark or light theme
                           "font_size": "medium",   # how big is text (big, medium, small)
                           "dark_mode_schedule": {
                                "enabled": true,        # is the auto dark theme on
                                "start_time": "18:00",       # when dark theme starts
                                "end_time": "06:00"          # when dark theme ends
                            }
                        },
                        "notification_preferences": {      # 
                            "post_likes": true,      # notification come if someone likes post
                            "comments": true,      # notification come if someone comments post
                            "new_followers": false,      # notification come if someone follows
                            "mentions": true,            # notification come if someone mentions user
                            "group_invitations": false,      # notification come if someone invite user in group
                            "security_alerts": true     # secuity alerts
                        },
                        "security_settings": {      # secuity settings
                            "password_last_changed": "2024-08-15T10:30:00Z",      # when last time the password was changed
                            "session_management": {      
                                "active_sessions": [      # active sessions, i.e. devices that have been logged in with credentials
                                {
                                    "device": "iPhone 13",      # active session device name
                                    "ip_address": "192.168.1.1",      # active session device ip address
                                    "last_active": "2024-09-13T14:00:00Z"      # when was last active
                                }
                              ]
                            }
                          },
                        "blocked_users": [      # usernames of blocked users
                        ],
                        "miscellaneous_settings": {      # miscellaneous settings
                            "timezone": "Europe/Helsinki",      # which time zone the user has set
                            "auto_login": false,                # has the user selected "remember me"
                            "username_visibility": true         # 
                        },
                        "content_preferences": {       # Content settings
                            "preferred_topics": [    # primary topics for which the user wants recommendations
                              "technology",         
                              "sports",
                              "travel"
                            ],
                            "mute_keywords": [         # muted keywords that the user wants to mute
                              "politics",
                              "violence"
                            ]
                        },
                        "privacy_settings": {      # privacy settings
                           "show_online_status": false,      # can others see when the user is online
                           "profile_visible_to_followers_only": true,  # who can see the content of the user's profile, true or false
                           "allow_message_requests": true,      # whether the user accepts message requests
                           "login_alerts": true      # login alerts, on(true) and off(false)
                        },
                        "trusted_devices": [      # Trusted devices
                            {
                                "device_name": "iPhone 13",      # Trusted device name
                                "device_id": "12345abcdef"      # Trusted device id
                            }
                        ],
                        "account_recovery_options": {      # account recovery methods
                            "recovery_email": "recovery@example.com",      # recovery email
                            security_questions": [      # security questions
                        {      
                            "question": "What was your childhood pet's name?",      # question
                            "answer": "Fluffy"      # answer
                        }
                    ]
                },
                }
                ],
                "login_history": [      # user login history
                    {
                        "login_id": "",                                 # login id
                        "login_date": "2024-08-22 12:39:22.397803",      # login day
                        "ip_address": "192.168.0.1",      # login ip
                        "successful": true      # whether the login was successful(true) or not successful(false)
                    }
                ],
                "total_likes_received": 1200,       # total likes getted
                "total_comments_received": 300       # total comments getted
            }
            ]
        }

## Post database schema
        {
            "posts": [            # posts
                    {
                    "post_id": "64e09a129c2b3f3a5d60a9",        # post unique id
                    "user_id": "64e09a13429c2b3f3a5d60a9",      # id of the user who posted the post
                    "username": "",             # the user who made the post
                    "title": "",                # post title
                    "text": "",                 # post text
                    "like_count": 67,                 # how many people have liked the post
                    "publication_date": "2024-08-22 12:39:22.397803",    # date of publication of post
                    "post_tags": ["outdoors", "hiking", "nature"],      # post tags
                    "comments": [               # post comments
                            {
                                "comment_id": "64e09a129c2b3f3a5d60a9",     # comment unique id
                                "text": "",                         # the content of the comment
                                "comment_date": "2024-08-22",       # when comment lefted
                                "comment_likes": 12                       # how many people have liked the comment
                                "report_status": null  # whether the comment has been reported
                            }
                        ],
                    "post_likes": [               # post comments
                            {
                                "user_id": "64e09a129c2b3f3a5d60a9",     # user unique id
                                "like_date": "2024-08-22",       # when like lefted
                            }
                        ],
                    "edited": false,                    # it post been edited
                    "report_status": null,              # it post been reported
                    "warning_message": null,  # if the post has received a warning (admin or mod)
                    "reported_count": 0  # how many times the post has been reported
                    }
                ],
            }

## Group Database schema
        {
        "groups": [
            {
                "group_id": "64e09a1f9a8c2b3f3a5d60a9",      # group unique id   
                "group_name": "",               # group public name
                "Verified": true,               # is a Verified group(true/false)
                "group_status": "public",      # who can join the group (public or private)
                "group_privacy": "public",      # who can see the group in the list (public or private)
                "who_can_send": "members",      # who can send message (open, members, group_admin_only, )
                "group_last_activity": "2024-09-13",      # when was the last message sent
                "group_description": "",                 # group description
                "group_creation_date": "2023-05-15",      # when the group is created
                "group_creator": "64e309a1f9a8c2b3f3a5d60a9",      # who created the group
                "member_count": 150,
                "users_in_group": [                         # users who are members of the group
                    {
                        "user_id": "64e09a1f9a48c2b3f3a5d60a9",      # user id
                        "join_date": "2024-08-22 12:39:22.397803",      # when has joined the group
                        "user_group_role": "member"    # role in group (member/owner/invigilator)
                    }
                ],
                "group_message": [      # group messages
                    {
                        "message_id": "64e999a1f9a8c2b3f3a5d60a9",      # message id
                        "message_date": "2024-09-01",      # message send date
                        "message_content": "message"      # message content
                    }
                ],
                "user_restrictions": [
                    {
                        "user_id": "64e09a1f9a48c2b3f3a5d60a9",     # user id
                        "restriction_type": "mute",             # Blocked from sending messages
                        "restriction_start_date": "2024-09-01",      # restriction start date
                        "restriction_end_date": "2024-09-05"        # restriction end date
                    }
                ]
                "group_tags": ["outdoors", "hiking", "nature"]      # group tags
                "invite_policy": "group_admin_only",  # Who can invite members (group_admin_only, members, open_invite)
            }
        ]
        }

## Support Database schema
        {
            "support": [    #
                {
                    "ticket_id": "SUPPORT12345",    # unique_id
                    "issue": "Unable to log in",     # issue description
                    "status": "Resolved", # processing, Resolved, Unsolved
                    "submitted_date": "2024-08-20",     #Date of submmit
                    "submitted_by": {                    # information about the sender
                        "user_id": "64e09a1f9a8c2b3f3a5d60a9",    # user_id who sent the support request
                        "username": ""    # username who sent the support request
                    },
                    "priority": "High",    # how important its get problem resolved(High, medium, low)
                    "responses": [    # messaging handler and when the problem is
                        {
                            "response_id": "RESP12345",    # response id
                            "response_date": "2024-08-21",    # response date
                            "response_by": "",    # who has accepted the support ticket, handler fills this out
                            "response_message": ""    # what the recipient has received, handler fills this out
                        }
                    ],
                    "ticket_history": [    # Event history
                        {
                            "event": "",    # what has been done in a certain event
                            "event_date": "2024-08-20"    # event day
                        }
                    ],
                    "resolution_type": "Password Reset"    # type of problem statement
                }
            ]
        }

## Report Database schema
        {
            "report": [
                {
                    "issue_id": "REPORT98765",    # unique issue id 
                    "post_id": "64e09a129c2b3f3a5d60a9",    # to which post is thty report
                    "post_id": "64e09a129c2b3f3a5d60a9",    # which user is thty report
                    "issue_type": "inappropriate content", # issue type (make a problem list)
                    "status": "Under review",    # report issue status
                    "report_date": "2024-08-22",    # report date
                    "reported_by": {    
                        "user_id": "64e09a1f9a8c2b3f3a5d60a9",      # user id who report 
                        "username": "JaneDoe"      # username
                    },  
                    "report_comments": "",   # the repairer can comment on why he/she has reported
                    "report_history": [     # processing history
                        {
                          "event": "Report submitted",    # event description, mitä on tehty 
                          "event_date": "2024-08-22"    # event day
                        }
                    ],
                    "reported_content": {    # which is reported
                        "content_text": ""    # reported content
                      },               
                      "resolution": {    # how has been found out
                        "resolution_type": "Post hidden",    # type of solution
                        "resolution_date": "2024-08-24",    # date of solution
                        "resolved_by": "Mod123"    # solver, handler fills this out
                      },
                      "report_status_update": {    # report status update
                        "notified_user": true,    # whether the reporter has been notified
                        "notification_date": "2024-08-25"    # notified date
                      }
                }
            ]
        }


### File Structure
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
