1. Total Transactions = COUNT(fraudTest[transaction id])
2. Total Fraud = COUNTAX(
    FILTER('fraudTest', 'fraudTest'[is_fraud] = 1),
    fraudTest[transaction id]
3. Fraud Rate % = DIVIDE(fraudTest[Total Fraud],fraudTest[Total Transactions],0)
