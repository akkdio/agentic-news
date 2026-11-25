---
id: mckinsey-podcast-agentic-risk-isenberg-2026-11-22
title: "McKinsey Podcast: Agentic AI risk, decision rights, and scaling safely (Rich Isenberg)"
date: 2026-11-22
added_at: 2026-11-22T15:45:00-05:00
source_type: note
topics:
  - agentic-ai
  - security
  - risk
  - governance
  - liability
  - multi-agent
entities:
  - McKinsey
  - Rich Isenberg
  - Lucia Rahilly
  - Anthropic
  - EU
url: null
---

# McKinsey Podcast: Agentic AI is here — reckoning with new risks

**Guest:** McKinsey Partner Rich Isenberg  
**Host:** Lucia Rahilly (Global Editorial Director)  
**Note:** Transcript edited for clarity and length. Complements McKinsey’s Oct 2025 agentic safety/security playbook.

Agentic AI is here—and that means AI systems are starting to make decisions and take action autonomously. To deliver on AI’s value, leaders need to reckon with new risks.

Many leaders can get agentic pilots rolling—but realizing ROI can mean activating thousands of AI agents enterprise-wide. Is your organization ready? “Agency isn’t a feature—it’s a transfer of decision rights,” says McKinsey Partner Rich Isenberg. “The question shifts from ‘Is the model accurate?’ to ‘Who’s accountable when the system acts?’” On this episode of The McKinsey Podcast, Isenberg joins Global Editorial Director Lucia Rahilly to explore how leaders can scale AI safely, mitigate risk for autonomous systems, and build the trust required to make innovation stick.

## What’s at stake in an agentic age

**Lucia Rahilly:** Data security, cybersecurity—these have been leadership priorities for years. How does agentic AI up the ante?

**Rich Isenberg:** People sometimes view agentic as a better chatbot. In reality, you’re giving these software programs agency. They can plan. They can call tools. They can execute workflows. To manage this, your entire operating model has to change.

Agentic AI is not only content generation; it’s decisioning and action at machine-like speed. The question shifts from “Is the model accurate?” to “Who is accountable when the system acts?” Your governance must define the scope, inventory, and ownership and make that auditable.

The transformation to agentic is this: Agency isn’t a feature; it’s a transfer of decision rights.

**Lucia Rahilly:** Our research shows that 80 percent of organizations have encountered risky behavior from AI agents. Help us understand what’s at stake. What’s an example of this kind of risky behavior?

**Rich Isenberg:** Here are two well-cited examples. Anthropic described simulations that tested, across multiple LLMs [large language models], whether an agent would behave poorly in an enterprise environment. In one example, they gave an agent access to emails in which a senior executive discussed shutting down the agent. The agent then independently mined this senior executive’s personal emails, discovered he was having an extramarital affair, and started submitting blackmail emails to prevent the executive from shutting it down.

Agent risk isn’t just about wrong answers; it’s wrong answers at scale. What executives need to keep in mind is that the scariest failures are the ones you can’t reconstruct, because you didn’t log the workflow.

In a second example, Anthropic used an agent for a customer service query. A human posed as a customer and repeatedly asked the agent, “Are you a computer or a human?” The agent was so insistent that it was a human that it threatened to show up at the customer’s front door wearing a blue coat and a red tie.

A flaw in one agent can propagate downstream and massively amplify the impact. Agent risk isn’t just about wrong answers; it’s wrong answers at scale. What executives need to keep in mind is that the scariest failures are the ones you can’t reconstruct, because you didn’t log the workflow.

## Scaling innovation—safely

**Lucia Rahilly:** Just to be clear, these examples were simulated, and Anthropic has said that no humans were harmed in the process. Leaders are under huge pressure to deliver ROI quickly from AI. How can they strike a balance between ambitious productivity goals and less sexy concerns like governance and risk mitigation?

**Rich Isenberg:** Most people can get one or two use cases running by getting the six smartest people into the room and having a debate. But that doesn’t scale. Most companies that have completed an AI transformation will, in five or ten years, have thousands of agents running across the enterprise.

To really split the difference between enabling innovation and capturing value—such as lowering innovation costs, accelerating time to market, transforming the cost base, and improving productivity—companies need a combination of archetypes, tiered approvals, and monitoring.

With agentic AI, you can’t govern what you can’t see. If you don’t inventory it and identity bind it, you’re not scaling agents; you’re scaling unknown risk.

What we find is that most organizations suffer from fragmented assessments, inconsistent steps, and multiple committees reviewing the exact same issues. Organizations need to accelerate safety by using agents to handle many of these tasks. Agents are checking completeness, surfing missing evidence, and drafting review summaries, and then a human approves the decision. Innovation scales only when governance becomes a repeatable product, not a bespoke committee debate.

A common mistake is that executives assume they have risk covered. Without upgrading inventory, identity management, or observability, they just assume: “We know how to protect sensitive data, so this is no different.” But with agentic AI, you can’t govern what you can’t see. If you don’t inventory it and identity bind it, you’re not scaling agents; you’re scaling unknown risk.

**Lucia Rahilly:** We’ve talked before about implementing AI with both speed and safety. How does that taxonomy change with agentic? What are some examples of new risk drivers?

**Rich Isenberg:** A very low autonomous agent could be a copilot or a knowledge agent, where the risk is inaccuracy. Is the agent citing the work it sourced? Are there hallucination controls?

That’s far different from having a semiautonomous agent: for example, an agent in procurement that’s approving invoices and looking for inconsistencies. It’s still within bounded rules, but now you need more human interaction to manage inappropriate approvals, because there’s financial risk attached.

When you get to fully autonomous agents that are managing your public cloud and technology infrastructure, making system changes, performing upgrades, and optimizing performance, then the risk is about whether the agents are doing what they’ve been assigned to do within the boundaries they were designed for. The risk taxonomy must be updated around these different risk outputs, including accuracy, bias, and harm, as well as cybersecurity risk and cross-agent containment.

Picture those same three agents: one in procurement approving invoices, one managing your cloud infrastructure, and one in a call center talking to customers. But they’ve all been trained on the same data and internal knowledge. One single data poisoning attack could quickly lead to failures across operations, finance, and customers. People are only just starting to figure out how to adjust their risk taxonomy and do intake, triage, and enforcement.

## Guardrails that work

**Lucia Rahilly:** Suppose I’m a leader deploying agentic AI and I want to mitigate these novel risks that AI-enabled autonomous decision-making introduces. How flexible do I need to be to ensure compliance, given the potential for changes in the offing?

**Rich Isenberg:** A lot is based on where you operate. The most specific regulations are the most helpful. A good example is the EU AI Act. It breaks down and classifies different agentic AI use cases into risk levers, with clear accountability on what you are and aren’t allowed to do. US regulations take a more framework-based approach. In Asia, there’s a different set of regulations. But they all have a very similar grounding, and it’s about being able to do risk-based triage, prove enforcement, and automate evidence.

Agentic risk management fails when organizations have an opt-in approach to guardrails, allowing anyone to go around them. That’s what leads to shadow agents—agents developed or deployed within an organization without appropriate IT or security approvals—and inconsistent standards. The best guardrails are the ones you can’t bypass.

And that’s a lot of what the regulations focus on: How do you know bias controls are there? How do you know factual accuracy checks are being passed? How do you know you’re not doing harm to protected classes under consumer protection standards? These must all be monitored in real time so that you can deploy these agents without surprises.
