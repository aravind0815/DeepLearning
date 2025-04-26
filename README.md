# StarCoder2 SQL Instruction Generation Project

> Deep Learning Project | DS677 | NJIT  
> Authors: Uyen Nguyen, Aravind Kalyan Sivakumar, Kartik Pandit

---

## About the Project

This project leverages **StarCoder2-15B**, a large language model, and a custom **Tree-sitter-SQL** parser to automatically generate SQL code, instructions, and explanations.  
We designed a pipeline to automate and validate SQL code generation using **few-shot prompting** and **self-validation** techniques.

---

## Key Components

- **HF Token Setup** and Environment Configuration
- **Tree-sitter-SQL Parser** for tokenizing SQL code
- **Seed to Concept (S→C)** stage for extracting task concepts
- **Concept to Instruction (C→I)** stage for generating natural language instructions
- **Instruction to Response (I→R)** stage for generating solutions
- **Few-shot Prompting** for SQL tasks
- **Self-Validation Scripts** to validate SQL responses

---

## How It Works

1. **Seed Gathering**  
   Extracted 100K SQL code snippets and prepared them for processing.

2. **Concept Extraction (S→C)**  
   Identified core tasks and keywords from the seed code.

3. **Instruction Generation (C→I)**  
   Generated clear, human-readable instructions from extracted concepts.

4. **Response Generation (I→R)**  
   Generated SQL queries and explanations for each instruction.

5. **Self-Validation**  
   Automatically executed generated SQL to validate correctness.

---

## Technologies Used

- **StarCoder2-15B** model
- **Tree-sitter-SQL** (SQL parser)
- **VLLM** inference server
- **Python** for scripting
- **Bash** for environment setup

---

## Folder Structure

- `seed/` : Sample seed JSON files.
- `scripts/` : Automation scripts for environment setup and execution.
- `examples/` : Few-shot examples used for model prompting.
- `docs/` : Project documentation (includes project report PDF).

---

## Installation

```bash
# Clone the repository
git clone https://github.com/yourusername/StarCoder2-SQL-DeepLearning-Project.git
cd StarCoder2-SQL-DeepLearning-Project

# Install dependencies
pip install -r requirements.txt
```

---

## License

This project is licensed under the MIT License.

---

# 🚀 Contribution

Open to contributions! Feel free to fork, raise issues, or submit pull requests.

---

# 📄 Acknowledgments

- Professor Hai Phan (NJIT)
- NJIT DS677 Deep Learning Course
