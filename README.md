# prompt_engineering_and_langChain_prompt_templates

# build an LLM using IBM watsonx.ai

ibm-watsonx-ai: Enables the use of LLMs from IBM's watsonx.ai.
langchain: Provides various chain and prompt functions from LangChain.
langchain-ibm: Facilitates integration between LangChain and IBM watsonx.ai.

Some key parameters are explained here:

model_id specifies which model you want to use. There are various model options available; refer to the Foundation [Models documentation](https://ibm.github.io/watsonx-ai-python-sdk/v1.4.11/foundation_models.html)  for more options. In this tutorial, you'll use the granite-3-2-8b-instruct model.
parameters define the model's configuration. Set five commonly used parameters for this tutorial. To explore additional commonly used parameters, you can run the code GenParams().get_example_values(). If no custom parameters are passed to the function, the model will use default_params.
credentials and project_id are required to successfully run LLMs from watsonx.ai. (Leave credentials and project_id as they are so you don't need to create your own keys to run models.) This ensures you can run the model inside this lab environment.

# Basic prompt
A basic prompt is the simplest form of prompting, where you provide a short text or phrase to the model without any special formatting or instructions. The model generates a continuation based on patterns it has learned during training. Basic prompts are useful for exploring the model's capabilities and understanding how it naturally responds to minimal input.

# Zero-shot prompt
Zero-shot prompting is a technique where the model performs a task without any examples or prior specific training on that task. This approach tests the model's ability to understand instructions and apply its knowledge to a new context without demonstration. Zero-shot prompts typically include clear instructions about what the model should do, allowing it to leverage its pre-trained knowledge effectively.

# One-shot prompt
One-shot prompting provides the model with a single example of the task before asking it to perform a similar task. This technique gives the model a pattern to follow, improving its understanding of the desired output format and style. One-shot learning is particularly useful when you want to guide the model's response without extensive examples.

# Few-shot prompt
Few-shot prompting extends the one-shot approach by providing multiple examples (typically 2-5) before asking the model to perform the task. These examples establish a clearer pattern and context, helping the model better understand the expected output format, style, and reasoning. This technique is particularly effective for complex tasks where a single example might not convey all the nuances.

# Chain-of-thought (CoT) prompt
Chain-of-thought (CoT) prompting encourages the model to break down complex problems into step-by-step reasoning before arriving at a final answer. By explicitly showing or requesting intermediate steps, this technique improves the model's problem-solving abilities and reduces errors in tasks requiring multi-step reasoning. CoT is particularly effective for mathematical problems, logical reasoning, and complex decision-making tasks.

# Self-consistency
Self-consistency is an advanced technique in which the model generates multiple independent solutions or answers to the same problem, then evaluates these different approaches to determine the most consistent or reliable result. This method enhances accuracy by leveraging the model's ability to approach problems from different angles and identify the most robust solution through comparison and verification.

