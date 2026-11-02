# inquire

An AI interview agent for voice and text, with the evaluation suite and language models that support it.

**Status: early development. The items below are the plan, and no results exist yet.**

## Plan

- **Interview agent.** A state machine tracks interview progress and whether the person is frustrated or confused, then adapts its questions.
- **Evaluation.** 70 simulated personas with hidden fact sheets. The scorer measures fact recall, accuracy, attribution errors, cost and latency. 30 personas are held out.
- **Revision loop.** A 5-round loop proposes changes to the agent and accepts a change only if it improves results on held-out personas.
- **From-scratch model.** A sub-30M language model pre-trained on TinyStories, compared with the published TinyStories-33M checkpoint, then used to detect frustration and confusion.
- **Fine-tuned model.** A 1.5B open model fine-tuned with LoRA on filtered transcripts from a stronger open model, to lower interview cost.

Results will appear here once they are measured.
