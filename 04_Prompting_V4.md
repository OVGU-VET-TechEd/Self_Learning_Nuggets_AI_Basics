
04_AI_Prompting.md
<!-- author: AI in TVET Workshop Team version: 1.0.0 language: en narrator: US English Female comment: AI Prompting Strategies for TVET Teachers (AI-Assisted Teaching Competency) link: https://raw.githubusercontent.com/OVGU-VET-TechEd/ASSET_UNESCO_Coinitiative/refs/heads/main/ASSET_basic.css @style .sector-card { background: linear-gradient(135deg, #667eea 0%, #764ba2 100%); color: white; padding: 2rem; margin: 1rem; border-radius: 15px; box-shadow: 0 8px 32px rgba(0,0,0,0.3); transition: transform 0.3s ease; } .sector-card:hover { transform: translateY(-5px); } .ai-tool-demo { background: #f8f9fa; border: 2px solid #007bff; border-radius: 10px; padding: 1.5rem; margin: 1rem 0; } .quiz-interactive { background: linear-gradient(45deg, #ff6b6b, #ffa726); color: white; padding: 1rem; border-radius: 10px; margin: 1rem 0; } .resource-link { background: #28a745; color: white; padding: 0.5rem 1rem; border-radius: 5px; text-decoration: none; display: inline-block; margin: 0.25rem; transition: all 0.3s ease; } .resource-link:hover { background: #218838; transform: scale(1.05); } @end @customQuiz [[.]] <script> "@0" == btoa( "@input".trim().toLowerCase() ) </script> @end @aiDemo: <div class="ai-tool-demo">**AI Demo:** @0<br>**Tool:** @1<br>**Try it:** [Click here](@2)</div> @sectorCard: <div class="sector-card">**@0**<br>@1</div> @resourceLink: <a href="@1" class="resource-link" target="_blank">@0</a> -->
AI Prompting: Getting the Best from AI (AI-Assisted Teaching)
<div style="text-align:center;"> <img src="https://github.com/OVGU-VET-TechEd/ASSET_UNESCO_Coinitiative/blob/main/media/UNESCO-UNEVOC_logo.png?raw=true" alt="UNEVOC Logo" width="80" style="margin:0 10px;"/> <img src="https://github.com/OVGU-VET-TechEd/ASSET_UNESCO_Coinitiative/blob/main/media/ASSET_icon.png?raw=true" alt="ASSET Logo" width="80" style="margin:0 10px;"/> <img src="https://github.com/OVGU-VET-TechEd/ASSET_UNESCO_Coinitiative/blob/main/media/hrdc_logo.png?raw=true" alt="HRDC Logo" width="80" style="margin:0 10px;"/> <img src="https://github.com/OVGU-VET-TechEd/ASSET_UNESCO_Coinitiative/blob/main/media/mitd_logo.png?raw=true" alt="MITD Logo" width="80" style="margin:0 10px;"/> <img src="https://github.com/OVGU-VET-TechEd/ASSET_UNESCO_Coinitiative/blob/main/media/HWK_Blume.png?raw=true" alt="HWK Blume Logo" width="80" style="margin:0 10px;"/> </div>
Introduction
Now that we have the tools at our disposal, the next step in AI-assisted teaching is mastering the skill of prompting. Think of prompting as the art of asking the AI for exactly what you need, in a way that yields useful responses. Just like posing questions to students effectively is a teaching skill, posing questions/commands to AI is a key digital skill. This module will cover what prompts are, how to structure them, and introduce strategies like the 5-step prompting method, using decision trees in prompts, and even constructing “mega prompts” for complex tasks. We will continue following Rani’s journey – seeing how she uses prompts for administrative tasks and to engage her students. By the end, you should be able to craft better prompts that get better results, saving you time and enhancing the quality of AI outputs in your teaching practice.
What is a Prompt?
A prompt is any input you give to an AI system to elicit a response. It could be a question, a task description, or a set of instructions. In simple terms, prompting is how you “communicate” with AI. For example, typing “Explain the law of reflection in simple terms” into ChatGPT is a prompt. But prompting can be more involved: you might provide context, specify a format, or break a request into steps. A well-crafted prompt can dramatically improve the relevance and accuracy of the AI’s response. In a way, learning to prompt is like learning to ask better questions and give clearer directions.
A prompt can also be iterative – you refine it based on the AI’s previous answer (this is like a conversation). Prompting isn’t one-size-fits-all; it’s an interactive process. If the AI doesn’t give what you want, you can tweak the prompt and try again. For instance, if Rani asks, “Give me questions for my electronics quiz” and gets too-hard questions, she can refine prompt: “Give me simple, basic-level questions on electronics suitable for beginners.”
Anatomy of a Good Prompt
A well-structured prompt often contains these elements:
Task: What do you want the AI to do? (e.g., “Create a quiz question,” “Summarize this text,” “Act as a student and ask a question about …”).
Context: Any background info that might help. (e.g., “My students are 16-year-old electronics majors,” or “We just covered topic X in class.”)
Format or Style: If you need the answer in a certain format. (e.g., “Answer in a bulleted list,” “Provide the answer and a short explanation,” “Use a friendly tone.”)
Constraints (if any): Any specific limitations. (e.g., “Use at most 3 sentences,” “Don’t use technical jargon,” “Include one real-world example.”)
Examples (optional): Sometimes giving an example of what you want can guide the AI. (e.g., “For example, if asked about Y, an answer could be… Now answer about Z similarly.”)
Not every prompt needs all of these, but thinking in these terms helps. For complex tasks, you might include all. For a simple fact query, just the task is enough (“What’s the formula for…?”).
Consider Rani wants the AI to write a word problem for her electronics class:
A bad prompt might be: “Give me a word problem about electronics.” This is vague – the AI might not know what level or what concept. The result could be unsatisfactory (too hard, too easy, or off-topic).
A good prompt: “You are a teacher creating a word problem for a Basic Electronics class. The topic is Ohm’s Law (V = I×R). The problem should involve a real-life scenario (like using a battery, a resistor, etc.). It should ask students to find one of the values (voltage, current, or resistance) given the other two. Format it as a short story. Then provide the solution with the formula step clearly shown.”
Notice how this good prompt: assigns a role (“You are a teacher…” which helps set the context/tone), specifies the content (Ohm’s Law scenario), format (short story style), and what output parts are needed (problem + solution). The chances of getting a useful result are much higher now.
Prompting Strategies
There are various techniques to get better outputs. Let’s discuss a few:
The 5-Step Prompting Framework (Google’s method)
Google suggests a clear framework for crafting prompts, especially for complex tasks:
Task – State what you want the AI to do as clearly as possible.
Context – Provide background or additional info that can guide the AI.
References – If applicable, include any references or data (like giving a paragraph and saying “continue this”).
Evaluate – Tell the AI how to judge a good result, if needed (e.g., “The answer should be correct and use proper units”).
Iterate – Not exactly in the single prompt, but the notion that you refine and repeat as needed.
For example, if Rani wants an AI to draft a rubric:
Task: “Draft a rubric for a practical electronics project.”
Context: “The project is building a small AM radio; students are vocational high schoolers.”
References: (If she had an example rubric, she might include it or parts of it as a guide.)
Evaluate: “The rubric should have clear criteria across 3 levels: Excellent, Satisfactory, Needs Improvement.”
Iterate: After the first output, she reviews and says, “Iterate: Now make sure each criterion is phrased in student-friendly language.”
By structuring her prompt this way, she hits all necessary info. The AI likely returns a decent rubric, maybe needing minor tweaks.
Decision Tree / Chain-of-Thought Prompting
Sometimes it helps to have the AI break down its reasoning step by step (especially for problem-solving or complex decisions). You can prompt the AI to follow a logical chain or to consider a decision tree.
For example, Rani wants help figuring out how to improve a student’s study habits using AI suggestions. She might prompt: “Let’s think step-by-step. A student is struggling with understanding circuit theory. Step 1: Identify possible reasons for the difficulty. Step 2: For each reason, suggest a strategy to help. Step 3: Provide a final recommended plan combining the best strategies. Now proceed through the steps.”
Here she’s basically giving the AI a decision process. The AI would then output something like:
“Step 1: Possible reasons – (a) foundational math gaps, (b) not enough hands-on practice, (c) difficulty with technical language.
Step 2: Strategies – for (a) review basic algebra with the student; for (b) incorporate simple circuit building exercises; for (c) use analogies and clarify jargon…
Step 3: Plan – The student should spend 1 week on algebra refresh, then do a guided hands-on activity each lesson, and we’ll create a glossary of key terms together.”
This chain-of-thought approach often yields thorough answers because the AI is guided to not skip steps. It also makes the reasoning transparent, which is useful if Rani wants to see the “why” behind suggestions.
Another angle of decision tree prompting: asking the AI to present options and then refine one. E.g., “Give me two different approaches to teaching soldering: one very structured, one very exploratory. Then explain the pros and cons of each.” This kind of prompt yields a comparative answer – effectively the AI is following a mental branching of approaches and evaluating them.
Step-by-Step and “Let’s think step by step” Technique
A known strategy with complex models is explicitly telling them “Let’s think step by step” for complex questions. This tends to make them break down the solution logic, often leading to more accurate results (especially for math or logical reasoning problems).
If Rani were using AI to check a solution: “A student’s circuit has 3 resistors… [problem data]. Let’s solve this step by step:” – the AI will list each step (calc total resistance, then current, etc.) instead of jumping to an answer, which helps catch mistakes.
Mega Prompts – What are they?
A mega prompt is essentially a very detailed, comprehensive prompt (or series of prompts) that tries to account for many aspects of a task. It’s like giving the AI a full project brief. Mega prompts might combine context, multiple instructions, format specs, and even role-play elements in one go.
For instance, say Rani wants the AI to generate an entire lesson plan. A mega prompt might look like:
“You are an experienced electronics instructor assistant. Task: Help me create a 45-minute lesson plan on the topic of renewable energy in electronics (focusing on solar panels and their electrical characteristics). Context: Students are 2nd-year vocational students, familiar with basic circuits. Include: 1) Learning objectives at the start. 2) A brief introduction (with an interesting fact or question to grab attention). 3) Two hands-on activities (with required materials listed). 4) One group discussion prompt. 5) A short quiz (3 questions) at the end. Format: Provide the plan in outline form with clear headings for each section. Tone: Teacher-friendly, clear, and encouraging active learning. Additional Info: One activity should involve actual measurement (maybe using a multimeter on a small solar panel). Check: Ensure the content is accurate and safety is addressed where relevant.”
This mega prompt leaves little to guesswork. The AI likely will produce a structured lesson plan meeting those criteria. Rani might still tweak it, but most of the heavy lifting is done. The advantage of a mega prompt is efficiency – one prompt, one fairly complete output. The disadvantage is if something is off, the whole output may need revising or re-generation. Sometimes, splitting tasks (like first asking for objectives, then activities, etc.) can allow more control, but it takes more iterations. Mega prompts shine when you know exactly what you want and can describe it fully.
However, if Rani noticed the lesson plan from the mega prompt missed something, she could either prompt again adding that detail or just edit manually. Mega prompting is a great skill once you’re comfortable because you can practically get draft lesson plans, project outlines, or reports in one shot. It’s like being a very specific supervisor to the AI.
Examples: Prompting for Teaching and Administration
Let’s see some concrete prompt and response pairs to illustrate good prompting in Rani’s world:
Use Case 1: Administrative Task (Email Draft)
Prompt: “You are my teaching assistant. Write a polite, concise email to parents informing them about an upcoming field trip to an electronics manufacturing plant. Include the date (Oct 15, 2025), what students should bring (packed lunch, ID), and a reassurance about safety measures in place.”
Expected AI Behavior: It will generate a clear email. Because the prompt is specific, it should include all points (date, what to bring, safety). Rani will then just adjust any details (like adding the exact plant name or changing tone slightly if needed). Without those specifics, the AI might have written a very generic email missing one of these details.
Use Case 2: Student Engagement (Role-play prompt)
Rani wants the AI to create a scenario for students: e.g., a conversation with an AI tutor.
Prompt: “Act as a curious student learning about microcontrollers, and ask me (the teacher) three questions in simple language about how microcontrollers work or how to get started programming them. After each question, wait for my answer.”
Expected AI Behavior: The AI will output something like Student: “What exactly does a microcontroller do in a device?” (and then maybe some system like waiting for answer), then second question, etc. This can give Rani insight into common questions or she could even show this to the class to discuss answering them. The structured prompt led the AI to produce content in a specific format (3 separate questions).
Use Case 3: Prompting for a Mega Prompt Example
We gave an example above for a mega prompt for a lesson plan. Let’s see another quick mega prompt:
Prompt: “Create a mega prompt for generating a troubleshooting guide. The guide is for identifying and fixing common problems in a basic electronics lab (e.g. circuit not powering, component overheating, etc.). The mega prompt should instruct the AI assistant to provide a structured guide with cause->solution format, include at least 5 common problems, and an introduction and conclusion.”
(Notice this is meta – asking AI to help create a mega prompt. Actually, this is a trick: you can ask AI to help you write better prompts! It’s a valid strategy if you explain what you need. The AI might output a possible mega prompt which you can then use on itself or another run. Essentially, AI can assist in prompt engineering itself – a reflective use.)
Rani’s Classroom Prompt Use Example
Rani also involves prompting in student activities. For instance, she might have students practice crafting prompts as part of digital skills. One exercise: She shows them a mediocre AI output (like a flashcard list on soldering that’s incomplete) and shares the original prompt. Then challenges students: “How can we prompt it better to get more complete flashcards?” Students suggest adding specifics. This not only improves the output but teaches them how to interact with AI critically – a great skill aligned with human agency and AI literacy.
@sectorCard("Student Engagement with Prompting","Rani turned prompting into a learning activity. She presented a wrong answer ChatGPT gave to a physics question (due to a vague prompt). She then asked her class: “How do you think I asked the question to get this answer? How could I ask it better?”<br><br>Her students discussed and realized the original prompt might have been too broad. They suggested adding details and steps. Together they formulated a new prompt, fed it to the AI, and got a correct and clear explanation. The class cheered – they had “taught” the AI by asking the right question! Rani used this moment to highlight that in real life and AI: asking good questions is key to getting good answers. This exercise not only clarified the physics concept but also empowered students with a bit of AI know-how.")
Quizzes and Reflection on Prompting
Now let’s test and reinforce your understanding of prompting strategies:
You want ChatGPT to create a step-by-step solution for a calculation problem (like calculating total resistance in a circuit). What is a useful phrase to include in your prompt?
[[X]] “Let’s think step by step” to encourage the AI to show each step clearly.
[[ ]] “Give me the answer immediately” (this likely yields just the answer without explanation).
[[X]] “Provide the solution in a clear sequence of steps” – being explicit about format helps.
[[ ]] No special phrasing, just the question (which might result in a direct answer with no steps).
Which prompt is better for getting an AI to draft a student project guideline?
A. “Write a project guide for electronics.”
B. “You are an instructor. Write a step-by-step project guideline for building a simple FM radio. Include: objectives, required materials, construction steps, and testing procedure. Write it as a numbered list with short, clear sentences.”
[[ ]] A is better
[[X]] B is better (it’s specific about context, content, and format)
[[ ]] They will yield the same quality
True or False: A mega prompt includes multiple pieces of information (like context, format, examples) to guide the AI in detail.
[[X]] True
[[ ]] False
Rani wants the AI to role-play as a student to generate questions. Which is a good way to start that prompt?
[[X]] “Act as a beginner student in electronics and ask me three questions about how transistors work…”
[[ ]] “Imagine someone asks questions.” (too vague about who and what)
[[X]] “Role: a curious teen learner. Task: ask questions about transistors…”
[[ ]] “Make questions.” (not specifying context or role will yield generic results)
Consider the 5-step prompting method. Which component is illustrated in this instruction to the AI: “The answer should be formatted as a table with two columns” ?
[[ ]] Task
[[ ]] Context
[[ ]] References
[[ ]] Iterate
[[X]] Format/structure requirement (which falls under how to evaluate/produce the output format)
Reflection (open-ended): Rani tried prompting an AI to create a “decision tree for choosing a career path” for her guidance class, but the result was confusing. She’s not sure if the prompt was the issue. What could she do to improve it? Think of at least two prompt adjustments or strategies based on this module’s ideas.
Hint: Perhaps break the task down, specify format (maybe ask for a bullet list of questions leading to career suggestions), or provide more context about the students, etc. This question is for you to ponder and perhaps write down your thoughts or discuss with a peer.
Your thoughts: [[___]]
Feel free to re-prompt yourself by reviewing the prompting tips above! Prompting is iterative even for us humans learning it.
By now, you’ve gained insight into how to communicate your needs to AI effectively. Prompting is truly an exercise in clarity of thought – something teachers practice daily when explaining to students, now applied to AI. In the final module, we will turn to ensuring quality and ethics in our AI usage, rounding out the framework with the all-important principles that should guide all these technical explorations. Keep your curiosity and critical eye sharp as we move forward.
<div style="text-align:center;"> <img src="https://github.com/OVGU-VET-TechEd/ASSET_UNESCO_Coinitiative/blob/main/media/UNESCO-UNEVOC_logo.png?raw=true" alt="UNEVOC Logo" width="80" style="margin:0 10px;"/> <img src="https://github.com/OVGU-VET-TechEd/ASSET_UNESCO_Coinitiative/blob/main/media/ASSET_icon.png?raw=true" alt="ASSET Logo" width="80" style="margin:0 10px;"/> <img src="https://github.com/OVGU-VET-TechEd/ASSET_UNESCO_Coinitiative/blob/main/media/hrdc_logo.png?raw=true" alt="HRDC Logo" width="80" style="margin:0 10px;"/> <img src="https://github.com/OVGU-VET-TechEd/ASSET_UNESCO_Coinitiative/blob/main/media/mitd_logo.png?raw=true" alt="MITD Logo" width="80" style="margin:0 10px;"/> <img src="https://github.com/OVGU-VET-TechEd/ASSET_UNESCO_Coinitiative/blob/main/media/HWK_Blume.png?raw=true" alt="HWK Blume Logo" width="80" style="margin:0 10px;"/> </div>
