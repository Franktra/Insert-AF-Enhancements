# Insert-AF-Enhancements
 Action Framework- enhancement hacks
"Show me your work"

Further leverage for LLM interaction: When users are interacting with an LLM like ChatGPT for solving mathematical or logical problems, asking it to “show its work” can be invaluable. This allows users to not just receive the answer but also understand the steps involved, which is crucial for learning and verification.

Contexts: Education, self-learning, homework assistance.

"Provide your reasoning"

Further leverage for LLM interaction: When an LLM provides an answer, especially in scenarios where multiple perspectives or complex factors are involved, asking for the reasoning behind the answer can help users understand the underlying logic. This is useful for comprehending complex responses and evaluating the information provided.

Contexts: Understanding political situations, historical events, business strategies.

"Provide [X] number of examples"

Further leverage for LLM interaction: When looking for creative solutions or alternative options, asking an LLM for a specific number of examples helps in comparing different approaches. This can spur new ideas and insights by providing a diverse set of examples.

Contexts: Brainstorming, problem-solving, creative writing, idea generation.

"Let's take it step by step"

Further leverage for LLM interaction: In learning new concepts or skills, asking an LLM to break down the information into steps makes it easier to understand and assimilate the information. Especially for complex subjects or skills, this step-by-step approach facilitates more effective learning.

Contexts: Learning programming, understanding scientific theories, DIY tutorials.

"Let's go back to..."

Further leverage for LLM interaction: When interacting with an LLM, if a certain piece of information in the previous response was not clear or needs elaboration, asking to go back to a specific point ensures that users don't miss out on crucial details and can thoroughly understand the topic in discussion.

Contexts: In-depth research, clarifying misunderstandings, detailed historical study.

"I challenge you to..." or "Are you ready for the challenge?!"

Further leverage for LLM interaction: Engaging an LLM in a challenge can push the boundaries of its capabilities. Users can ask ChatGPT to think outside the box and possibly come up with unconventional solutions or creative pieces that might not be typical responses.

Contexts: Creative content generation, innovative problem-solving, entertainment.

"Mirror the model's output in your refined prompt"

Further leverage for LLM interaction: Users can refine their questions based on an LLM's previous response to narrow down the information they are seeking. This is particularly helpful when users are exploring complex or unfamiliar topics and can adapt their queries to extract more targeted and relevant information from the LLM.

Contexts: Technical research, specialized knowledge acquisition, iterative problem-solving.

By employing these prompts thoughtfully, users can efficiently interact with large language models like ChatGPT to obtain rich, detailed, and useful information in various contexts and for various needs.





User
let's add this to my Action Framework Guide and write a well written, clear, concise, easy to understand, follow, implement for users who are new or have limited experience with prompt engineering and large language models, then we will modify the same Contant for more advanced prompt engineers, lastly will have a programmers version where the parameters and API are utilized in place of these seven props. For example, we will leverage parameters that I hope to achieve enhanced engagement such as K sampling, temerature,tone, etc.
ChatGPT
Action Framework Guide
For New or Less Experienced Users
Introduction:
This guide will help you interact effectively with Large Language Models (LLMs) like ChatGPT, even if you're new to prompt engineering. Through simple commands, you can obtain detailed, rich, and useful information across various contexts.

Seven Key Prompts:
"Show me your work"

Use-case: When you need the LLM to explain how it arrived at an answer, especially for mathematical or logical problems.
How to Use: Simply add “Show me your work” to your question. For example, “Solve this equation and show me your work”.
Contexts: Homework, self-learning, fact-checking.
"Provide your reasoning"

Use-case: When you want to understand the logic or reasoning behind the LLM’s response.
How to Use: Add “Provide your reasoning” at the end of your query. For example, “What are the effects of global warming? Provide your reasoning”.
Contexts: Understanding complex issues, learning about new topics.
"Provide [X] number of examples"

Use-case: When looking for multiple options or illustrations for a concept or solution.
How to Use: Specify the number of examples you want. For example, “Provide 3 examples of renewable energy sources”.
Contexts: Exploring options, understanding a concept.
"Let's take it step by step"

