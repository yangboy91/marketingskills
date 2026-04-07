# Reddit Marketing Strategy — Agent Playbook

## Core Principle

Reddit hates self-promotion. Reddit loves genuine value.
Strategy: give 10x value, mention the product 1x naturally. Never post a link in the original post. Never sound like an ad.

---

## Target Subreddits (Priority Order)

| Subreddit | Members | Strategy | Post Type |
|-----------|---------|----------|-----------|
| r/ClaudeAI | ~200k | Hottest leads — already use Claude | Tutorial posts, config tips |
| r/SideProject | ~180k | Builders who want to ship | Show-and-tell, process posts |
| r/IndieHackers | ~150k | Revenue-focused founders | Revenue milestones, lessons |
| r/artificial | ~1M | AI enthusiasts | Educational, thought leadership |
| r/passive_income | ~500k | Income seekers | Results posts, strategy |
| r/ChatGPT | ~5M | AI users ready to level up | Level up your AI angle |
| r/MachineLearning | ~3M | Technical — high credibility | Technical deep-dives only |

---

## Post Type 1: The Value Tutorial (r/ClaudeAI, r/artificial, r/ChatGPT)

Strategy: Teach something genuinely useful. No link in the post body.
When people ask "where can I learn more?" — answer in comments with link.

Template title: "I built an AGENT.md file that makes Claude Code run marketing tasks automatically — here is exactly how it works"

Template body:
The difference between Claude as a chatbot and Claude as an agent comes down to one file.

I have been running my marketing on autopilot using Claude Code plus a config file called AGENT.md. Here is the full setup:

What AGENT.md does — it gives Claude Code:
- An identity (who it is, what it is trying to accomplish)
- A schedule (what to do Monday, what to do Friday)
- A permission model (what it can do autonomously vs what needs approval)
- A memory pointer (where to store what it learned)

The Weekly Schedule section looks like this:

Monday: audit landing page, give me 3 improvements
Tuesday: write Reddit posts for review
Wednesday: batch social content
Friday: report what is working

I check in once a day for about 15 minutes. The rest runs.

Happy to answer questions on the setup — took me about an afternoon to get working.

---

When commenters ask "where is the guide?", reply:
"I actually wrote up the full system including the config files as a $29 guide at https://my-agent-guide.vercel.app — but honestly most of what you need is in this thread. Happy to keep answering questions here."

---

## Post Type 2: Build-in-Public Revenue Post (r/SideProject, r/IndieHackers)

Strategy: Share real numbers. The $0 dashboard is a feature, not a bug.
Transparency builds trust faster than success.

Template title: "I launched a $29 AI agent guide this week. Here is everything: traffic, revenue, what I am trying next."

Template body:
Product: Agent Playbook — a 60-page guide on building AI agents that generate income
URL: https://my-agent-guide.vercel.app
Revenue so far: $0

Not a humble brag. I just launched and I am posting this to hold myself accountable and document what actually works.

What I built: An AI agent that handles my marketing — Reddit posts, SEO content, social media. The guide teaches you how to build the same thing for your own product.

What is set up:
- Landing page (live, Stripe connected)
- Live revenue dashboard (public — you can see the $0 yourself)
- Email capture popup (going live today)
- 5-email nurture sequence

What I am testing first:
1. Reddit: value posts in r/ClaudeAI and r/SideProject
2. SEO: targeting "how to build AI agent" keywords
3. Build-in-public on X: documenting every week

Why I am sharing at $0: because every person who posts only after success gives a survivorship-biased view. I want to document the whole thing.

Will update in 2 weeks with real numbers. What would you test first if you were me?

---

## Post Type 3: Strategic Comment (daily, 15 min)

Find threads where your ICP is already asking your product's question.
Add the most useful comment in the thread. Mention the guide only if directly relevant.

Search queries to run daily:
- subreddit:ClaudeAI "agent" OR "automate" OR "passive income"
- subreddit:SideProject "AI" OR "automate" OR "marketing"
- subreddit:IndieHackers "AI agent" OR "automate marketing"
- subreddit:passive_income "AI" OR "automate"

Comment template when someone asks "how do I automate X with AI?":
The key thing most people miss is giving the AI an identity, not just a task.

When you just ask Claude to do a task, it forgets everything next session.
When you give it an AGENT.md file with a mission, memory pointers, and a schedule — it starts behaving like an employee instead of a tool.

For your specific case: [specific advice]
1. [Step 1]
2. [Step 2]
3. [Step 3]

This took me a while to figure out. Happy to share the config file structure if useful.

---

## Reddit Rules

1. Spend first 2 weeks commenting only — no posts until karma is above 50 in each sub
2. Never post your URL in the original post body
3. Always answer the question first, link second or not at all
4. Reply to every comment on your posts within 24 hours
5. Upvote genuinely useful posts in your target subs daily

---

## Weekly Reddit Schedule

| Day | Task |
|-----|------|
| Tuesday | Draft 1 value tutorial post + 3 strategic comments |
| Thursday | Draft 1 build-in-public update (alternates weekly) |
| Daily | Search for relevant threads, draft comment responses |

---

## Agent Command (run every Tuesday in Claude Code)

Read .agents/product-marketing-context.md, then use the social-content and copywriting skills.

Draft this week's Reddit content for Agent Playbook:

1. One value tutorial post for r/ClaudeAI — teach something genuinely useful about building AI agents or AGENT.md config files. No promotional language. Link only in comments if people ask.

2. Three strategic comments for threads in r/SideProject, r/IndieHackers, or r/artificial where people are asking about AI automation, passive income, or AI agents.

For each piece of content include:
- The exact text ready to copy-paste
- Which subreddit and why
- The specific value being provided
- What to watch for (upvotes, comments asking for more info)
