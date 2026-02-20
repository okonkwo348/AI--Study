1. Use the same prompt with temperature = 0.2 and then with temperature = 0.9.

    **Prompt:**

    > “Summarize the main AI techniques in 5 bullet points.”

    ---

    ### **1️⃣ Temperature = 0.2** (low randomness)

    * Very **deterministic and focused**, little variation if repeated.

    * **Machine Learning (ML):** Algorithms that learn patterns from data.

    * **Deep Learning (DL):** Neural networks modeling complex patterns.

    * **Natural Language Processing (NLP):** Machines understanding human language.

    * **Computer Vision:** Machines analyzing images and videos.

    * **Reinforcement Learning (RL):** Learning by rewards and trial-and-error.

    **Observation:**

    * Output is **predictable, accurate, and standard**.
    * Suitable when you want **reliable and factual results**.

    ---

    ### **2️⃣ Temperature = 0.9** (high randomness)

    * More **creative, diverse, and exploratory** wording.

    * **Pattern-Learning Systems:** Algorithms that detect trends in datasets.

    * **Neural Deep Networks:** Deep models handling complex tasks.

    * **Language Comprehension Engines:** AI that reads, writes, or chats with humans.

    * **Visual Intelligence Tools:** Systems interpreting images or video content.

    * **Trial-and-Error Learners:** AI agents learning through rewards and mistakes.

    **Observation:**

    * Output is **more varied, less predictable, sometimes more imaginative**.
    * Good for **creative ideas, brainstorming, or exploring alternative phrasing**.

    ---

    ✅ **Key takeaway:**

    * **Low temperature (0–0.3)** → consistent, precise, factual outputs.
    * **High temperature (0.7–1.0)** → diverse, creative, less constrained outputs.



2. Repeat with different top-p values (e.g., 0.5 vs 1).

    **Prompt:**

    > “Summarize the main AI techniques in 5 bullet points.”

    **Top-p** controls **probability-based token selection**:

    * Low top-p → only the most likely words are considered → **less diverse output**
    * High top-p → more possible words included → **more varied output**

    ---

    ### **1️⃣ Top-p = 0.5** (low probability mass)

    * Restricts generation to the top 50% most likely tokens.

    * Output tends to be **safe, predictable, and concise**:

    * **Machine Learning (ML):** Algorithms that find patterns in data.

    * **Deep Learning (DL):** Neural networks modeling complex data relationships.

    * **Natural Language Processing (NLP):** Systems understanding human language.

    * **Computer Vision:** AI that interprets images and videos.

    * **Reinforcement Learning (RL):** Learning via trial-and-error with rewards.

    **Observation:**

    * Very **deterministic and conventional wording**.
    * Good for **accurate summaries and factual explanations**.

    ---

    ### **2️⃣ Top-p = 1** (full probability mass)

    * Includes all possible tokens → output can be **more diverse and creative**:

    * **Pattern-Learning Systems:** Algorithms spotting trends and patterns in datasets.

    * **Neural Deep Networks:** Complex networks tackling sophisticated tasks.

    * **Language Intelligence Tools:** AI systems reading, writing, or conversing like humans.

    * **Visual Understanding Engines:** Systems analyzing images, video, or visual data.

    * **Trial-and-Error Learners:** Agents improving behavior based on feedback and rewards.

    **Observation:**

    * Output is **less constrained, more imaginative**, slightly more varied in phrasing.
    * Good for **creative explanations, brainstorming, or alternative expressions**.

    ---

    ✅ **Key takeaway on top-p:**

    * **Low top-p (0.5–0.6)** → safe, predictable outputs (like low temperature).
    * **High top-p (0.9–1.0)** → more diverse, flexible outputs, allows creative phrasing.




3. Record how the style, randomness, and focus of responses change.

    Observations

    Temperature effect:

    Low (0.2) → outputs are predictable, factual, focused.

    High (0.9) → outputs are creative, variable in wording, less rigidly structured.

    Top-p effect:

    Low (0.5) → restricts token choices → reduces randomness, keeps responses tight and safe.

    High (1.0) → allows all tokens → increases diversity, sometimes slightly reducing strict focus.

    Combined effect:

    Low temp + low top-p → most reliable, formal, highly focused output.

    High temp + high top-p → most creative, high variance in phrasing, moderate focus.

    Mixed values (low temp + high top-p or high temp + low top-p) → balance between accuracy and creativity.

    ✅ Summary:

    Style → becomes more creative as temp or top-p increase.

    Randomness → rises with higher temp or higher top-p.

    Focus → strongest with low temp and low top-p; loosens as parameters rise.

    | Temp | Top-p | Style                      | Randomness | Focus          | Example Bullet Point                                                   |
| ---- | ----- | -------------------------- | ---------- | -------------- | ---------------------------------------------------------------------- |
| 0.2  | 0.5   | Formal, standard           | Very low   | Very high      | “Machine Learning (ML): Algorithms that find patterns in data.”        |
| 0.2  | 1.0   | Slightly flexible          | Low        | High           | “Machine Learning (ML): Algorithms that learn patterns from data.”     |
| 0.9  | 0.5   | Creative wording           | Medium     | Moderate       | “Pattern-Learning Systems: Algorithms spotting trends in datasets.”    |
| 0.9  | 1.0   | Very creative, imaginative | High       | Moderate/Loose | “Neural Deep Networks: Complex networks tackling sophisticated tasks.” |
