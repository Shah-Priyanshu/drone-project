Created: .opencode/agent/docs-maintainer.md
This agent is configured as a subagent that you or your friend can invoke by mentioning it:
@docs-maintainer help me organize these meeting notes
Key features of this agent:
- Specialized tools: Has access to file operations (read, write, edit) and git commands
- Smart permissions: Will ask before running git commands but auto-approve other operations
- Project-aware: Knows about your team (Pri and Sam), version roadmap, and documentation structure
- Temperature 0.3: Balanced between focused and slightly creative for good documentation writing
- Uses Claude Sonnet 4: A capable model for understanding context and organizing information
How to use it:
1. In your OpenCode session, mention the agent: @docs-maintainer
2. It will automatically handle documentation tasks based on the instructions
3. You can also let the primary Build agent invoke it automatically when working on documentation
The agent now has all the context and instructions from our session built right in!