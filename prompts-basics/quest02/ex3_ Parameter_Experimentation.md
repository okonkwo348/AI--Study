1. Use the same prompt with temperature = 0.2 and then with temperature = 0.9.

    - Temperature = 0.2

        OUTPUT:

        With a **low temperature (0.2)**, the AI gives very predictable, common answers. So the output would likely be:

        1. Python
        2. Java
        3. C++

        These are among the most widely known and commonly referenced programming languages.

    - Temperature = 0.9

        OUTPUT: 
        With a **high temperature (0.9)**, the AI is more creative and less predictable. So instead of the most common answers, you might get something more varied like:

        1. Rust
        2. Elixir
        3. Haskell

        At higher temperature, the model is more likely to pick less obvious or less frequently mentioned languages instead of always defaulting to Python, Java, or C++.




2.  Repeat with different top-p values (e.g., 0.5 vs 1).

    top-p = 0.5

    OUTPUT:
    With **top-p = 0.5** (nucleus sampling), the AI only chooses from the most probable answers that together make up the top 50% of likelihood. This makes the output focused but still slightly varied.

        A likely result would be:

        1. Python
        2. JavaScript
        3. Java

        Because these languages are very common, they usually fall within the highest-probability group that the model is allowed to sample from when top-p is set to 0.5.


    top-p =1

    OUTPUT:

    With **top-p = 1**, the model can sample from the entire probability distribution (no restriction). That means it can choose both very common and less common answers.

    A possible output could be:

    1. Python
    2. Kotlin
    3. Haskell

    Since top-p is unrestricted, the response may include a mix of very popular and more niche programming languages, depending on randomness.


3. Record how the style, randomness, and focus of responses change.

    - Temperature at 0.2 give a low randomness output which is predictable, focuss and standard. Popular languages like python, java and C++ was used.
    - Temperature at 0.9 gives an high randomness output that is creative and exploratory. The model was creative giving unpopular and likely unhard languages like Rust, Elixir and Haskell.
    - Top-p at 0.5 give an output that only uses the most likely word, very safe and focuse, while at top-p at 1.0 the output is chooses from many words option and diverse that are quite unknown but to be explored.