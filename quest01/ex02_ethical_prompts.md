Part A: Independent Analysis
https://saicharankummetha.medium.com/few-examples-of-bad-prompts-and-how-to-improve-them-e717a1087735

https://blog.agent.ai/how-to-identify-and-fix-a-bad-prompt

1. Write three poorly designed prompts that might lead to biased/unsafe answers.
    I) Tell me about animals.
    II) Write a about Django framework
    III)Write a summary of this journal on kids.

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

    III)Write a summary of this journal on kids.
    Why it's problematic: No formate or structure specified

    Potential harm: Gives output in an unstructure and disorganized formate. 

    Hidden assumptions: The model doesn't know hoe to structure or order your work.

3. Rewrite each prompt to be clearer, fairer, and safer.

    I)Tell me about dogs from Germany with mixed colours and height for guarding home and lives in 250 words.

    II) As an expert backend python developers with many years of experiences. Write a summary of Django framework in creating a blog.

    III) Summarize this journal on kids into 3 bullet points under the headings: Problem, Solution, and Outcome.”

4. Explain your improvements.
    I)Tell me about dogs from Germany with mixed colours and height for guarding home and lives in 250 words.
    This adds clarity (place and features), context(guarding), and constraint (word limit).

    II) As an expert backend python developers with many years of experiences. Write a summary of Django framework in creating a blog.
    Setting a persona guides tone, depth, and style — producing a more aligned response.

    III) Summarize this journal on kids into 3 bullet points under the headings: Problem, Solution, and Outcome.”
    A structured output reduces ambiguity, improves readability, and simplifies downstream automation.


Part B: Test and Validate

5. Test original vs. improved prompts with an LLM.

 I)Test Original: Tell me about animals

 Output: Animals are living organisms that belong to the biological kingdom **Animalia**. They are multicellular, consume organic material (they are heterotrophs), can usually move independently, and respond to their environment.

Let’s break it down clearly:

---

## 1. What Makes an Animal an Animal?

Animals generally:

* Are made of many cells (multicellular)
* Do not make their own food (unlike plants)
* Obtain energy by eating other organisms
* Can move at some stage of life
* Have specialized tissues (like nerves and muscles)

---

## 2. Major Groups of Animals

Animals are divided into two large categories:

### A. Invertebrates (No Backbone)

These make up about **95% of all animal species**.

Examples:

* Insects (ants, butterflies)
* Spiders
* Worms
* Jellyfish
* Octopuses

They tend to be smaller and often have exoskeletons or soft bodies.

---

### B. Vertebrates (Have a Backbone)

These animals have a spinal column.

Main groups include:

* Fish
* Amphibians (frogs, salamanders)
* Reptiles (snakes, lizards)
* Birds
* Mammals

Humans are mammals.

---

## 3. Mammals (Since You’re in Nigeria, You’ll Recognize Many)

Mammals:

* Have hair or fur
* Are warm-blooded
* Produce milk for their young

Examples found in Africa include:

* African elephant
* Lion
* Cheetah

---

## 4. Birds

Birds:

* Have feathers
* Lay eggs
* Are warm-blooded
* Most can fly

Example:

* Ostrich (the largest bird, found in Africa)

---

## 5. Why Animals Are Important

Animals:

* Maintain ecological balance
* Help pollinate plants
* Control pest populations
* Provide food and materials for humans
* Contribute to biodiversity

Predators like the Lion help regulate herbivore populations, keeping ecosystems stable.

---

## 6. Intelligence in Animals

Some animals show remarkable intelligence:

* Dolphins use complex communication
* Elephants show memory and emotional behavior
* Crows use tools

---

## 7. Fun Fact

The largest animal ever known is the Blue whale — even larger than dinosaurs.


Improved version:Tell me about dogs from Germany with mixed colours and height for guarding home and lives in 250 words.

Output: One of the most well-known dogs from Germany that has mixed colours, medium-to-tall height, and excellent guarding ability is the German Shepherd. This breed originated in Germany in the late 19th century and was developed specifically for intelligence, strength, and protection work. German Shepherds usually have mixed coat colours such as black and tan, sable (brown and black mix), black and silver, or even solid black, which gives them a striking and alert appearance.

In terms of height, adult German Shepherds are considered large dogs. Males typically stand about 24–26 inches (60–65 cm) tall at the shoulder, while females are slightly shorter at around 22–24 inches (55–60 cm). Their strong build, upright ears, and confident posture make them naturally intimidating to intruders, which is why they are widely used for home security and protection roles.

German Shepherds are highly intelligent and loyal, making them excellent guard dogs for homes and families. They are naturally protective and can quickly detect unusual movements or threats. However, they are not aggressive by default; with proper training and socialization, they become calm, disciplined, and reliable protectors.

Another important trait is their strong sense of duty. They are often used by police and security services because they can be trained to follow commands, patrol areas, and respond to danger effectively. They also form deep bonds with their owners, meaning they guard not only property but also the lives of the people they love. Overall, their mixed coat colours, tall stature, intelligence, and loyalty make them one of the best German breeds for home guarding.


III) Test Original: Write a summary of a journal on kids.

Output: ### Sample Journal Summary on Kids (Child Development)

This journal focuses on the growth and development of children, emphasizing how early childhood experiences shape cognitive, emotional, and social outcomes. It explains that children learn rapidly through interaction with their environment, caregivers, and peers, making early education and supportive parenting crucial for healthy development.

The journal highlights key developmental stages, noting that physical growth, language acquisition, and problem-solving skills evolve progressively as children mature. It also discusses the importance of play, stating that play-based learning enhances creativity, social skills, and emotional regulation. Additionally, the journal stresses the role of nutrition, healthcare, and a safe environment in promoting overall well-being.

Another major point in the journal is the impact of family and school on a child’s behavior and academic performance. Positive reinforcement, effective communication, and structured learning environments are identified as factors that improve children’s confidence and learning abilities. The journal also addresses challenges such as behavioral issues, learning difficulties, and the effects of technology on children’s attention span and social interaction.

In conclusion, the journal argues that a holistic approach involving parents, educators, and society is essential for raising well-rounded children. Supporting children’s emotional, physical, and intellectual needs during early years lays a strong foundation for their future success and personal development.


Improved version: Summarize this journal on kids into 3 bullet points under the headings: Problem, Solution, and Outcome.”

Output:
* **Problem:** Children’s development can be negatively affected by poor early experiences, inadequate learning environments, limited parental support, and challenges such as behavioral issues, learning difficulties, and excessive technology use.
* **Solution:** Provide supportive parenting, quality early education, play-based learning, proper nutrition, healthcare, and structured school environments that encourage communication, creativity, and emotional growth.
* **Outcome:** Children develop stronger cognitive, social, and emotional skills, leading to better academic performance, improved well-being, and a solid foundation for future success.




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