# Expendidator

A little expenses calculator

When you create your own Firebase app, search and replace `https://expenditator.firebaseio.com` with your app's Firebase url.

# Data

Take a look at sample-expenses.json to get an idea of how the data is structured. You should also load it up:

	curl -X PUT https://expenditator.firebaseio.com/.json --data @sample-expenses.json

Some curl commands to try

	curl https://expenditator.firebaseio.com/expenses.json
	curl https://expenditator.firebaseio.com/expenses/id1/amount.json
	curl -X PATCH https://expenditator.firebaseio.com/expenses/id1.json -d '{"amount": 20}'          
	curl -X PUT https://expenditator.firebaseio.com/expenses/id1.json -d '{"amount": 20}'
	curl -X POST https://expenditator.firebaseio.com/expenses.json -d '{"amount": 20}'

