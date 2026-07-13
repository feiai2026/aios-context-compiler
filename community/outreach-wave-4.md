<!-- outreach-wave-4 -->

@darrenhinde — OpenAgentsControl's ContextScout, ContextManager, MVI principle, and OpenCode/Claude Code integration are the closest public prior art we have found to this product direction.

Rather than duplicate OAC, we are testing a narrower missing layer: a model-driven compiler that fully controls every provider request, records exactly which context and tools entered each loop, and runs an independent A/B protocol that separates token savings from task quality.

Two questions would help determine whether these efforts should connect:

1. Can OAC's current agent/plugin path prove that unselected native instructions, tools, skills, or history never bypass ContextScout and enter the final request?
2. What raw experiment supports the public `8,000 -> 750 tokens / 80% reduction` claim, and which task-quality metric would you pair with it?

Our aggregate evidence and its limitations are public: https://github.com/feiai2026/aios-context-compiler/tree/main/evidence

If the boundary looks complementary, we would value a short design review and can explore an integration or shared experiment before discussing any deeper collaboration. A critical “this should live inside OAC instead” answer would also be useful.
