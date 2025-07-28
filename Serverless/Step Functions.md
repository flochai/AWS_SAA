#Amazon 

[[Lambda]] functions have a 15-minute max execution time and the runtime environment is stateless so it is not possible to have large functions. It is also messy to chain functions together. 

The solution to this problem is the state machine which is a workflow model made of states, transitions, and rules that define how a process moves from one step to another. The different states are: 

- Succeed & Fail
- Wait (timer)
- Choice
- Parallel
- Map
- Task: a single unit of work performed by a state machine 

On AWS, step functions address the limitation of Lambda by letting the architect define state machines that allow for long workflows. Each state can make use of an AWS service. 

---
Links:

[[AWS Index]]
[[Lambda]]