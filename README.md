# promptengineering_week1_experiment3
# Experiment 3 – Iterative Prompt Refinement

## Aim

To demonstrate iterative prompt refinement by improving a prompt step-by-step to explain **photosynthesis to a 10-year-old child**.

## Problem Statement

The experiment starts with a basic prompt and progressively improves it through two refinement rounds.

- **Iteration 0:** Basic explanation.
- **Iteration 1:** Adds a simple analogy, short explanation, and simple language.
- **Iteration 2:** Adds a memory trick and simple diagram description.

## Tools and Technologies

- Python
- Google Colab
- Google Gemini API
- `google-genai` library
- `python-dotenv`

## Prompt Refinement

### Iteration 0 – Baseline

> Explain photosynthesis to a 10-year-old.

### Iteration 1 – Analogy and Brevity

> You are a friendly science teacher. Explain photosynthesis to a 10-year-old using a simple analogy. Keep the explanation to 3 short sentences and avoid technical jargon.

### Iteration 2 – Mnemonic and Diagram

> You are a friendly science teacher. Explain photosynthesis to a 10-year-old using a simple analogy. Keep the explanation short and avoid technical jargon. Include a simple memory trick and describe a basic diagram.

## Algorithm

1. Set up the Gemini API key.
2. Create a function to send prompts to the Gemini model.
3. Define the baseline prompt.
4. Send the baseline prompt and display the response.
5. Analyse the baseline response.
6. Create the first refined prompt.
7. Send and display the first refined response.
8. Analyse the improvement.
9. Create the second refined prompt.
10. Send and display the final response.
11. Compare all three outputs.
12. Save the results to a text file.

## Expected Output

The program displays:

- Iteration 0 prompt and response.
- Iteration 1 prompt and response.
- Iteration 2 prompt and response.
- Analysis after each iteration.
- Final summary comparing the three iterations.

The responses are also saved in:

`experiment_3_results.txt`

## Conclusion

The experiment demonstrates that iterative prompt refinement can improve the quality of an LLM response. Adding an analogy and simple language improves clarity, while adding a memory trick and diagram description improves memorability and visualization.

## Repository Structure

```text
experiment-3-prompt-refinement/
│
├── experiment_3_prompt_refinement.ipynb
├── experiment_3_prompt_refinement.py
├── experiment_3_results.txt
├── README.md
├── .env.example
├── .gitignore
│
└── outputs/
    └── output_1.png
```

## API Key Security

The actual Gemini API key must not be uploaded to GitHub.

The repository contains only `.env.example`:

```text
GEMINI_API_KEY=your_api_key_here
```

The real `.env` file is excluded using `.gitignore`.
