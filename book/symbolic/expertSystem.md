# Expert System

Created by researchers at Stanford University, an expert system uses knowledge from a human expert to emulate one. They can be generally split into two parts: the knowledge base and the inference engine.

## Knowledge Base

It is a collection of expert knowledge in order to imitate a human expert.  The quality and depth of this information is what generally determines the success of expert systems.

The data can be represented in a couple ways:

* Assertions about variables
* Object-oriented assertions
* If-Then statements

## Inference Engine

It applies the rules of the knowledge base to the facts to ensure they comply. It can then uses the rules and facts to make inferences, if necessary, which are added into the knowledge base.

There are two methods for finding a solution:

* Forward Chaining
* Backward Chaining

### Forward Chaining

The inference engine begins with given facts and deduces new facts which it adds to the knowledge base and continues to do so until a solution is found.

This strategy is for determining a conclusion based on given facts, predicting an effect of the givens.

### Backward Chaining

The inference engine begins with a given result and deduces new facts for the result to occur and continues to do so until no more causes can be determined.

This strategy is for determining causes of a result.