# MP2 Reflection

## What worked

Section-based chunking worked best for me. I first tried a sliding-window approach, but some related information was split between chunks. With section-based chunking, the text stayed with its section heading, so the retrieved context was more useful and the answers became more relevant.

## What didn't work

The sliding-window approach was easy to start with, but it did not keep related context together. I also learned that retrieving the correct story does not always mean the answer includes all the expected facts. In my saved validation run, the expected source matched for all questions, but some fact-match scores were low, including 0/6 for the Speckled Band question. The saved learner results are from my earlier questions, before I updated them, so I still need to validate the new questions.

## What I'd change

With five more hours, I would first rerun validation with my updated questions and look at the retrieved chunks for any answers that miss facts. After that, I would try query rewriting, query decomposition with an LLM, and hybrid retrieval using both dense semantic search and sparse keyword search. I would compare the results to see which changes actually help.

## One surprise

I was surprised that the system could give relevant answers with a simple prompt when I provided useful context with the question. I did not need very long instructions for the LLM. At the same time, the validation showed me that a relevant answer does not always include every expected fact, so checking the retrieved context and the final answer is still important.
