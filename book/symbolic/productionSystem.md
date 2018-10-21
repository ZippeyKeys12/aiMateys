# Production System

Used in [expert systems](expertSystem.md) to store the rules used to make inferences and determine a solution. A production system is used specifically for [forward chaining](expertSystem.md#forward-chaining)

The rules, known as productions, are comprised of two parts: the condition and the action. If the given condition is satisfied by current facts then the action is executed. The productions must also  have an order in case of multiple being executed.