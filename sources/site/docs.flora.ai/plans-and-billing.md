# Source: https://docs.flora.ai/plans-and-billing

For the complete documentation index, see [llms.txt](https://docs.flora.ai/llms.txt). This page is also available as [Markdown](https://docs.flora.ai/plans-and-billing/pricing.md).

**Launch bonus extended through August 1, 2026.** Every paid plan gets extra usage during launch. See the [Launch Bonus](https://docs.flora.ai/plans-and-billing/launch-bonus) page for full details.

**Starter and above** include a monthly usage budget (denominated in dollars) for **text, image, video, audio, and other models** in the app. One usage bar. No per-generation math in the flow. Usage resets each month — it doesn't carry over.

The **Free** plan is for trying the canvas: **text and image models** only (no video models in the app), **limited complimentary generations** for exploration — not a monthly dollar allowance — plus **no FLORA API or MCP** (those start on **Starter**). See [flora.ai/pricing](https://flora.ai/pricing) for the current free-generation cap and footnotes.

## 

Plans

Plan

Price

Monthly usage per seat

Launch bonus

Total during launch

Max seats

Free

$0

—

—

—

1

Starter

$18/mo

$18

+$12

$30

8

Pro

$50/mo

$50

+$50

$100

8

Max

$200/mo

$200

+$100

$300

8

Enterprise

Custom

Custom

—

—

Custom

**Plan features compared.** The table above covers price, usage, and seats — for the full feature comparison (workspace controls, team features, support tiers, etc.), see [flora.ai/pricing](https://flora.ai/pricing).

Annual plans save 20% on **Starter, Pro, and Max**. Those plans share the same published per-generation rates for every model your plan can access in the app, and **Starter and above** include **API & MCP**. **Free** stays on **text and image** in the product, **explore-only generation limits**, and **no API or MCP**. FAUNA is free on every plan, always — it doesn't count against your budget.

## 

How Usage Works

**On paid plans,** your monthly budget is denominated in dollars. When you run a generation, the model's cost is deducted from your budget. You see a simple percentage bar in the header — by default, no dollar amounts in the generation flow, no per-generation math. If you'd rather see exact costs, toggle **Preferences → Show generation costs in dollars** to replace the flower meter with the per-run dollar amount on every model and Run button. See [Model Pricing](https://docs.flora.ai/plans-and-billing/model-pricing#show-exact-dollar-amounts).

**What counts as usage.** Any generation from an AI model — images, video, audio, text — based on the model's published cost. FAUNA messages and interactions don't count against your budget on any plan.

**Where to see your usage.** A live percentage bar lives in the app header. Open **Settings → People & Seats** and scroll to **Usage this period** to see included usage for the current billing cycle, how much is left, when your budget **resets**, and any overage for the period.

![Usage this period on People and Seats showing included usage, reset date, and overage](https://docs.flora.ai/~gitbook/image?url=https%3A%2F%2F526296967-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FWthH0GpcCHwVdtbvahZS%252Fuploads%252Fgit-blob-2bb1999bd056d6c6a79499bfe3bd07102acc90fd%252Fusage-this-period.png%3Falt%3Dmedia&width=768&dpr=3&quality=100&sign=5a2fca2f&sv=2)

People & Seats → Usage this period

**Usage History** (under **Plan & Usage**) shows exact dollar cost per generation, per project, and per member — useful for client billing or team budgets.

**Model costs.** A public model pricing page lists the rate for every model we support, so you can compare if you want to plan around a specific workflow.

## 

Teams

Every paid plan includes team collaboration, and each seat adds both cost and budget based on your plan's per-seat rates.

**Example (Pro plan):**

- Pro costs **$50 per seat/month**
 
- Pro includes **$50 usage per seat/month**
 
- So a 4-person Pro workspace = **4 x $50 = $200/month** and **4 x $50 = $200/month shared budget**
 

During the [launch bonus](https://docs.flora.ai/plans-and-billing/launch-bonus) (through August 1, 2026), that 4-person Pro workspace's shared budget doubles to **$400/month**.

Admins have control over how usage flows inside a workspace:

- **Pooled or per-user.** By default, everyone draws from the same shared pool. Admins can switch to per-user budgets at any time.
 
- **Per-member caps.** Set a dollar cap on any individual member to prevent one person from draining the pool. When a personal limit is set, that member's usage indicator in the app header shows their individual usage percentage (or "Limit reached" when the cap is hit) with a tooltip explaining the admin-set limit.
 

Self-serve plans go up to 8 seats. Beyond that, [Enterprise](https://docs.flora.ai/plans-and-billing/pricing#enterprise) gives you a custom seat count plus admin, security, and advanced features.

## 

Extra Usage (On-Demand Spending)

When your monthly budget runs out, you have two options: upgrade your plan, or turn on on-demand spending (called **Overage** in workspace settings).

On-demand is:

- **Opt-in.** Disabled by default. Workspace admins enable it in **Settings → People & Seats**.
 
- **Capped.** You set a **max overage** limit for the billing period so there are no runaway charges.
 
- **Card-required (self-serve).** A payment method must be on file. Enterprise accounts on invoice billing follow your contract instead.
 
- **Same price as included usage.** No markup — you pay the published model rates.
 

### 

Your max overage cap

The max overage setting is the most extra usage you allow **in the current billing period** — not just what is unpaid at the moment.

- Flora tracks **total overage this period** (everything above your included budget and wallet balance, whether or not it has been invoiced yet).
 
- When total overage would exceed your cap, **new generations stop** until the next billing period.
 
- When total overage **reaches** your cap, any remaining balance is **billed** and overage stops for the rest of the period.
 

If your cap is **lower** than your workspace's monthly subscription total, the cap controls both spending and billing. If your cap is **higher**, you can still be charged earlier when other thresholds are met (see below).

Paying an overage charge does **not** reset your cap for the period — only your subscription renewal starts a fresh overage tally.

### 

When self-serve workspaces are charged

For Starter, Pro, and Max workspaces paying by card, overage is **not** held until the end of the billing cycle. Charges happen when enough unpaid overage has built up:

1. **Max overage reached** — total overage this period hits the limit you set.
 
2. **Large unpaid balance** — unpaid overage reaches **$200** (a system safety threshold).
 
3. **Subscription-sized chunk** — unpaid overage reaches your workspace's **monthly subscription total** (plan price × editor seats; for annual billing, Flora uses the monthly equivalent). Example: one editor on Starter ($18/mo) is charged when about **$18** of overage is unpaid; four editors on Pro ($50 × 4 = $200/mo) is charged when about **$200** of overage is unpaid.
 
4. **Daily balance check** — if unpaid overage is still **more than $5** but has not hit the thresholds above, Flora attempts to collect it once per day (around 8:15 AM UTC).
 

You may see **multiple charges in one period** as you keep generating — especially when your max overage is higher than your subscription total. Each charge covers what was unpaid at that moment; your period total keeps counting toward your cap.

Charges appear on your card through Stripe. Open **People & Seats → Manage & Invoices** to view invoices and payment history.

If a subscription payment fails, **new overage charges pause** until billing is healthy again. Existing prepaid or wallet balance is not removed.

### 

Enterprise overage billing

Enterprise overage follows your contract. Most enterprise workspaces receive **invoices** (not automatic card charges) on a **monthly or quarterly** schedule tied to the contract start date, with payment terms set in your agreement (commonly net 60). The **People & Seats** overage settings show the next scheduled invoice date when invoice billing applies.

Some enterprise setups use the same threshold rules as self-serve, but still bill via invoice rather than an immediate card charge. Your account team can confirm which model applies to your workspace.

## 

Enterprise

For organizations that need a custom seat count, SSO, admin controls, audit logs, invoice billing, and the rest. Negotiated annually. [Contact us](https://flora.ai/contact) to start a conversation.

---

## 

Further Reading

- [Launch Bonus](https://docs.flora.ai/plans-and-billing/launch-bonus) — extra usage through August 1, 2026
 
- [Pricing FAQ](https://docs.flora.ai/plans-and-billing/faq) — common questions about plans, usage, and billing
 
- [Manage Subscription](https://docs.flora.ai/plans-and-billing/manage-subscription) — change, upgrade, or cancel your plan
 
- [flora.ai/pricing](https://flora.ai/pricing) — full feature comparison across plans
 

## 

Questions?

- General: [support@florafauna.ai](mailto:support@florafauna.ai)
 
- Enterprise: [flora.ai/contact](https://flora.ai/contact)
 

[PreviousAudio Models](https://docs.flora.ai/models/audio-models) [NextModel Pricing](https://docs.flora.ai/plans-and-billing/model-pricing)

Last updated 6 days ago

Was this helpful?