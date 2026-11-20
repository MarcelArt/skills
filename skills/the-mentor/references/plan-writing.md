# Write a learning plan

## Choose the destination

- Use `learning/<topic-slug>/` inside the workspace by default. Honor a learner-specified destination inside the workspace. Inspect the target first and make sure its resolved path stays inside the workspace. If it is unclear whether to reuse a populated target, ask or choose a new unoccupied folder. Revise existing lessons only when asked and preserve learner notes.
- Create only the plan directory and its Markdown files. Keep source code, commands, and exercises inside Markdown. If workspace writes are unavailable, share the proposed Markdown files in chat under distinct filenames.

## Make lessons easy to follow

- Write a brief `README.md` with the goal, prerequisites, an ordered list of relative lesson links, and where to begin. Create more than one lesson file, with names such as `01-first-program.md` and `02-read-input.md`. Give each file one outcome. Size the sequence to the learner's goal and split any lesson that covers several independently useful steps.
- Start a lesson with what the learner will do and why. Give one small worked example or demonstration where it helps, then a task they do themselves. End with an observable check such as expected output, visible behavior, or a question they can answer, and a link to the next lesson if one exists.
- Use short paragraphs, bullets, and familiar words. Define a new term near its first use. Include only setup the learner needs for that step. Keep setup explanations close to the commands they describe.
- Put code and terminal commands in separate, language-tagged fences. Say which file or directory each block belongs in. Give enough context to copy and run it. Keep shell prompts and sample output outside command blocks. Explain any placeholder before the learner uses the block.
- Verify that the index and lesson links resolve and that each lesson has a clear action and check. Link the index and first lesson in chat so the learner can start there.
