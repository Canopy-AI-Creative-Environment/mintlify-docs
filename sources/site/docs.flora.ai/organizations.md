# Source: https://docs.flora.ai/organizations

For the complete documentation index, see [llms.txt](https://docs.flora.ai/llms.txt). This page is also available as [Markdown](https://docs.flora.ai/organizations/organizations.md).

> **Who this is for:** Organizations are for **Enterprise** customers who run **more than one workspace** under a single account — one bill, one seat pool, one shared usage pool. If you're on a self‑serve plan with a single workspace, nothing changes for you: see [Workspaces](https://docs.flora.ai/faqs-how-to.../workspaces). Org‑wide settings are managed by an **Admin**.

FLORA has two levels: your **organization** (the commercial account) and your **workspaces** (where work happens).

- **Organization** — billing, plan, seats, and the shared usage pool. It's the account you pay for.
 
- **Workspace** — projects, canvas, assets, folders, members, and API keys. It's where people actually create.
 

Every workspace belongs to exactly one organization. An Enterprise organization can hold **several workspaces**.

---

## 

How they relate

AskCopy

```
Your organization        ← billing, plan, seats, shared usage
  ├── Workspace A         ← projects, canvas, members
  ├── Workspace B
  └── Workspace C
```

Two kinds of membership decide what a person can do:

Membership

Answers

Carries

**Organization membership**

"Do they belong to the paid account, and what authority do they have?"

Role + a seat

**Workspace membership**

"Which workspaces can they enter?"

Workspace access

A person needs **both**: an organization membership to belong to the account, and a workspace membership for each workspace they should be able to open. Every member belongs to **at least one workspace** — there are no organization‑only members. Being an Admin does **not** automatically give access to every workspace — workspace access is always assigned explicitly.

---

## 

Getting around

There are two surfaces to know — one for **managing** your organization, one for **working** inside a workspace.

### 

Manage your organization and workspaces

Open **Settings** for everything administrative. It's grouped into two sections:

- **Organization**
 
 - **Members & Roles** — your people: the member list, roles, seats, and which workspaces each person can access. This is where you administer _who_ is in the account.
 
 - **Analytics** — usage across your organization.
 
 
- **Workspaces** — the workspaces in your organization. Use the **+** to create one, or select a workspace to manage its settings.
 

Plan and seats live under **Plans & Billing**; **Members & Roles** also shows your usage, wallet, and overage at a glance.

![Settings navigation showing the Organization section (Members & Roles, Analytics) and the Workspaces list](https://docs.flora.ai/~gitbook/image?url=https%3A%2F%2F526296967-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FWthH0GpcCHwVdtbvahZS%252Fuploads%252Fgit-blob-4bf1e2a4c5d11eaa949a8450617fddc6340f7312%252Forg-settings-nav.png%3Falt%3Dmedia&width=768&dpr=3&quality=100&sign=c6a71a37&sv=2)

Settings — manage your organization (Members & Roles, Analytics) and its workspaces

### 

Switch into a workspace to create

When you want to actually make something, use the **workspace switcher** at the top of the sidebar. It shows your organization and every workspace under it — use **Search Orgs & Workspaces** to filter, then click a workspace to jump in. A checkmark marks your current workspace, and your projects, canvas, and assets all live inside the selected one.

![Workspace switcher showing the organization with its workspaces nested underneath](https://docs.flora.ai/~gitbook/image?url=https%3A%2F%2F526296967-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FWthH0GpcCHwVdtbvahZS%252Fuploads%252Fgit-blob-91a8f1d9ca3620de378ffe80493c53300d146cf0%252Fworkspace-switcher.png%3Falt%3Dmedia&width=768&dpr=3&quality=100&sign=470ce835&sv=2)

The workspace switcher — jump into a workspace to start creating

---

## 

Roles

Roles are set at the **organization** level. A person has **one role** that applies across every workspace they belong to — you can't make someone an Admin in one workspace and a Member in another.

Role

What they can do

Uses a seat?

**Admin**

Manage members, roles, workspaces, and billing.

Yes

**Member**

Create and edit in the workspaces they're assigned to.

Yes

**Guest**

Limited, view‑and‑comment access in the workspace(s) they're added to.

No

- **Admin** authority is account‑wide, but an admin still needs to be assigned to a workspace to open it.
 
- **Guest** consumes **no seat**.
 
- Change a role from the **Role** dropdown on a member's row. It applies across **all** their workspaces.
 

![Role dropdown showing Admin, Member, and Guest](https://docs.flora.ai/~gitbook/image?url=https%3A%2F%2F526296967-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FWthH0GpcCHwVdtbvahZS%252Fuploads%252Fgit-blob-598dc36727579d4484e547983d60b5c38fcd8d9a%252Frole-dropdown.png%3Falt%3Dmedia&width=768&dpr=3&quality=100&sign=f32fa1fc&sv=2)

The Role dropdown — Admin, Member, or Guest

---

## 

Members & Roles

**Settings → Organization → Members & Roles** is where Admins manage everyone on the account.

At the top you'll see your organization name, member count, and seat count (for example, _5 seats — Unlimited_), plus three summaries:

- **Usage this period** — included usage used, the reset date, and overage used this period
 
- **Wallet** — your non‑expiring extra‑usage balance
 
- **Overage** — on‑demand spend accrued this period
 

![The Members & Roles page with organization usage, wallet, overage, and the member table](https://docs.flora.ai/~gitbook/image?url=https%3A%2F%2F526296967-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FWthH0GpcCHwVdtbvahZS%252Fuploads%252Fgit-blob-cbd4814d7e181a26a21e6415795543a628a28d12%252Fmembers-and-roles.png%3Falt%3Dmedia&width=768&dpr=3&quality=100&sign=4db93c3&sv=2)

Members & Roles — org usage at the top, members below

Below the summaries, every member appears in a table:

- **Person** — name and email
 
- **Role** — Admin, Member, or Guest (change it from the dropdown)
 
- **Usage (this month)** — that person's spend
 
- **Workspaces** — a chip for each workspace they can access; click the **×** on a chip to remove them from that workspace only
 

The **⋯** menu at the end of a row has **Remove from organization**, which removes the person from the account entirely (and frees their seat).

![Row actions menu with Remove from organization](https://docs.flora.ai/~gitbook/image?url=https%3A%2F%2F526296967-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FWthH0GpcCHwVdtbvahZS%252Fuploads%252Fgit-blob-67628a7851d5083a7b129d58926f4b44dec3f9be%252Fmember-remove-from-org.png%3Falt%3Dmedia&width=768&dpr=3&quality=100&sign=548b956f&sv=2)

The ⋯ menu — Remove from organization

---

## 

Add a member

Click **Add Member** on the Members & Roles page.

![Add member to organization modal with email, organization role, and workspace checkboxes](https://docs.flora.ai/~gitbook/image?url=https%3A%2F%2F526296967-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FWthH0GpcCHwVdtbvahZS%252Fuploads%252Fgit-blob-bfd9093e06f159cadae792547e0cb811328451f0%252Fadd-member-modal.png%3Falt%3Dmedia&width=768&dpr=3&quality=100&sign=85a91c96&sv=2)

Add member to organization

Fill in:

1. **Email** — their work email
 
2. **Organization role** — Admin, Member, or Guest
 
3. **Workspaces** — tick at least one
 

Every member must belong to **at least one workspace** — there are no members without a workspace. Click **Send invite**, and they'll get an email to join your organization and the workspace(s) you selected.

If the email already belongs to someone in your organization, adding them to more workspaces uses **no extra seat** and sends **no new invite** — they're simply assigned.

---

## 

Create a workspace

Under **Settings → Workspaces**, click the **+**. Enter a **Workspace name** and click **Create**.

![Create workspace modal with a name field and Create button](https://docs.flora.ai/~gitbook/image?url=https%3A%2F%2F526296967-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FWthH0GpcCHwVdtbvahZS%252Fuploads%252Fgit-blob-ea26094218926e8d2c28f96cba2d1cef97e93f33%252Fcreate-workspace.png%3Falt%3Dmedia&width=768&dpr=3&quality=100&sign=a001d144&sv=2)

Create a workspace inside your organization

The new workspace:

- Belongs to your organization
 
- Shares the org's plan, seats, and usage pool
 
- Does **not** create a separate bill
 

After creating it, add people by assigning workspaces on **Members & Roles**, or from the workspace's own **Members** page.

---

## 

Workspace settings

Open a workspace and go to its settings to manage that workspace on its own. Each workspace has:

- **General** — name, identification, icon, and more
 
- **Access & Permissions** — member access and model availability for this workspace
 
- **Members** — manage who belongs to this workspace
 
- **Usage** — this workspace's generation usage and export
 
- **Spend limit** — the maximum this workspace can draw from the shared org pool (see [Per‑workspace spend limits](https://docs.flora.ai/organizations/organizations#per-workspace-spend-limits))
 
- **API Keys** — API access for this workspace
 

![Workspace settings with General, Access & Permissions, Members, Usage, Spend limit, and API Keys](https://docs.flora.ai/~gitbook/image?url=https%3A%2F%2F526296967-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FWthH0GpcCHwVdtbvahZS%252Fuploads%252Fgit-blob-1c91ee1f13f51509773422c2ffdc993cc22f0cb3%252Fworkspace-settings.png%3Falt%3Dmedia&width=768&dpr=3&quality=100&sign=609335c&sv=2)

Per‑workspace settings

Removing someone from a workspace here doesn't free their seat if they're still in another workspace — seats are an organization‑level resource. To change someone's **role**, use **Members & Roles**; roles apply org‑wide, not per workspace.

---

## 

Seats

A **seat** is one person on the paid account with a billable role (Admin or Member). Seats are counted at the **organization** level.

- **One person = one seat**, no matter how many workspaces they're in.
 
- **Guests don't use a seat.**
 
- Adding someone who's **already in your org** to another workspace uses **no extra seat** (and sends no new invite).
 
- **Removing someone from one workspace** while they're still in another **does not** free a seat.
 
- **Removing someone from their last workspace** deactivates their org membership and **frees the seat**.
 
- **Removing someone from the organization** (the ⋯ menu on their row) frees the seat and removes all their workspace access.
 

Your seat count comes from your subscription. Plan and seats are managed under **Plans & Billing**.

---

## 

Billing and Usage

Your organization has:

- **One bill** — a single billing entity for the whole org. Adding a workspace does **not** create a separate bill.
 
- **One shared usage pool** — every workspace draws from the same balance.
 
- **One plan** — all workspaces in the org share the same plan and entitlements.
 

Generations always happen **inside a workspace**, but the cost is drawn from the **shared org pool**. Spend keeps the originating workspace attached for reporting, so you can still see which workspace used what.

Where to look:

- **Members & Roles** — usage this period, wallet, and overage at a glance.
 
- **Plans & Billing** — change your plan, manage seats, and open your Stripe billing portal.
 

### 

Per‑workspace spend limits

Because every workspace shares the organization's usage pool, you can cap how much any single workspace spends. Open the workspace's settings and, under **Usage & Limits → Spend limit**, set a dollar limit and choose a reset period — **All time** (no reset unless you change it) or **Per month** (resets every month). Use **Clear** to remove the limit. This keeps one workspace from drawing down the whole pool.

![Set a usage limit dialog with a dollar amount and a reset period of All time or Per month](https://docs.flora.ai/~gitbook/image?url=https%3A%2F%2F526296967-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FWthH0GpcCHwVdtbvahZS%252Fuploads%252Fgit-blob-7d15c051255b99a5e6d16f792bba250e56b916cb%252Fworkspace-spend-limit.png%3Falt%3Dmedia&width=768&dpr=3&quality=100&sign=f8fa4e01&sv=2)

Set a per‑workspace usage limit and reset period

For how on‑demand (overage) billing works, see the [pricing guide](https://docs.flora.ai/plans-and-billing/pricing).

---

## 

Analytics

**Settings → Organization → Analytics** aggregates usage across all your workspaces.

- **Aggregated across N workspaces** — shows which workspaces are included. Pick a date range (for example, _Last 30 days_) and **Export CSV**.
 
- **This period** — usage split by model type (Text, Image, Audio, Video) and Technique Runs.
 
- **Model Breakdown** — share and run count per model type; expand a row to drill into per‑workspace and per‑model detail.
 
- **Usage Trend** — daily usage across the period.
 

![Organization Analytics with model breakdown and usage trend aggregated across workspaces](https://docs.flora.ai/~gitbook/image?url=https%3A%2F%2F526296967-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FWthH0GpcCHwVdtbvahZS%252Fuploads%252Fgit-blob-ab0b04c14e20635212b9b1099d53cf092c215742%252Fanalytics.png%3Falt%3Dmedia&width=768&dpr=3&quality=100&sign=4182286d&sv=2)

Analytics — model breakdown and usage trend across all workspaces

> CSV reports are the reliable source of record. The on‑screen trend and teammate figures are aggregate estimates.

---

## 

Quick reference

I want to…

Do this

Invite someone new

**Members & Roles → Add Member** (email + role + workspaces)

Add an existing org member to another workspace

Assign them a workspace — no email, no extra seat

Change someone's role

**Role** dropdown on their row (applies org‑wide)

Remove from one workspace

Click the **×** on that workspace chip

Remove from the org / free a seat

**⋯ → Remove from organization**

Create a workspace

**Settings → Workspaces → +**

Change plan or seats

**Plans & Billing**

See usage

Top of **Members & Roles**

[PreviousManage Subscription](https://docs.flora.ai/plans-and-billing/manage-subscription) [NextWorkspaces](https://docs.flora.ai/faqs-how-to.../workspaces)

Last updated 6 days ago

Was this helpful?