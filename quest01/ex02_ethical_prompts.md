Part A: Independent Analysis
https://saicharankummetha.medium.com/few-examples-of-bad-prompts-and-how-to-improve-them-e717a1087735

https://blog.agent.ai/how-to-identify-and-fix-a-bad-prompt

1. Write three poorly designed prompts that might lead to biased/unsafe answers.
    I) Tell me about animals.
    II) Write a about Django framework
    III)Write a summary of this journal.

2.  For each, note:

    Why it's problematic

    Potential harm

    Hidden assumptions


    I) Tell me about animals.
    Why it's problematic: The question is too generic, broad, no goal or scope. 

    Potential harm: Too long output and absence of desired output

    Hidden assumptions: The model doesn’t know what aspect of animals you want — reptile, mammal, fishes, birds, insects.

    II) Write a about Django framework
    Why it's problematic: No role or perspective specified 

    Potential harm: Generic tone of output  

    Hidden assumptions: The model doesn’t know from which perspective your output should to be.

    III)Write a summary of this journal.
    Why it's problematic: No formate or structure specified

    Potential harm: Gives output in an unstructure and disorganized formate. 

    Hidden assumptions: The model doesn't know hoe to structure or order your work.

3. Rewrite each prompt to be clearer, fairer, and safer.

    I)Tell me about dogs from Germany with mixed colours and height for guarding home and lives in 250 words.

    II) As an expert backend python developers with many years of experiences. Write a summary of Django framework in creating a blog.

    III) Summarize the following journals into 3 bullet points under the headings: Problem, Solution, and Outcome.”

4. Explain your improvements.
    I)Tell me about dogs from Germany with mixed colours and height for guarding home and lives in 250 words.
    This adds clarity (place and features), context(guarding), and constraint (word limit).

    II) As an expert backend python developers with many years of experiences. Write a summary of Django framework in creating a blog.
    Setting a persona guides tone, depth, and style — producing a more aligned response.

    III) Summarize the following journals into 3 bullet points under the headings: Problem, Solution, and Outcome.”
    A structured output reduces ambiguity, improves readability, and simplifies downstream automation.


Part B: Test and Validate

5. Test original vs. improved prompts with an LLM.

6. Compare outputs: Did your changes work? What surprised you?
    I) My work changed dramatically from the original Test.The original test output was generic, broad and lengthy telling me about all catergories of animals 
     but improved prompt output was specific tailoring on a dog from Germany with mixed colours and height in brief wortds of 250.

    II) My work changed completely from the original Test. The improved prompt output sounded in a persona guide tone, and depth aligning to the desired output
    in few words of 250 but the Test original output sound as a ramdom testbook with long things to read and understand.

    III) The improved prompt was brief, organized, well ordered and much readable but the test original out put was not ordered and structured, and less readable.


7. "Original: [...] Improved: [...] My reasoning: [...] What ethical issues might I have missed? How could this still go wrong?"

    I) Your improved prompt is clearer, but you may have missed ethical risks like promoting aggressive dog use, reinforcing breed stereotypes, ignoring animal welfare needs, and giving advice that may not fit legal or living conditions.

    It could still go wrong if someone chooses a dog only for guarding without proper training, care, or understanding of temperament, which can harm both the animal and people.

    A more ethical approach is to include responsibility, training, and welfare — not just protection features — so the information stays safe, balanced, and realistic.

    I could refine it like this:

    “Tell me about German dog breeds with mixed coat colours that are suitable for home protection. Include information about temperament, training needs, and responsible ownership in about 250 words.”


    II) Using an “expert” persona can create a false sense of authority, encourage over-trust in the response, and risk authenticity or plagiarism issues if published as your own expertise. It could also include outdated or inaccurate technical details. Always verify, adapt, and ensure the work reflects your real understanding.

    You could refine the prompt like this:

    “Write a technically accurate summary of Django for building a blog. Include architecture, security features, and best practices. I will review and adapt it.”

    This:

    Removes false authority framing

    Encourages verification

    Keeps responsibility with you

    III) Structured prompts improve clarity and automation, but they risk oversimplifying research, misrepresenting findings, omitting limitations, and producing misleading summaries if the original nuance is compressed or not carefully verified.

    I could refine it to:

    “Summarize the journal into bullet points under Problem, Method, Key Findings, Limitations, and Outcome. Do not add information not explicitly stated.”

    This:

    Preserves nuance

    Reduces hallucination

    Improves academic integrity

    Keeps structure without distortion


Part C: Reflection

    - If you'd asked AI to "write ethical prompts" from the start, would you understand why they're ethical?

    Yes, I will understand why they are ethical.

    - Can you now design ethical prompts without AI?

    Yes, I can design a design ethical prompts without AI.