# From Personal Skills to Enterprise Agents

# Monday morning

**Tim:** It’s Monday morning. Elena has three spreadsheets open, last week’s inventory report beside her, and a meeting in an hour. She’s done this report for months. Combine the files, check the reservations, investigate the odd numbers, and write up what the team needs to know.

**Nichalia:** She knows the work and what good looks like. That matters, because today she’s going to ask an AI agent to help with it. We’ll follow her from that first attempt to something colleagues can use, and eventually a workflow that could run as a shared agent.

**Tim:** Elena puts the input files and a checked example report into a folder and creates a project in either the Claude or ChatGPT desktop app. This gives her desktop agent access to that folder, and she says, “Help me produce this week’s inventory report. The inputs and an example of the finished report are in the folder you have access to.”

**Nichalia:** The first draft looks promising but not good enough. For example, one line says there are a hundred and twenty-one units available. Elena knows forty are already reserved. She points out the error and explains the rule: available stock must exclude those reservations.

**Tim:** The next draft fixes that, but buries an important shortage halfway down the page. She asks for shortages at the top, with the evidence behind each one. Then she checks how it handles returns. They iterate through several versions, until the report is genuinely useful to support daily management.

**Nichalia:** During that back-and-forth, she asks the agent to save the instructions for producing the report as markdown files in the project folder: which files to use, what each field means, how to calculate availability, and what to do when something is missing. She’s making the reasoning explicit as they improve the standard operating procedures.

# Capturing and testing the skill

**Tim:** Now Elena says, “Turn the above reporting workflow into a reusable skill called Magenta Inventory Report.” The agent packages the method so she can invoke it again without rebuilding the conversation.

**Nichalia:** And now she can test the skill itself. Could it produce a good report without all the corrections she supplied during that original conversation?

**Tim:** She makes a small test set: several weeks of input files, the corresponding final reports she has checked, and a few difficult cases. A missing reservations file. An unexpected return. A product with no available stock. She documents what a good result should contain.

**Nichalia:** In a new project she invokes the skill with those inputs and compares the outputs. Are the numbers right? Are the important exceptions visible? Can she trace a conclusion back to the data? Does it flag missing information rather than invent an answer?

**Tim:** These repeated runs are important. One successful run doesn’t tell her whether the skill is dependable. When a result is wrong, she updates the skill and runs through the test set again, checking that the fix hasn’t broken something else.

**Nichalia:** She keeps a few sets of input data in reserve from the ones she is iterating over to improve the instructions. Those help show whether the skill handles a new situation that it hasn’t been tested and improved on before. This iteration continues until she’s comfortable the skill consistently meets her standard of a good human report.

**Tim:** Refining the skill’s instructions is real work but Elena builds it into her process. Each time the report isn’t right and she has to fix it, she tells her desktop agent to update the skill so she never has to make those manual corrections. Only after the skill meets her standards can she take the next step of sharing it with others.

# Sharing with a small team

**Nichalia:** Elena’s tests have given her confidence in the skill. So she tells her desktop agent, “Package this tested skill as a plugin called Magenta Inventory Report. Include the instructions, input requirements, supporting files, and known limitations, but no connectors.”

**Tim:** She doesn’t have to assemble it by hand. The plugin creator in her desktop agent does that work. The plugin is what she’ll share with her pilot group. It might contain one skill, or a few related ones. We’re starting with the skills; the connector approval process is separate.

**Nichalia:** And she makes one more request: “Give me a ZIP copy of the finished plugin.” In Claude you can just download that plugin ZIP file from the Customize tab; in other platforms you have to ask the agent to create it for you.

**Tim:** That exported ZIP file can be used to import the plugin to Claude, ChatGPT and other platforms.

**Nichalia:** She can now go into Customize and share the plugin with specified individuals who have agreed to test it.

**Tim:** She finds three teammates who have the Claude or ChatGPT license and agree to test it. She enters their names in the sharing dialog. Then she tells them how to add the plugin and invoke the reporting skill in a conversation that has the required input files.

**Nichalia:** Pro tip: you can just ask your desktop agent for a nicely formatted set of instructions on how to use the skill, or even create a quick website.

**Tim:** Each of these testers runs the skills in that plugin with their own inputs and lets her know the result. One teammate’s export uses a different column name. Another finds that the explanation of a shortage needs more context. Elena improves the skill, reruns her tests, asks her agent to update the plugin, and asks them to try again.

**Nichalia:** After several iteration cycles, the teammates are using it regularly. They can show the reports, describe the time saved, and confirm that the quality is useful for their work. Elena records that feedback and their sign-off. Now she has evidence to support wider distribution.

# Trying another approved platform

**Nichalia:** This is also a good time to try another approved platform. Elena takes the plugin ZIP the agent produced and uploads it through that platform’s plugin-upload process. She isn’t uploading the report or copying the whole conversation.

**Tim:** Elena runs her familiar tests again in the destination tool before sharing it with specified colleagues who want to test it on that other platform. At this point the plugin has proved its worth and she wants to make it available to anyone in her organization.

# Earning a place in the marketplace

**Tim:** In Claude, she opens the plugin and clicks “Publish to org.” This doesn’t make it live in the organization marketplace though, since publishing requires review. She submits it as available to install, with release notes and the pilot evidence. Where another platform needs a separate approval process, we’d establish the equivalent steps.

**Nichalia:** The review consists of a few parts. First off, the plugin is automatically scanned for malicious content.

**Tim:** The reviewer asks four questions. Did the automatic scan pass? Are colleagues actually using this and finding value? Does it duplicate something already in the catalog? And is the package and its intended use allowed under our policies?

