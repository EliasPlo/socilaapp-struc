    {
      "business_accounts": [
        {
          "account_id": "2001",
          "business_id": "biz456",
          "business_name": "ABC Oy",
          "account_type": "current",
          "balance": 150000.75,
          "currency": "EUR",
          "transactions": [
            {
              "transaction_id": "tx2001",
              "date": "2024-08-30",
              "description": "Office Supplies",
              "amount": -500.00,
              "category": "office_expenses"
            },
            {
              "transaction_id": "tx2002",
              "date": "2024-09-03",
              "description": "Client Payment",
              "amount": 10000.00,
              "category": "income"
            }
          ],
          "invoices": [
            {
              "invoice_id": "inv123",
              "issued_date": "2024-08-25",
              "due_date": "2024-09-10",
              "amount": 5000.00,
              "status": "paid"
            }
          ],
          "payroll_management": {
            "employees": [
              {
                "employee_id": "emp001",
                "name": "John Doe",
                "salary": 3000.00,
                "last_payment_date": "2024-08-31"
              }
            ]
          },
          "security": {
            "2FA_enabled": true,
            "trusted_devices": ["Office Desktop", "Business Laptop"],
            "session_timeout": 30
          },
          "notifications": {
            "low_balance_alert": 5000.00,
            "transaction_notifications": true,
            "invoice_reminders": true
          }
        }
      ]
    }
    
