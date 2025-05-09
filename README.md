# Finetuning-DeepSeekR1-distill-model-1.5B

A lightweight, fine-tuned language model based on the DeepSeek-R1 Distill Qwen architecture with 1.5 billion parameters. This model is designed for efficient reasoning, mathematical problem-solving, and logical inference, making it ideal for resource-constrained environments and edge deployments.

Key Features

1.5B parameters for a compact yet capable model size

Fine-tuned on high-quality reasoning data generated by DeepSeek-R1

Excels at mathematical reasoning, achieving 83.9% on the MATH-500 benchmark (high-school-level math problems)

Demonstrates strong logical inference and basic reasoning skills

Optimized for performance and efficiency on limited compute resources

Suitable for deployment on mobile, edge, and low-power devices

Performance Highlights

Benchmark	Score	Description
MATH-500	83.9%	High-school-level math & logical reasoning
LiveCodeBench	16.9%	Basic coding abilities
Model Details

Architecture: Qwen-based, distilled from larger DeepSeek-R1 models

Training: Fine-tuned with 800k+ curated reasoning samples

License: MIT (weights); Qwen base under Apache 2.0

Use Cases

Educational tools and math assistants

Logic and reasoning applications

Lightweight chatbots and virtual assistants

Edge AI and mobile deployments

How to Use

python
# Example: Load with Hugging Face Transformers
from transformers import AutoModelForCausalLM, AutoTokenizer

model = AutoModelForCausalLM.from_pretrained("your-finetuned-model-repo")
tokenizer = AutoTokenizer.from_pretrained("your-finetuned-model-repo")
About DeepSeek-R1 Distill

The DeepSeek-R1 Distill series demonstrates that advanced reasoning capabilities from large models can be effectively transferred to smaller, more efficient architectures-offering a strong balance between performance and resource requirements.

"This lightweight model demonstrates that reasoning patterns from larger models can be effectively distilled into much smaller architectures, making it ideal for resource-constrained deployments."
