# Chain-of-Thought Prompting

## Base models

Base models can be prompted to answer questions

## Language Models Are Few-Shot Learners (NIPS 2020)

Shows showing a few examples of the task in context, "primes" the model states (activations) to detect a pattern (or, known task).
This helps model to perform tasks, but limited to reasoning task.
Referred to as "In-Context Learning"

## Reasoning Task

Tasks involving multiple steps.

## Chain-of-Thought

Showing reasoning steps => answer, helps model to break down multi-step tasks.
Increases performance as shown in previous papers which trained models to generate chain-of-thought.

## Languagen Models Are Zero-Shot Reasoners (NIPS 2022)

Just adding "Let' think step-by-step" to prompt triggers model to generate reasoning path.
Better than standard few-shot with no such triggers.

## Chain-of-Thought Prompting Elicits Reasoning in Large Language Models (NIPS 2022)

Why not teach models in-context to generate chain-of-thought?
Adding few examples of tasks with reasoning paths, helps models "mimic" reasoning.
We get benefit of few-shot + reasoning (breaking down).

## Self-Consistency Improves Chain of Thought Reasoning in Language Models (ICLR 2023)

Rather than sampling the response once with cot-prompting, we sample `k` times.
Out of that, take the most _consistent_ one (e.g. most frequent).