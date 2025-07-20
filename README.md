<img width="960" height="532" alt="460220361-eb67af3c-6496-4ac6-9b2e-858c917ffbb8" src="https://github.com/user-attachments/assets/b1ddcc59-ca08-4c17-bb55-27645e55cf2f" />


## Kubernetes AI Foundation LiteLLM | ☸️
Call all LLM APIs using the OpenAI format [Bedrock, Huggingface, VertexAI, TogetherAI, Azure, OpenAI, Groq etc.] 

🎯 Features
```
✅ Minio Object S3 Storage
✅ Keda AutoScaler 
✅ Velero Data Migration
✅ Argo Events 

```

🔨 Example : 

```
from litellm import completion
import os

## set ENV variables
os.environ["OPENAI_API_KEY"] = "your-openai-key"
os.environ["ANTHROPIC_API_KEY"] = "your-anthropic-key"

messages = [{ "content": "Hello, how are you?","role": "user"}]

# openai call
response = completion(model="openai/gpt-4o", messages=messages)

# anthropic call
response = completion(model="anthropic/claude-sonnet-4-20250514", messages=messages)
print(response)
---
