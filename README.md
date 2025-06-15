# AI Model Comparison Sheet

This comparison evaluates four AI models: **GPT-4o**, **Claude Sonnet**, **Gemini Flash**, and **DeepSeek-R1:7B (via Ollama)**. Each model was tested on real-world software development use cases including bug resolution, code generation, data analysis, and infrastructure automation.

---

## 🧪 Evaluation Criteria

Each model was evaluated on the following capabilities:

- **Code Quality** – Ability to generate clean, readable, and correct code.
- **SQL Generation** – Skill in handling SQL tasks such as joins, filters, and aggregations.
- **Infrastructure Automation** – Writing scripts or commands for DevOps and cloud infrastructure.
- **Ease of Use** – Accessibility, setup, and user-friendliness.
- **Speed / Latency** – Time taken to respond with usable output.

> 💡 **My primary use case**:  
> I frequently use these AI models to identify and fix bugs in **Node.js** and **Angular** applications, especially related to async issues, template errors, and API handling.

---

## 📊 Model Comparison Table

| Model              | Code Quality | SQL Generation | Infra Automation | Ease of Use | Speed / Latency | Comments |
|--------------------|--------------|----------------|------------------|-------------|------------------|----------|
| **GPT-4o**         | Excellent    | Excellent      | Good             | Excellent   | Good             | Helped resolve a Node.js API error and an Angular rendering bug caused by `*ngIf` logic. Great at interpreting stack traces and suggesting precise changes. |
| **Claude Sonnet**  | Good         | Good           | Basic            | Excellent   | Excellent        | Suggested fixes for issues with `FormArray` rendering in Angular templates. Very natural explanations, helpful for learning and debugging. |
| **Gemini Flash**   | Good         | Excellent      | Good             | Good        | Excellent        | Helped rewrite a MongoDB aggregation in Node.js and debug a reactive form binding issue in Angular. Fastest model in terms of output. |
| **DeepSeek-R1:7B** | Limited      | Good           | Good             | Moderate    | Excellent (local) | Handled basic JavaScript and Node.js issues well. Struggled with Angular-specific concepts like lifecycle hooks or structural directives. Useful for quick offline tasks. |

---

## 🔍 Real Prompts Used During Testing

### Node.js Bug Fixing
> “Why is my Express route not catching a ForbiddenException even though it's inside a try-catch block?”

### Angular Debugging
> “Fix an issue where a component’s template is not rendering a section correctly using *ngIf and async pipe.”

### SQL Generation
> “Write a SQL query to fetch users with at least 3 failed login attempts in the past 7 days.”

### Infrastructure Automation
> “Create a bash script to deploy an Nginx Docker container and set up a health check endpoint.”

---

## 🏁 Summary & Observations

- **GPT-4o**: Best overall. Accurate across all tasks, especially good at handling full-stack app bugs.
- **Claude Sonnet**: Great for explanation-based debugging and understanding complex code. Slightly wordy.
- **Gemini Flash**: Lightning fast, strong with structured data and shell scripting. Angular support is good but needs careful prompting.
- **DeepSeek-R1:7B**: Great local model for simple logic or offline coding. Best used as a backup, not for complex UI frameworks.

---

## 🔧 Test Environment

- **GPT-4o**: Used via ChatGPT Pro (OpenAI)
- **Claude Sonnet**: Accessed via Claude.ai (Anthropic)
- **Gemini Flash**: Tested on Google AI Studio
- **DeepSeek-R1:7B**: Deployed locally using `ollama` on macOS M1 with 16GB RAM

---

## 📎 Legend

- **Excellent** – Consistently accurate and reliable
- **Good** – Performs well with occasional limitations
- **Basic / Limited** – Works for simple cases only
- **Not Supported** – Task not handled properly

