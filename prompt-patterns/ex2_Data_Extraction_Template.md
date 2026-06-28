1. Choose an unstructured text (e.g., "John Doe, age 29, lives in Paris and works as a software engineer.").

  - answer: "Jerry Peace, age 19, lives in Poland and works as a  Robotics engineer."

2. Create a template prompt:

    "Extract the following fields from 'Jerry Peace, age 19, lives in Poland and works as a  Robotics engineer.':Name, Age, Location, Occupation. Return the output in JSON format."


    OUTPUT:
        {
    "Name": "Jerry Peace",
    "Age": 19,
    "Location": "Poland",
    "Occupation": "Robotics engineer"
    }
   

3. Validate the output and ensure consistency across multiple inputs.
    The output and the multiple inputs are consistency, the data types marches at all fields in the text.

