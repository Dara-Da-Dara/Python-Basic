# 🚀 Usage of 2024 Gen-AI Python Libraries

## 1. Transformers (Hugging Face)
_Run pretrained LLMs easily._

```python
from transformers import pipeline

# Load a text-generation pipeline with a small model
generator = pipeline("text-generation", model="gpt2")
print(generator("AI in 2024 will", max_length=40, num_return_sequences=1))
```

---

## 2. Diffusers (for images, audio, video)
_Generate images from text with Stable Diffusion._

```python
from diffusers import StableDiffusionPipeline
import torch

pipe = StableDiffusionPipeline.from_pretrained("runwayml/stable-diffusion-v1-5")
pipe = pipe.to("cuda")  # use GPU if available

image = pipe("A futuristic city skyline at sunset").images[0]
image.show()
```

---

## 3. PEFT (Parameter Efficient Fine-Tuning)
_LoRA fine-tuning on top of Hugging Face models._

```python
from peft import LoraConfig, get_peft_model
from transformers import AutoModelForCausalLM

model = AutoModelForCausalLM.from_pretrained("gpt2")
config = LoraConfig(task_type="CAUSAL_LM", r=8, lora_alpha=16, lora_dropout=0.1)
peft_model = get_peft_model(model, config)
print("Model ready for parameter-efficient fine-tuning 🚀")
```

---

## 4. LangChain
_Build LLM apps (chains, agents)._

```python
from langchain.prompts import PromptTemplate
from langchain.llms import OpenAI

llm = OpenAI(temperature=0.7)  # needs OPENAI_API_KEY env var

template = PromptTemplate.from_template("Tell me a story about {topic}")
print(llm(template.format(topic="an AI-powered robot in 2024")))
```

---

## 5. Tiktoken
_Tokenize text (useful for cost estimation + LLM inputs)._

```python
import tiktoken

enc = tiktoken.get_encoding("cl100k_base")
tokens = enc.encode("Generative AI is transforming industries.")
print("Tokens:", tokens)
print("Decoded:", enc.decode(tokens))
```

---

## 6. Bitsandbytes
_Memory-efficient quantized inference/training._

```python
from transformers import AutoModelForCausalLM, AutoTokenizer
import torch

model_name = "meta-llama/Llama-2-7b-hf"
tokenizer = AutoTokenizer.from_pretrained(model_name)

# Load in 4-bit precision to save VRAM
model = AutoModelForCausalLM.from_pretrained(model_name, load_in_4bit=True, device_map="auto")

inputs = tokenizer("Hello AI world!", return_tensors="pt").to("cuda")
outputs = model.generate(**inputs, max_new_tokens=30)
print(tokenizer.decode(outputs[0], skip_special_tokens=True))
```

---

## 7. Accelerate
_Handle multi-GPU / mixed precision training with ease._

```python
from accelerate import Accelerator

accelerator = Accelerator()
print("Accelerator device:", accelerator.device)
```

---

## 8. Datasets
_Easy access to thousands of datasets._

```python
from datasets import load_dataset

dataset = load_dataset("imdb")
print(dataset["train"][0])  # sample movie review
```

---

✅ These libraries together cover **text, image, fine-tuning, orchestration, tokenization, quantization, distributed training, and datasets** — a full Gen-AI development stack in Python (2024 versions).
