<!-- outreach-wave-1 -->

@kitlangton @code-yeongyu — your work on OpenCode instruction checkpoints/compaction and oh-my-openagent context injection is directly relevant to the failure mode we are testing.

We observed a consistent efficiency signal in a controlled-but-still-manual setup: 30/30 paired trials used fewer total tokens, averaging -50.8%. We are **not** treating that as proof that an automatic compiler improves task success. The next step is to make context selection automatic and fully control every OpenCode model request.

The most useful response would be a critical one: **where is this design most likely to leak native context, or optimize tokens while hurting task quality?**

- Runtime control-plane spike: https://github.com/feiai2026/aios-context-compiler/issues/2
- Independent context/eval protocol: https://github.com/feiai2026/aios-context-compiler/issues/3

No endorsement is implied or expected. A short objection or a pointer to prior art would already be valuable.
