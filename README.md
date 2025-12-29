# prompt_engineering_and_langChain_prompt_templates

# build an LLM using IBM watsonx.ai

ibm-watsonx-ai: Enables the use of LLMs from IBM's watsonx.ai.
langchain: Provides various chain and prompt functions from LangChain.
langchain-ibm: Facilitates integration between LangChain and IBM watsonx.ai.

Some key parameters are explained here:

model_id specifies which model you want to use. There are various model options available; refer to the Foundation [Models documentation](https://ibm.github.io/watsonx-ai-python-sdk/v1.4.11/foundation_models.html)  for more options. In this tutorial, you'll use the granite-3-2-8b-instruct model.
parameters define the model's configuration. Set five commonly used parameters for this tutorial. To explore additional commonly used parameters, you can run the code GenParams().get_example_values(). If no custom parameters are passed to the function, the model will use default_params.
credentials and project_id are required to successfully run LLMs from watsonx.ai. (Leave credentials and project_id as they are so you don't need to create your own keys to run models.) This ensures you can run the model inside this lab environment.

