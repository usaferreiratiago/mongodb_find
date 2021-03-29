#these command is similar the command Select * from in Database SQL
# mongodb_find              #"Retrieve Everything"

db.accounts.find()


#mongo_db_find_with_filter


db.accounts.find(
    {
        "$and": [
            {
                "limit": 9000.0
            },
            {
                "account_id": 371138.0
            },
            {
                "products": "InvestmentStock"
            }
        ]
    }
).sort({"limit": 1.0})