**Nichalia:** We recommend being thoughtful about which plugins you submit to the company marketplace. Start with it as a personal skill, share it with a few colleagues, and only submit it for organization review if it has proven itself to be generally useful.

**Tim:** In this case, Elena’s plugin passes the review. The administrator approves it for the marketplace. That makes it available for anyone to install; it doesn’t force the plugin onto everyone’s account.

**Nichalia:** While a human would do that review at the beginning, just like with Elena’s skill, we can teach an AI agent what rules we want, iterate, and eventually it can complete most of the review by itself. It can’t click the approve button though; that is the responsibility of the admin.

# More people use it and Elena keeps improving it

**Tim:** The story continues. A colleague in another team finds Magenta Inventory Report in the marketplace, reads what it does, and clicks “Add.” They bring their own inputs, invoke the skill, and check whether it helps them. Now the method can reach people Elena has never met.

**Tim:** Meanwhile, Elena keeps improving her own copy. Suppose she adds a clearer explanation of slow-moving stock. She tests the revised skill, gets feedback, and submits a new version with a description of what changed.

**Nichalia:** That version goes through the review process again. The currently approved version remains in use until the replacement is approved. Wider distribution makes disciplined updates more important, because more people now depend on the result.

# From regular use to a managed agent

**Tim:** Some colleagues run the report only when they need it. Others decide to schedule it every Monday at 8 AM. They choose that separately, after making sure the inputs will be available and the task handles missing or stale data sensibly.

**Nichalia:** Eventually, several teams depend on this report. It’s used repeatedly and delivers enough value to justify operating it as a shared workspace agent, inside a platform or on another approved cloud service.

**Tim:** So what happens then?

**Nichalia:** They give that agent a supported home, approved access to its inputs, an owner, monitoring, and cost controls. It can run without depending on Elena’s desktop being open or her remembering to start it. Some schedules already run remotely; this step is about taking responsibility for a shared capability.

**Tim:** In a future episode, we’ll look at how to build one of these shared agents—or submit a proven workflow to be professionally developed into an enterprise autonomous agent or app.

**Nichalia:** Elena’s original folder of files has led somewhere useful. But she didn’t begin by asking for an enterprise agent. She began with a report she understood, figured out how her desktop agent could help her, captured the method, and tested it.

**Tim:** Then she taught a few colleagues to use it, gained confidence in the solution, and submitted it to be used broadly. Each handoff made the next one possible. Whether your own idea stays a personal skill or reaches that final stage, that’s a process you can start with the work on your desk today.

# Reference notes

These notes and section headings are not spoken. Only the Tim and Nichalia dialogue is narrated.

**Packaging clarification:** The plugin creator builds a plugin directory and manifest, validates it, and produces a ZIP-based `.plugin` artifact with an installation preview. The script’s process explicitly asks for editable source and a downloadable `.zip` copy at creation. Named sharing inside Claude is separate from moving that copy to another platform. An ordinary managed-plugin export button has not been established; Claude’s administrator Plugins API can download an exact version, but this story does not depend on that route.

Elena, her colleagues, report details, test results, and rollout are illustrative—not claims about an actual company deployment.

- **Primary editorial source:** Tim’s October 25 direction and five-column diagram. Plugin packaging before sharing, named pilot testers, evidence of value, skills-only submissions, the four review criteria, opt-in installation, and selective promotion to agents are the process being proposed.

- [Anthropic: Use plugins in Claude](https://support.claude.com/en/articles/13837440-use-plugins-in-claude): named sharing, skill invocation, Add, and Publish to org. This story assumes an eligible organizational plan with sharing enabled. Requiring a plugin before sharing is this process’s rule, not a claim that standalone skill sharing is technically impossible.

- [Anthropic: Provision and manage skills for your organization](https://support.claude.com/en/articles/13119606-provision-and-manage-skills-for-your-organization): review-required publishing, fixed submitted versions, optional availability, and review of later versions. The story assumes Elena is a member submitting to a reviewer, not an owner whose own submission may bypass review.

- [Anthropic: Skill and plugin scanning](https://support.claude.com/en/articles/15927065-get-started-with-skill-and-plugin-scanning): security scanning of covered uploads and edits. The story assumes Enterprise scanning is enabled and the upload is in scope. Coverage has exceptions; a scan does not evaluate business correctness or guarantee safety in every respect.

- **Cross-platform example:** Tim reports testing the same plugin package in Claude, ChatGPT, and Copilot Cowork. This is his tested example, not a guarantee that every component or workflow is universally portable. Destination upload permissions, organizational availability, and re-testing still matter.

- [Anthropic: Schedule recurring tasks in Claude Cowork](https://support.claude.com/en/articles/13854387-schedule-recurring-tasks-in-claude-cowork): scheduled use of skills and plugins; local-file requirements can keep a run local, while other scheduled tasks can already run remotely.

- [OpenAI: ChatGPT workspace agents](https://help.openai.com/en/articles/20001143-chatgpt-workspace-agents-for-enterprise-and-business): reusable agents with skills, tools, testing, sharing, schedules, and API triggers. The final stage requires deliberate deployment and authorized data access; installing a plugin does not create an always-running agent.

- [Anthropic plugin creator source](https://raw.githubusercontent.com/anthropics/knowledge-work-plugins/main/cowork-plugin-management/skills/create-cowork-plugin/SKILL.md): plugin directory, manifest, validation, and ZIP-based `.plugin` output.

- [OpenAI: Plugins in ChatGPT](https://help.openai.com/en/articles/20001256-plugins-in-chatgpt): destination plugin workflow and requirements.

- [Microsoft: Plugins in Copilot Cowork](https://learn.microsoft.com/en-us/microsoft-365/copilot/cowork/cowork-plugins): destination plugin support and organizational requirements.
