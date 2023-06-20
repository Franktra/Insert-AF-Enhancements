# Action Framework Guide

## Table of Contents
1. [For Beginners](#for-new-or-less-experienced-users)
2. [For Advanced Prompt Engineers](#for-advanced-prompt-engineers)
3. [For Engineers and Software Developers](#for-engineers-and-software-developers)


## For Beginners <a name="for-new-or-less-experienced-users"></a>

### Introduction:
This guide will help you interact effectively with Large Language Models (LLMs) like ChatGPT, even if you're new to prompt engineering. Through simple commands, you can obtain detailed, rich, and useful information across various contexts.

### Seven Key Prompts:

#### "Show me your work"
- **Use-case**: When you need the LLM to explain how it arrived at an answer, especially for mathematical or logical problems.
- **How to Use**: Simply add “Show me your work” to your question. For example, “Solve this equation and show me your work”.
- **Contexts**: Homework, self-learning, fact-checking.

#### "Provide your reasoning"
- **Use-case**: When you want to understand the logic or reasoning behind the LLM’s response.
- **How to Use**: Add “Provide your reasoning” at the end of your query. For example, “What are the effects of global warming? Provide your reasoning”.
- **Contexts**: Understanding complex issues, learning about new topics.

#### "Provide [X] number of examples"
- **Use-case**: When looking for multiple options or illustrations for a concept or solution.
- **How to Use**: Specify the number of examples you want. For example, “Provide 3 examples of renewable energy sources”.
- **Contexts**: Exploring options, understanding a concept.

#### "Let's take it step by step"
- **Use-case**: When you need to understand a complex process or learn a new skill.
- **How to Use**: Ask the LLM a question and add “Let’s take it step by step” to indicate that you want a detailed breakdown. For example, “Explain photosynthesis. Let's take it step by step”.
- **Contexts**: Learning new concepts, DIY tutorials.

#### "Let's go back to..."
- **Use-case**: When you need more information or clarification on a specific point that was previously mentioned.
- **How to Use**: Say “Let’s go back to” followed by the specific point you want to discuss. For example, “Let’s go back to the part about greenhouse gases”.
- **Contexts**: In-depth learning, clarification.

#### "I challenge you to..." or "Are you ready for the challenge?!"
- **Use-case**: To engage the LLM in a creative or playful manner for unique solutions or content.
- **How to Use**: Phrase your request as a challenge. For example, “I challenge you to come up with a story about a talking cat!”.
- **Contexts**: Creative writing, problem-solving, entertainment.

#### "Mirror the model's output in your refined prompt"
- **Use-case**: When you need to fine-tune your questions based on previous responses for more precise information.
- **How to Use**: Reiterate your question using key information from the LLM's previous response.
- **Contexts**: Technical queries, complex research.

## For Advanced Prompt Engineers <a name="for-advanced-prompt-engineers"></a>

### Introduction:
For experienced prompt engineers, the above-mentioned prompts can be refined further by incorporating domain-specific language, critical feedback, and iterative prompting.

### Enhancements to Key Prompts:

#### "Show me your work"
- **Advanced Use**: Use domain-specific language. Example: “Derive the Schrödinger equation and elucidate each step.”

#### "Provide your reasoning"
- **Advanced Use**: Ask for evidence, counterarguments, or historical precedents. Example: “Provide your reasoning along with empirical evidence.”

#### "Provide [X] number of examples"
- **Advanced Use**: Specify examples from distinct categories. Example: “Provide two examples each of classical and operant conditioning.”

#### "Let's take it step by step"
- **Advanced Use**: Request flowcharts or systematic breakdowns. Example: “Outline the M&A process in a step-by-step flowchart.”

#### "Let's go back to..."
- **Advanced Use**: Reference previous information and ask for correlations or trends. Example: “Let’s go back to the economic data from 1950-2000 and analyze the trends.”

#### "I challenge you to..."
- **Advanced Use**: Pose complex or abstract challenges. Example: “I challenge you to create a poem that can be read both forwards and backwards.”

#### "Mirror the model's output in your refined prompt"
- **Advanced Use**: Utilize an iterative approach to create more sophisticated queries.

# Content for Advanced Prompt Engineers
advanced_content = 
## For Advanced Prompt Engineers <a name="for-advanced-prompt-engineers"></a>

### Introduction:
Advanced users can push the boundaries by using more refined prompts that get the model to think in steps, reason through problems, and even be creative.

### Key Prompts:

1. **"Show me your work"**
    - **Advanced Use:** Ask the LLM to solve complex equations and provide logical precedents.
    - **Example:** “Provide your reasoning along with empirical evidence.”

... (include all the advanced content here) ...


# Content for Programmers
programmers_content = """
## For Engineers and Software Developers <a name="for-engineers-and-software-developers"></a>

### Introduction:
This section focuses on how experienced engineers and software developers can interact programmatically with LLMs such as ChatGPT via API, utilizing parameters for fine-tuning and extracting detailed responses.

### Prerequisites:
- Familiarity with Python programming language
- Access to ChatGPT or similar LLM API
- Installation of necessary Python libraries

# Action Framework Guide


## For Programmers <a name="for-programmers"></a>

### Introduction:
For programmers who want to interact with Large Language Models like ChatGPT programmatically, using APIs and setting parameters to refine and control the model's responses.

### Example Code Snippets:


#### Setting Parameters for API calls


```python
import openai

openai.Completion.create(
    engine="davinci-codex",
    prompt="Explain the concept of machine learning.",
    max_tokens=100,
    n=1,
    stop=None,
    temperature=0.7,
    top_p=1,
)
```

#### Iteratively refining prompts using Python

```python
import openai

prompt = "Tell me about renewable energy sources."
num_iterations = 3

for i in range(num_iterations):
    response = openai.Completion.create(engine="davinci-codex", prompt=prompt, max_tokens=50)
    output_text = response.choices[0].text
    print(output_text)
    
    prompt = "Tell me more about how " + output_text.split()[-1] + " are used in renewable energy."
   
  ```
 #### Using Python to challenge the model  
```python
import openai

response = openai.Completion.create(
    engine="davinci-codex",
    prompt="I challenge you to write a poem about the universe in the style of Shakespeare.",
    max_tokens=100,
)
print(response.choices[0].text)
````


