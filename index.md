So Hirota, shirota@ucsd.edu
Reasoning with Large Language Models, Professor Hu Zhiting

1. What is the most interesting topic covered in your domain this quarter?
The most interesting idea we have covered are Process Reward Models. There is growing research to suggest that 
pre-trained LLMs by themselves are not sufficient to perform complex logical thought out-of-the-box. Process
Reward Models (PRMs) aim to reward models for correct process in their chain-of-thoughts, and this approach is opposed 
to the Outcome Reward Models (ORMs), which simply rewards the model for the correct final reasoning. Intuitively, PRMs should
work better than ORMs as rewards from PRMs are more fine-grained. It is trivial to think of a situation were an incorrect reasoning
path may still lead to the correct outcome. In our capstone, we want to do something with PRMs.
2. Describe a potential investigation you would like to pursue for your Quarter 2 Project.
I think our group is interested in exploring multi-modal reasoning for web-agents. Perhaps we can investigate the efficacy of PRM
style supervision for task completion on the web by LLMs.
3. What is a potential change you’d make to the approach taken in your current Quarter 1 Project?
For our checkpoint, we implemented a baseline approach for a teacher-student framework for LLM reasoning. Specifically,
there was a larger teacher model that would supervise and provide feedback to a smaller model's reasoning steps. We saw
improvements across different teacher models after 1, 2, and 3 steps of iterative feedback. However, our evaluation metric
was flawed. We marked a question correct if the larger teacher model deemed it as correct. There could be a bias for 
teacher models to prefer their thought processes over the small models thought process (even if the process was correct). 
Plus, we unsure about how reliable the teacher model is at accurately assessing the correctness of math problems. So we definitely
need to improve upon the evaluation metric. 
4. What other techniques would you be interested in using in your project?
I read a paper on using test-time fine-tuning (TTT) to achieve SOTA on the ARC-AGI prize, and thought that might be interesting
for general reasoning problems like math. However, the TTT paradigm is pretty limited, as they need to generate permutations of
the given problem, and train on the ground truth of permuted questions. But if we're trying to solve this novel question,
we should not have ground truth labels for permuted questions, so tat may be a limit. 