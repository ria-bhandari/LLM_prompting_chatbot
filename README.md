# Language Learning Model Prompting - Color Preference Chatbot

This project uses a conversational AI Model (gpt-3.5 Turbo) to simulate different personas and understand their favorite colors. It also provides a description to explain their choices. 

The AI has been configured for the above purpose in the `system_message` and `prompt` variables in `llm_prompting.ipynb`.

#### System Message
```python
system_message = "You are a helpful assistant that provides information about any topic that the user asks you."
```

#### Prompt

```py
prompt = f"You are a {persona['age']}-year-old and you are a {persona['occupation']}. List your favorite color among Pink, Yellow, Grey, Purple in the first word of your response and describe it two sentences."
```

## Table of Contents 

- [About](#about)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)


## About

The Color Preference Chatbot in this project is designed to collect data on ceratin people's favorite colors based on their age and occupation.

## Getting Started

To get started with this project on your machine, follow the instructions

### Prerequisites 

- Python 3.6 or higher
- OpenAI GPT-3 API key (edit cell 2 of `llm_prompting.ipynb`)

### Installation

1. Clone this repository:
```bash
git clone https://github.com/ria-bhandari/LLM_Prompting
```

2. Install the required modules using pip
```
pip install -r requirements.txt
```

3. Set up your API key on your OpenAI account online and replace it


### Plot of Color Preference vs. Occupation

<img width="840" alt="Screenshot 2023-10-01 at 2 22 37 PM" src="https://github.com/ria-bhandari/LLM_prompting_chatbot/assets/121469289/4419bf7d-000e-4f8e-a465-5bba72d95864">

In the example, the AI has simulated the personas: 
1. A 20 year old construction worker
2. A 60 year old golfer
3. A 7 year old primary school student

The bar chart provides an overview of what color the chat model chose the most for each persona. The persona can be edited for a different age or occupation in the below code snippet, which is the third cell of `llm_prompting.ipynb`.

```python
# Declare persona space
persona_space = [
    {"age": 20, "occupation": "construction worker"},
    {"age": 60, "occupation": "golfer"},
    {"age": 7, "occupation": "primary school student"},
]
```


