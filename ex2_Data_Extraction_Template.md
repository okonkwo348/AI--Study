1. Choose an unstructured text (e.g., "John Doe, age 29, lives in Paris and works as a software engineer.").

    OUTPUT:
    * **Name and Age:** John Doe, 29 years old.
    * **Location:** Lives in Paris.
    * **Occupation:** Works as a software engineer.

2. Create a template prompt:

    "Extract the following fields from the text: Name, Age, Location, Occupation. Return the output in JSON format."

    OUTPUT:

        ```json
    {
    "Name": "John Doe",
    "Age": 29,
    "Location": "Paris",
    "Occupation": "Software engineer"
    }
    ```

3. Validate the output and ensure consistency across multiple inputs.
    The output and the multiple inputs are consistency, the data types marches at all fields.
