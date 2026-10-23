# Enterprise AI News Studio — Episode 2: OpenAI Goes Enterprise
*Friday, October 23, 2026 · Hosts: Andrew (en-US-AndrewMultilingualNeural) and Ava (en-US-AvaMultilingualNeural)*

Sources:
- OpenAI, "OpenAI models are coming to Google Cloud" (Oct 21, 2026): https://openai.com/index/openai-models-google-cloud/
- OpenAI, "Build more responsive apps with the Decisions API" (Oct 22, 2026): https://openai.com/index/decisions-api/
- OpenAI, "Uber brings ChatGPT Work to all employees with OpenAI" (Oct 22, 2026): https://openai.com/index/uber-chatgpt-work-rollout
- TechCrunch (Oct 22, 2026): https://techcrunch.com/2026/10/22/uber-puts-all-30000-employees-on-chatgpt-work/
- OpenAI, "GPT-6 and Intelligent UI for everyone" (Oct 7, 2026): https://openai.com/index/gpt-6-for-everyone/
- Rumor: ArtificialWatch (Oct 19, 2026): https://artificialwatch.com/wire/gpt-6-1-terra-microsoft-eval-configs ; dotnet/efcore PR #39217; @LuminaBench, @steph_palazzolo (The Information, paywalled), @koltregaskes on X. Rumor items are attributed to the people who made them.

## Cold open
ANDREW: OpenAI models, sold through Google Cloud. A decision engine that costs ten cents per million tokens. And thirty thousand Uber employees with an AI agent at work. All in one week.
AVA: Welcome to Enterprise AI News Studio. This is episode two, OpenAI Goes Enterprise, for Friday, October twenty-third. I'm Ava.
ANDREW: And I'm Andrew. Confirmed news first, then the rumor mill, clearly labeled, and then what it all means if you buy AI for a company.

## Confirmed news
AVA: Story one. On October twenty-first, OpenAI announced that its frontier models and Codex are coming to Model Garden on Google Cloud.
ANDREW: The key detail for enterprises: purchases go through the Google Cloud Marketplace, so companies with Google Cloud spending commitments can draw those down to pay for OpenAI models.
AVA: OpenAI says its models will also soon be available in Google Antigravity and the Gemini Agent. General availability is planned in the coming weeks.
ANDREW: And OpenAI adds that Microsoft remains its primary cloud partner.
AVA: Sound familiar? In episode one, we covered the full Claude Platform arriving on Google Cloud on October twenty-second. So in the same week, both OpenAI and Anthropic moved deeper into Google's cloud.
ANDREW: Story two. On October twenty-second, OpenAI made the Decisions API generally available. It's built on GPT-6 Luna, and it's designed for small, bounded decisions. Think classify an input, route a request, or score something against a rubric.
AVA: OpenAI says it's up to ten times faster than running GPT-6 Luna through the regular Responses API. You can ask up to four hundred questions in a single request, which is double the old limit.
ANDREW: And the pricing is unusual. Ten cents per million input tokens, one cent per million for cached input, and no charge at all for output tokens.
AVA: Processing can stay in the US or the EU.
ANDREW: Story three, also October twenty-second. Uber is rolling out ChatGPT Work, OpenAI's agent inside ChatGPT Enterprise, to more than thirty thousand employees, after a pilot with one thousand people.
AVA: It connects to tools like Google Drive, Gmail, Calendar, and Slack, and the default model is GPT-6.1 Sol. What wasn't disclosed: the cost, or any savings numbers. The companies say they'll share results as the rollout goes.
ANDREW: And a bit of background. On October seventh, OpenAI started rolling out GPT-6 with Intelligent UI to every ChatGPT tier. That means answers built from charts, buttons, and forms, not just text.
AVA: For Enterprise customers, availability depends on admin settings.

## The rumor mill (unconfirmed)
ANDREW: Time to switch hats. Everything in this segment is unconfirmed. OpenAI has not announced a model called GPT-6.1 Terra.
AVA: Here's the trail. A Microsoft code change in the dotnet E F Core project, pull request three nine two one seven, was merged on October sixteenth. It switched test settings to use a model called G P T six point one Terra as a judge.
ANDREW: The account at LuminaBench spotted it on X, and ArtificialWatch reported on it. Their own caveat is worth repeating: a name in a config file is not a launch. It says nothing about price or date.
AVA: Then Stephanie Palazzolo of The Information said on X that the newsletter has news on "a potential new Terra model" from OpenAI. That article is paywalled.
ANDREW: And X accounts citing The Information, for example at koltregaskes on October twentieth, say Terra, Gemini 4 Carbon, and Fable 5.5 are all due in November. That's secondhand reporting on a paywalled story, so treat it as a maybe.

## What it means for enterprise buyers (analysis)
ANDREW: Okay, now some analysis. This is our take, not news.
AVA: First, multi-cloud procurement. If you can pay for OpenAI and Claude out of an existing Google Cloud commitment, the question shifts from which cloud has which model, to which budget you want to spend from.
ANDREW: Second, cheap, high-volume decisions. With no output charge and ten-cent input, routing and triage steps that used to be too expensive at scale may now be worth testing. Run your own evals before trusting the speed claims.
AVA: Third, org-wide rollouts. Uber went from a thousand-person pilot to the whole company. The thing to watch is whether they publish real outcomes, because that's the number every other buyer will want.

## Sign-off
ANDREW: That's OpenAI Goes Enterprise. Confirmed news stays confirmed, rumors stay labeled.
AVA: Thanks for listening to Enterprise AI News Studio. See you next episode.
