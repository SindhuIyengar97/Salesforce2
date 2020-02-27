# Salesforce2
Requirement:-

When a lead is converted
Assign Account Name to Company Name

1)If Status is 'Open-Not Contacted'
  Create a Task with Subject Call
  Set Due_date to 1 week from today

2)If Status is 'Working-Contacted'
 Set Rating to 'Warm'
 
3)If Status is 'Closed-Converted'
  Set Rating to 'Hot'
  Create Account with Account Name = Company Name
  Contact => First Name, Last Name
  Opportunity oppName => AccountName Concatenated with (opp)
  
4)If Status is 'Closed-Not Converted'
  Set Rating to 'Cold'
  Create new field Reason
  If Reason is Blank Throw Error to provide Reason
  