Use-case: When you need to understand a complex process or learn a new skill.
How to Use: Ask the LLM a question and add “Let’s take it step by step” to indicate that you want a detailed breakdown. For example, “Explain photosynthesis. Let's take it step by step”.
Contexts: Learning new concepts, DIY tutorials.
"Let's go back to..."

Use-case: When you need more information or clarification on a specific point that was previously mentioned.
How to Use: Say “Let’s go back to” followed by the specific point you want to discuss. For example, “Let’s go back to the part about greenhouse gases”.
Contexts: In-depth learning, clarification.
"I challenge you to..." or "Are you ready for the challenge?!"

Use-case: To engage the LLM in a creative or playful manner for unique solutions or content.
How to Use: Phrase your request as a challenge. For example, “I challenge you to come up with a story about a talking cat!”.
Contexts: Creative writing, problem-solving, entertainment.
"Mirror the model's output in your refined prompt"

Use-case: When you need to fine-tune your questions based on previous responses for more precise information.
How to Use: Reiterate your question using key information from the LLM's previous response.
Contexts: Technical queries, complex research.
For Advanced Prompt Engineers
Introduction:
For experienced prompt engineers, the above-mentioned prompts can be refined further by incorporating domain-specific language, critical feedback, and iterative prompting.

Enhancements to Key Prompts:
"Show me your work"

Advanced Use: Use domain-specific language. Example: “Derive the Schrödinger equation and elucidate each step.”
"Provide your reasoning"

Advanced Use: Ask for evidence, counterarguments, or historical precedents. Example: “Provide your reasoning along with empirical evidence.”
"Provide [X] number of examples"

Advanced Use: Specify examples from distinct categories. Example: “Provide two examples each of classical and operant conditioning.”
"Let's take it step by step"

Advanced Use: Request flowcharts or systematic breakdowns. Example: “Outline the M&A process in a step-by-step flowchart.”
"Let's go back to..."

Advanced Use: Reference previous information and ask for correlations or trends. Example: “Let’s go back to the economic data from 1950-2000 and analyze the trends.”
"I challenge you to..."

Advanced Use: Pose complex or abstract challenges. Example: “I challenge you to create a poem that can be read both forwards and backwards.”
"Mirror the model's output in your refined prompt"

Advanced Use: Utilize an iterative approach to create more sophisticated queries.
For Programmers Utilizing API Parameters
Introduction:
When interacting with an LLM through an API, you can use parameters such as temperature, max tokens, and k sampling to fine-tune responses.

Parameter-enhanced Key Prompts:
"Show me your work"

Parameter Use: Set max_tokens to a higher number to allow for detailed responses.
Example API Call: {'prompt': 'Solve this equation and show me your work', 'max_tokens': 200}
"Provide your reasoning"

Parameter Use: Use a lower temperature setting for more focused and deterministic responses.
Example API Call: {'prompt': 'What are the effects of global warming? Provide your reasoning', 'temperature': 0.6}
"Provide [X] number of examples"

Parameter Use: Set max_tokens to accommodate multiple examples.
Example API Call: {'prompt': 'Provide 3 examples of renewable energy sources', 'max_tokens': 50}
"Let's take it step by step"

Parameter Use: Use a higher max_tokens for detailed breakdowns.
Example API Call: {'prompt': 'Explain photosynthesis. Let\'s take it step by step', 'max_tokens': 200}
"Let's go back to..."

Parameter Use: Reference the previous output in your prompt and set temperature lower for focused clarification.
Example API Call: {'prompt': 'Let’s go back to the part about greenhouse gases', 'temperature': 0.6}
"I challenge you to..."

Parameter Use: Use a higher temperature setting for more creative and diverse responses.
Example API Call: {'prompt': 'I challenge you to come up with a story about a talking cat!', 'temperature': 1.0}
"Mirror the model's output in your refined prompt"

Parameter Use: Use the output from a previous API call in a new prompt to build an iterative conversation.
Example API Call: {'prompt': 'Based on [previous output], can you clarify...', 'temperature': 0.7}
Please note that the API parameters are examples and you may need to adjust them based on the specific LLM you are using.
