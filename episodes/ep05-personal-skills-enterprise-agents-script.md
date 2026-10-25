# Episode 5: From Personal Skills to Enterprise Agents

## Sources and editorial context

**October 25, 2026 · Story-driven episode**

This episode follows Elena, a fictional operations colleague, through Tim’s proposed five-stage process. Her colleagues, report details, test results, and rollout are illustrative, not claims about an actual company deployment.

- **Primary editorial source:** Tim’s October 25 direction and five-column diagram. Plugin packaging before sharing, named pilot testers, evidence of value, skills-only submissions, the four review criteria, opt-in installation, and selective promotion to agents are the process being proposed.
- [Anthropic: Use plugins in Claude](https://support.claude.com/en/articles/13837440-use-plugins-in-claude): named sharing, skill invocation, Add, and Publish to org. This story assumes an eligible organizational plan with sharing enabled. Requiring a plugin before sharing is this process’s rule, not a claim that standalone skill sharing is technically impossible.
- [Anthropic: Provision and manage skills for your organization](https://support.claude.com/en/articles/13119606-provision-and-manage-skills-for-your-organization): review-required publishing, fixed submitted versions, optional availability, and review of later versions. The story assumes Elena is a member submitting to a reviewer, not an owner whose own submission may bypass review.
- [Anthropic: Skill and plugin scanning](https://support.claude.com/en/articles/15927065-get-started-with-skill-and-plugin-scanning): security scanning of covered uploads and edits. The story assumes Enterprise scanning is enabled and the upload is in scope. Coverage has exceptions; a scan does not evaluate business correctness or guarantee safety in every respect.
- **Cross-platform example:** Tim reports testing the same plugin package in Claude, ChatGPT, and Copilot Cowork. The spoken script preserves that result and treats a Copilot Cowork organizational launch as conditional. It does not claim every plugin component or workflow is universally portable.
- [Anthropic: Schedule recurring tasks in Claude Cowork](https://support.claude.com/en/articles/13854387-schedule-recurring-tasks-in-claude-cowork): scheduled use of skills and plugins; local-file requirements can keep a run local, while other scheduled tasks can already run remotely.
- [OpenAI: ChatGPT workspace agents](https://help.openai.com/en/articles/20001143-chatgpt-workspace-agents-for-enterprise-and-business): reusable agents with skills, tools, testing, sharing, schedules, and API triggers. The final stage requires deliberate deployment and authorized data access; installing a plugin does not create an always-running agent.

## Monday morning

ANDREW: It’s Monday morning. Elena has three spreadsheets open, last week’s inventory report beside her, and a meeting in an hour. She’s done this report for months. Combine the files, check the reservations, investigate the odd numbers, and write up what the team needs to know.

AVA: She knows the work. That matters, because today she’s going to ask an AI agent to help with it. We’ll follow her from that first attempt to something colleagues can use, and eventually a workflow that could run as a shared agent. This is an AI-generated conversation about a proposed process.

ANDREW: Elena puts the input files and a checked example report into a project folder. She opens her Claude or ChatGPT desktop app, gives the agent access to that folder, and says, “Help me produce this week’s inventory report. Here are the inputs and an example of what I need.”

AVA: The first draft looks promising. But one line says there are a hundred and twenty units available. Elena knows forty are already reserved. She points out the error and explains the rule: available stock must exclude those reservations.

ANDREW: The next draft fixes that, but buries an important shortage halfway down the page. She asks for shortages at the top, with the evidence behind each one. Then she checks how it handles returns. They work through several versions, until the report is genuinely useful.

AVA: During that back-and-forth, she asks the agent to keep the instructions up to date: which files to use, what each field means, how to calculate availability, and what to do when something is missing. She’s making the reasoning explicit as they improve the work.

## Capturing and testing the skill

ANDREW: Now Elena says, “Turn these instructions and this reporting process into a reusable skill.” The agent packages the method so she can invoke it again without rebuilding the conversation.

AVA: And now she tests the skill itself. Could it produce a good report without all the corrections she supplied during that original conversation?

ANDREW: She makes a small test set: several weeks of input files, the corresponding reports she has checked, and a few difficult cases. A missing reservations file. An unexpected return. A product with no available stock. She writes down what a good result should contain.

AVA: Then she invokes the skill on those inputs and compares the outputs. Are the numbers right? Are the important exceptions visible? Can she trace a conclusion back to the data? Does it flag missing information rather than invent an answer?

ANDREW: She repeats the same cases, too. One successful run doesn’t tell her whether it’s dependable. When a result is wrong, she updates the skill and runs the test set again, checking that the fix hasn’t broken something else.

AVA: She keeps a few cases separate from the ones used to improve the instructions. Those help show whether the skill handles a new situation. She records the results until she’s comfortable it consistently meets the quality standard of a good human report.

ANDREW: This is real work, and it belongs to Elena before she asks anyone else to rely on her skill. We’ll devote a future episode to running an AI evaluation on your own skill. For now, her test results are what give her confidence to take the next step.

## Sharing with a small team

AVA: Elena tells her desktop agent, “Convert this tested skill into a plugin.” She gives it a clear name, Inventory Report, and includes the input requirements, how to invoke it, and the limitations her testing uncovered.

ANDREW: That’s the move from a personal skill to something she can share through this process. The plugin might contain one skill, or a few related ones. Initially, it contains no connectors. We’re starting with the skills, keeping connector approval separate.

AVA: If Elena already has an approved inventory connector and her own authorized access, the skill could use that connection. A colleague would need their own access. The plugin doesn’t carry Elena’s credentials or give anyone new permissions. For this first pilot, they’re using files in a folder.

ANDREW: She finds three teammates who have the appropriate licenses and agree to test it. She enters their names in the sharing dialog. Then she meets with them, rather than just sending a link and hoping they figure it out.

AVA: She shows them how to add the plugin, find the reporting skill, and invoke it. They walk through the required files and what the output means. Then each person runs it with their own inputs and checks the result.

ANDREW: One teammate’s export uses a different column name. Another finds that the explanation of a shortage needs more context. Elena improves the skill, reruns her tests, and asks them to try again.

AVA: After several reporting cycles, the teammates are using it regularly. They can show the reports, describe the time saved, and confirm that the quality is useful for their work. Elena records that feedback and their sign-off. Now she has evidence to support wider distribution.

## Earning a place in the marketplace

ANDREW: In Claude, she opens the plugin and clicks “Publish to org.” In this workflow, publishing requires review. She submits it as available to install, with release notes and the pilot evidence. Where another platform needs a separate approval process, we’d establish the equivalent steps.

AVA: With Enterprise scanning enabled, the covered upload is automatically checked for malicious content. The administrator sees that result. Elena’s report tests still matter: the security scan doesn’t tell us whether the inventory calculations are correct.

ANDREW: The reviewer asks four questions. Did the automatic scan pass? Are colleagues actually using this and finding value? Does it duplicate something already in the catalog? And is the package and its intended use allowed under our policies?

AVA: Elena’s submission has answers. There are tested reports and feedback from the pilot. The reviewer checks comparable tools and the contents of this version, including the rule against bundled connectors. If something is missing, it goes back to Elena with a specific request.

ANDREW: In our story, it passes review. The administrator approves it for the marketplace. That makes it available to install; it doesn’t force the plugin onto everyone’s account.

AVA: We’d start with a human doing that review. As the review method improves, we could capture it in a skill and test it ourselves. The people running the process would be learning through the same steps as Elena.

## More people use it and Elena keeps improving it

ANDREW: A colleague in another team finds Inventory Report in the marketplace, reads what it does, and clicks “Add.” They bring their own inputs, invoke the skill, and check whether it helps them. Now the method can reach people Elena has never met.

AVA: And the package can travel across tools. Tim has tested the same exact plugin in Claude, ChatGPT, and Copilot Cowork. In this example, colleagues can use that same package in Claude or ChatGPT, and in Copilot Cowork if the organization launches it, through each platform’s approved process.

ANDREW: Meanwhile, Elena keeps improving her own copy. Suppose she adds a clearer explanation of slow-moving stock. She tests the revised skill, gets feedback, and submits a new version with a description of what changed.

AVA: That version goes through the review process again. The currently approved version remains in use until the replacement is approved. Wider distribution makes disciplined updates more important, because more people now depend on the result.

## From regular use to a managed agent

ANDREW: Some colleagues run the report only when they need it. Others decide to schedule it every Monday at eight. They choose that separately, after making sure the inputs will be available and the task handles missing or stale data sensibly.

AVA: If a scheduled run fails, somebody needs to know. Elena and the team decide who receives the alert and who maintains the instructions. They watch whether the workflow keeps producing useful results as the data changes.

ANDREW: Eventually, several teams depend on this report. It’s used repeatedly and delivers enough value to justify operating it as a shared workspace agent, inside a platform or on another approved cloud service.

AVA: They give that agent a supported home, approved access to its inputs, an owner, monitoring, and cost controls. It can run without depending on Elena’s desktop being open or her remembering to start it. Some schedules already run remotely; this step is about taking responsibility for a shared capability.

ANDREW: Elena’s original folder of files has led somewhere useful. But she didn’t begin by asking for an enterprise agent. She began with a report she understood, improved it with her desktop agent, captured the method, and tested it.

AVA: Then she taught a few colleagues to use it, earned their confidence, and brought evidence to the reviewer. Each handoff made the next one possible. Whether your own idea stays a personal skill or reaches that final stage, that’s a process you can start with the work on your desk today.
