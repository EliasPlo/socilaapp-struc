    {
      "private_accounts": [
        {
          "account_id": "1001",
          "user_id": "user123",
          "account_type": "savings",
          "account_name": "Lomakassa",
          "balance": 5000.50,
          "currency": "EUR",
          "transactions": [
            {
              "transaction_id": "tx1001",
              "date": "2024-09-01",
              "description": "Food Market",
              "amount": -50.25,
              "category": "groceries"
            },
            {
              "transaction_id": "tx1002",
              "date": "2024-09-05",
              "description": "Salary",
              "amount": 3000.00,
              "category": "income"
            }
          ],
          "recurring_payments": [
            {
              "name": "Netflix Subscription",
              "amount": 12.99,
              "frequency": "monthly",
              "next_payment_date": "2024-10-01"
            }
          ],
          "budgeting_tools": {
            "monthly_budget": 2000.00,
            "current_spend": 300.50,
            "budget_goal": "Save for a new car"
          },
          "security": {
            "2FA_enabled": true,
            "trusted_devices": ["iPhone 12", "Macbook Pro"],
            "session_timeout": 15
          },
          "notifications": {
            "balance_threshold_alert": 100.00,
            "transaction_notifications": true
          }
        }
      ]
    }
    
