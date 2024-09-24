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
