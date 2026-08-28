Bedrock Evaluation Run 2 – Observation

Evaluation Run 2 completed successfully using the support-chatbot evaluation dataset and the Builtin.Correctness metric with Amazon Nova Pro as the evaluator.

The evaluation achieved a correctness score of 0.97. This indicates that the chatbot's responses were highly consistent with the expected behavior defined by the system prompt and the online shop FAQ.

The evaluation covered the main application paths:

1. Bug Report Path
The chatbot identifies reports of broken or malfunctioning features as bug reports. It collects the required bug description, steps to reproduce, and environment information before creating a ticket through the create_bug_report tool.

2. Platform Question Path
The chatbot answers supported customer questions using the embedded online shop FAQ. It provides information about orders, shipping, returns, refunds, payments, accounts, and privacy without inventing unsupported policies.

3. Other Request Path
For requests that are not covered by the FAQ or are outside the chatbot's supported scope, the chatbot directs the customer to human support at 1-800-555-0199 (Mon-Fri).

The 0.97 correctness score demonstrates that the final chatbot behavior closely matches the expected responses in the automated evaluation dataset. The small difference from a perfect score indicates that some individual responses may have had minor deviations from the expected answer, but the overall application behavior was highly accurate.

Run 2 was used as the final evaluation result rather than Run 1 [.9 correctness score] because the system prompt and application behavior were refined before the second evaluation.
