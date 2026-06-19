# Symbolic/Equation-Only CoD

Symbolic/Equation-Only CoD restricts the intermediate reasoning steps of the LLM entirely to mathematical or symbolic representations.

## How It Works
By bypassing natural language explanations entirely, the model is directed to output only numbers, operators, or variables (e.g., `5 * 2 = 10` $\rightarrow$ `10 + 3 = 13`) before outputting the final answer. This minimizes token counts dramatically.

## Diagram
```mermaid
graph TD
    A[Problem: Jason has 20 apples, gives 8 to Denny] --> B[Symbolic CoD Prompt]
    B --> C[LLM Output: 20 - 8 = 12]
    C --> D[Final Answer: 12]
```

## Benefits
- Perfect for mathematical or symbolic logic tasks.
- Eliminates semantic ambiguity.
- Extremely high token compression.
