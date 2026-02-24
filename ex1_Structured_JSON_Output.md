1. Write a prompt that asks for unstructured information (e.g., “List three cities with their populations.”).
    - Answer: "List four states in Nigeria with their population"

    **OUTPUT**:
    Here are **four states in Nigeria with their estimated populations** (based on recent demographic data): ([Gistfulnaija][1])

    1. **Lagos State** – about **21,000,000** people ([Gistfulnaija][1])
    2. **Kano State** – about **14,300,000** people ([Gistfulnaija][1])
    3. **Katsina State** – about **9,300,000** people ([Gistfulnaija][1])
    4. **Kaduna State** – about **8,300,000** people ([Gistfulnaija][1])

    These figures are estimates and can vary by source and year. ([Gistfulnaija][1])

    [1]: https://gistfulnaija.com/nigerias-top-10-most-populous-states-in-2024/?utm_source=chatgpt.com "Nigeria's Top 10 Most Populous States in 2024 - Gistfulnaija"

2. Rewrite the prompt to enforce structured JSON output:

    Example: “Return the following in JSON format: [{city: string, population: number}].”

    - Answer: "List four states in Nigeria with their population. Return the following in JSON formate. [{city: string, population: number}]."

    **OUTPUT**:
    ```json
    [
    {
        "city": "Lagos",
        "population": 21000000
    },
    {
        "city": "Kano",
        "population": 14300000
    },
    {
        "city": "Katsina",
        "population": 9300000
    },
    {
        "city": "Kaduna",
        "population": 8300000
    }
    ]
    ```

3. Test with multiple inputs and verify the JSON stays valid.

    **OUTPUT**:

    To ensure the JSON output remains **valid and consistent** across multiple inputs, here’s a verification process using your previous example:

    ---

    ### **Test Input 1**

    > List four states in Nigeria with their populations.

    **JSON Output:**

    ```json
    [
    { "city": "Lagos", "population": 21000000 },
    { "city": "Kano", "population": 14300000 },
    { "city": "Katsina", "population": 9300000 },
    { "city": "Kaduna", "population": 8300000 }
    ]
    ```

    ✅ **Check:**

    * Proper JSON array structure
    * Each object has **city** (string) and **population** (number)
    * All keys are consistent

    ---

    ### **Test Input 2**

    > List four other states in Nigeria with their populations.

    **Example JSON Output:**

    ```json
    [
    { "city": "Oyo", "population": 7200000 },
    { "city": "Rivers", "population": 7600000 },
    { "city": "Enugu", "population": 4000000 },
    { "city": "Imo", "population": 5000000 }
    ]
    ```

    ✅ **Check:**

    * JSON remains valid
    * Key names and types remain consistent with the first output
    * Format is reusable for programmatic parsing

    ---

    ### **Conclusion**

    * The **JSON format stays valid** for multiple inputs as long as:

    1. An array of objects is used `[...]`
    2. Each object has **city** as a string and **population** as a number
    3. Commas and braces are correctly placed

    If you want, I can create a **template function** that automatically converts any list of states and populations into **valid JSON** in this format. This ensures full consistency for any number of entries.

    Do you want me to do that?

