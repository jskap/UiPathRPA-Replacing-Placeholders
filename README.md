# UiPathRPA-Replacing-Placeholders
Get input information and use it to fill in the placeholders in a string.

You have the following template: "Hello Mr <first_name> <last_name>, we would like to invite you to our opening event next week 
on <day_of_week>. Please confirm by the end of current week.

Create a workflow to get input from the user and replace the provided input data in the phrase above.

Note: Please create a string variable with the text above.

In UiPath Studio, create a new project and follow the following steps:

  1. Start the project as sequence and create 3 string variables to store the first name, last name and the day of the week, 
     respectively.
     
  2. Use 3 'Input Dialog' activities to get the input from the user.
  
  3. Use the 'Replace' method in 'Assign' activities for each of the 3 strings with input data: 
  VariableName = VariableName.Replace("<parameter>",StringVariable.Trim). In order to preserve the formatting, use the 
  'Trim' method after each string variable to cut any unwanted spaces.
  
  4. Print the output using a 'Write Line' activity.
  
