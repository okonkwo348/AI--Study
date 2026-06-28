1. Choose a math or coding problem (e.g., "Calculate the factorial of 5").
    OUTPUT:
    The factorial of 5 (written as 5!) means multiplying 5 by all the positive integers less than it down to 1:

    5! = 5 × 4 × 3 × 2 × 1
    5! = 120


2. Prompt the model: "Let's think step by step before answering."

    OUTPUT:
    Sure! Let’s calculate **5!** step by step.

    **Step 1:** Start with the definition of factorial:

    [
    n! = n \times (n-1) \times (n-2) \times \dots \times 1
    ]

    **Step 2:** Apply it to 5:

    [
    5! = 5 \times 4 \times 3 \times 2 \times 1
    ]

    **Step 3:** Multiply step by step:

    * 5 × 4 = 20
    * 20 × 3 = 60
    * 60 × 2 = 120
    * 120 × 1 = 120

    **Final Answer:**
    [
    5! = 120
    ]


3. Compare outputs with and without the reasoning instruction.

    The first output of the prompt without reasoning instruction "Calculate the factorial of 5" gives an unexplanatory answer which is not step by step. While the last prompt with reasoning instruction "Let's think step by step before answering." gives an output that is explanatory and step by step approached in solving the problem.