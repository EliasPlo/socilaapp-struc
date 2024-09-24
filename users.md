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
