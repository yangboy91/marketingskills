# SETUP.md — Launch Your AI Marketing Agent in 45 Minutes

## What You Are Setting Up

An autonomous AI agent that handles marketing for Agent Playbook across 3 channels:
- Reddit: value posts + strategic comments in target subreddits
- - SEO: one blog post per week targeting buyer-intent keywords
  - - Social: X/Twitter build-in-public + LinkedIn thought leadership
   
    - Payment is already live (Stripe). This setup adds the email capture and content engine.
   
    - ---

    ## Prerequisites

    - Node.js installed (run: node -v to confirm)
    - - Claude Code installed: npm install -g @anthropic-ai/claude-code
      - - GitHub account (already have this)
        - - ConvertKit account, free up to 1000 subscribers: convertkit.com
         
          - ---

          ## Step 1 — Clone this repo locally (5 min)

          Open your terminal and run:

          git clone https://github.com/yangboy91/marketingskills.git
          cd marketingskills

          ---

          ## Step 2 — Install the marketingskills skills (5 min)

          npx skills add coreyhaines31/marketingskills

          This installs all skill files into .agents/skills/ and symlinks in .claude/skills/

          Confirm it worked: ls .agents/skills/
          You should see: page-cro, copywriting, email-sequence, seo-audit, social-content, and more.

          ---

          ## Step 3 — Set up email capture (15 min)

          1. Create a free ConvertKit account at convertkit.com
          2. 2. Create a Form and name it "Agent Starter Kit"
             3. 3. Note your Form ID from the URL in your browser
                4. 4. Go to Settings then API and copy your API Key
                   5. 5. Add the popup JS code to your index.html (see conversion/lead-magnet.md)
                      6. 6. Replace YOUR_FORM_ID and YOUR_API_KEY placeholders in the popup code
                         7. 7. Push to Vercel: git push
                           
                            8. Test: visit your site, trigger the popup, submit your own email, confirm you receive Email 1.
                           
                            9. ---
                           
                            10. ## Step 4 — Set up the email sequence in ConvertKit (10 min)
                           
                            11. 1. In ConvertKit, go to Automations then Sequences then New Sequence
                                2. 2. Name it: Agent Playbook Nurture
                                   3. 3. Copy all 5 emails from conversion/email-sequences.md into the sequence
                                      4. 4. Set delays: Email 1 immediate, Email 2 at 2 days, Email 3 at 4 days, Email 4 at 6 days, Email 5 at 8 days
                                         5. 5. Create an Automation: trigger = subscribes to Agent Starter Kit form, action = add to Agent Playbook Nurture sequence
                                           
                                            6. ---
                                           
                                            7. ## Step 5 — First run (5 min)
                                           
                                            8. Open Claude Code in this project folder:
                                           
                                            9. cd marketingskills
                                            10. claude
                                           
                                            11. Then paste this first command:
                                           
                                            12. Read AGENT.md and .agents/product-marketing-context.md. Tell me the 3 most important things to do this week to get the first sale, and what you need from me to get started.
                                           
                                            13. ---
                                           
                                            14. ## Step 6 — Daily operation (10-15 min per day)
                                           
                                            15. Open automation/commands.md every day and paste today's command into Claude Code.
                                           
                                            16. Monday: SEO blog post
                                            17. Tuesday: Reddit content
                                            18. Wednesday: Social media batch
                                            19. Thursday: Conversion review
                                            20. Friday: Weekly report
                                           
                                            21. Review what the agent produced. Publish what looks good. That is it.
                                           
                                            22. ---
                                           
                                            23. ## What Success Looks Like
                                           
                                            24. Week 1-2: Email capture live, first Reddit post published, first social content posted
                                            25. Week 3-4: First email subscribers, first SEO post live, Reddit karma building
                                            26. Month 2: 50+ subscribers, 4+ blog posts live, consistent social presence
                                            27. Month 3: First organic traffic from SEO, email converting, first sales
                                           
                                            28. ---
                                           
                                            29. ## Files Reference
                                           
                                            30. | File | Purpose |
                                            31. |------|---------|
                                            32. | AGENT.md | Agent identity, mission, permissions, weekly schedule |
                                            33. | .agents/product-marketing-context.md | Product info read by all skills |
                                            34. | .agents/memory.md | 3-layer memory — update after each session |
                                            35. | channels/reddit-strategy.md | Reddit subreddit targets, post templates, rules |
                                            36. | channels/seo-strategy.md | 12-week keyword and content calendar |
                                            37. | channels/social-strategy.md | X and LinkedIn post templates |
                                            38. | conversion/email-sequences.md | 5-email nurture sequence |
                                            39. | automation/commands.md | Daily copy-paste commands for Claude Code |
                                           
                                            40. ---
                                           
                                            41. ## Revenue Loop
                                           
                                            42. Organic traffic from Reddit, SEO, and Social
                                            43.   goes to Landing page at my-agent-guide.vercel.app
                                            44.     triggers Exit popup offering the free Agent Starter Kit
                                            45.   captures Email in ConvertKit
                                            46.     runs 5-email sequence over 8 days
                                            47.   converts to $29 purchase via Stripe
                                            48.     leads to Thank you page
                                            49.   cycle repeats with referrals and social sharing
