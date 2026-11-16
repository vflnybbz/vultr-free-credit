# Vultr Free Credit: Is It $300 or $200, Do You Need a Card, and How Long Does It Actually Last? (Plus the Free Tier That Isn't a Coupon)

Vultr's largest publicly listed new-customer offer right now is **$300 in promotional credit** on the code FLY300VULTR. There are three other codes on the same page: 250VULTRFLY for $250, FLYTWOHUNDRED for $200, and VULTRMATCH, which matches your first deposit dollar for dollar up to $100. All four are new customers only, none of them can be combined with another offer, and the credit won't appear until you attach a valid payment method. The credit also expires, and that single detail decides how you should spend it.

Below: what each code is actually worth, how Vultr's promo credit differs from its separate Free Tier Program (different product, much smaller hardware), the full plan list with prices, and the arithmetic on how much of the $300 you can realistically burn before it lapses.

> **Quick picks**
> - **Testing a workload for a few weeks:** FLY300VULTR, and run the instance size you'd genuinely deploy in production.
> - **Planning to stay and deposit real money:** VULTRMATCH. Up to $100 matched, and its expiry terms are reported to be looser than the fixed-amount codes.
> - **Want a small server that stays free:** neither code. That's the Free Tier Program, which you apply for and may not get.
>
> 👉 [See every Vultr plan and its current price](https://www.vultr.com/pricing/?ref=9738262-9J)

## Two different free things at Vultr, and only one of them is a coupon

Promotional credit is a one-time balance dropped into a new account. It's limited to select products, it can't be combined with other offers, it requires a verified payment method, and it disappears on a set date. Every "$300 free credit" article you've read is about this.

The Free Tier Program is a separate Vultr project that hands out an actual free instance. The hardware is small and fixed: **1 vCPU, 512 MB RAM, 10 GB SSD, one IPv4 address**. It deploys from Cloud Compute > Regular > Free Instance, and only in three locations: **Miami, Seattle, and Frankfurt**.

Getting one isn't a signup step. You apply inside the console and describe who you are and what you intend to run. Vultr assigns each applicant a weighted score during identity and usage validation, then grants access on a randomized basis, so more detail about your project raises your odds without guaranteeing anything. The program is in early access, quantities are limited, and Vultr states plainly that it doesn't share its verification process, including when an account is rejected. Results arrive by email and in the console. There's no published timeline.

If your goal is a permanently free box to run a tiny service, the Free Tier Program is the only real option at Vultr, and it's a lottery rather than a coupon. If your goal is to test something substantial for a month, the promo credit is the tool, and the free instance's 512 MB won't run much anyway.

👉 [Read the Free Tier Program requirements and apply from the console](https://www.vultr.com/free-tier-program?ref=9738262-9J)

## Every Vultr plan, and what each one costs

Vultr bills hourly, with a monthly cap of 672 hours on Cloud Compute and Optimized Cloud Compute, so a server left running all month costs exactly the listed monthly price and no more. VX1 and GPU instances are **not** subject to that cap; you pay for every hour in the month.

| Plan family | Entry configuration | Price / month | Best for | Get it |
| --- | --- | --- | --- | --- |
| Cloud Compute, Regular Performance | 1 vCPU / 0.5 GB / 10 GB SSD | $2.50 (IPv6 only) or $3.50 with IPv4 | Hobby sites, dev and test | [Pick this plan](https://www.vultr.com/products/cloud-compute/?ref=9738262-9J) |
| Cloud Compute, High Performance (AMD or Intel) | 1 vCPU / 1 GB / 25 GB NVMe | $6.00 | Small apps that need NVMe speed | [Pick this plan](https://www.vultr.com/products/cloud-compute/?ref=9738262-9J) |
| Cloud Compute, High Frequency | 1 vCPU / 1 GB / 32 GB NVMe | from $6.00 (ten sizes, up to $320) | Game servers, single-core-heavy work | [Pick this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |
| VX1, dedicated vCPU | 2 vCPU / 8 GB / 120 GB NVMe | from about $43.80 | Production apps, databases, SaaS | [Pick this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |
| Optimized, General Purpose | 1 vCPU / 4 GB / 30 GB NVMe | $30.00 | Web and app servers, e-commerce | [Pick this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |
| Optimized, CPU Optimized | 1 vCPU / 2 GB / 25 GB NVMe | $28.00 | CI/CD, video encoding, batch jobs | [Pick this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |
| Optimized, Memory Optimized | 1 vCPU / 8 GB / 50 GB NVMe | $40.00 | MySQL, Redis, analytics | [Pick this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |
| Optimized, Storage Optimized | 1 vCPU / 8 GB / 150 GB NVMe | $75.00 | Cassandra, MongoDB, OLTP | [Pick this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |
| Cloud GPU, NVIDIA GH200 | 1 GPU / 72 vCPU / 480 GB RAM | $2,913 (36-month reserved) | AI training, large-scale HPC | [Check GPU options](https://www.vultr.com/pricing/?ref=9738262-9J) |

The Regular Performance ladder is where most cheap projects land: 1 GB for $5, 2 GB for $10, 4 GB for $20, each step adding vCPU count, disk and included transfer. Above that, High Performance moves to newer AMD or Intel CPUs with NVMe storage for roughly 20% more per size, and includes more transfer at every tier. A 1 GB Regular plan comes with about 1 TB of transfer, the 1 GB High Performance plan with 2 TB, and traffic beyond the allowance costs **$0.01/GB** worldwide.

VX1 is Vultr's dedicated-CPU line, and it scales in four published sizes:

| VX1 size | vCPU / RAM / NVMe | Included transfer | Price / month |
| --- | --- | --- | --- |
| Entry | 2 / 8 GB / 120 GB | 3 TB | about $43.80 |
| Standard | 4 / 16 GB / 240 GB | 5 TB | about $112 |
| Large | 8 / 32 GB / 480 GB | 8 TB | about $224 |
| XL | 16 / 64 GB / 960 GB | 12 TB | about $448 |

Beyond the compute line, Vultr offers bare metal servers, S3-compatible object storage, managed MySQL, PostgreSQL, Redis and Kafka, a free Kubernetes control plane, and network-wide DDoS protection. GPU capacity tops out at eight H100s at $13,432/month, with AMD MI355X and MI325X instances also available.

Three costs sit outside the sticker price and matter for a short trial: automatic backups add **20%** to the instance price, snapshots cost **$0.05 per GB per month**, and extra IPv4 addresses are billed separately. A powered-off server keeps billing until you destroy it.

## How far does $300 actually stretch in a 30-day window?

Fifty months of a $6 server is the arithmetic, and it's the number most articles stop at. The clock kills it first. Vultr's coupons page doesn't print an expiry date, but the fixed-amount codes are widely reported to run **30 days from issue**, and billing pages show the exact date right after activation.

So the $300 is a one-month testing budget, not months of free hosting. Run the numbers on what a month actually costs:

- A $6 High Performance instance running for the full 30 days uses about **$6** of the credit, or 2% of it.
- A $30 General Purpose box for the same month uses **$30**.
- To spend the whole $300 inside the window you'd need to average roughly **$10 a day**. That's a VX1 Large at $224 plus a couple of 4 GB instances, or a dedicated 8-vCPU machine running around the clock.
- A GH200 at $2,913/month works out to about **$4.33 per hour**, so $300 disappears in roughly 69 hours, under three days. An eight-way H100 node burns through it in about 15.

The practical conclusion: pick the instance size you'd really deploy after the trial, not the cheapest box on the list. Benchmarking a 512 MB server for a month tells you nothing about whether a 4 GB production plan fits, and it leaves $294 of a one-time credit unused.

You also get one shot at choosing. Vultr's terms state promotional credit **cannot be combined with any other offers**, and that applies across codes as well as across promotions. FLY300VULTR and VULTRMATCH can't both land on the same account, so decide before you sign up: $300 that expires in about a month, or a $100 match on money you were going to deposit anyway.

## Claiming the credit: the step that decides whether you get it

1. Open the signup page through a promotional link, since the offer is tied to it.
2. Register with a real address and click the verification email.
3. **Add a payment method.** This is where most attempts fail. A credit card, a debit card, or a $1 PayPal top-up triggers the credit; without one, the promo balance stays empty.
4. Enter the code under Billing → Promotions / Coupon Codes and apply it. If the balance doesn't appear automatically, paste FLY300VULTR or VULTRMATCH there manually.
5. Check the billing page. Promotional credit shows separately from real funds, and so does the expiry date. Note it.
6. Deploy. The balance starts draining as soon as the instance is live.

The whole flow takes about ten minutes with a card in hand. Expect a fraud check on a brand-new account; Vultr is known for asking for identity verification, and that's routine rather than a sign you've done something wrong.

👉 [Start a new Vultr account and attach a payment method](https://bit.ly/VuLtr)

## What happens when the credit runs out

Once the promotional balance hits zero, Vultr bills your saved payment method at normal hourly and monthly rates. With no payment method on file, instances get suspended. Vultr's own account documentation makes two recommendations worth following literally: monitor your credit balance in the billing section to avoid unexpected charges, and deprovision resources before your credits expire so you aren't billed extra.

Refunds aren't part of the deal. Vultr's terms treat payments as final and credit as non-refundable, which makes the promo balance your only free attempt. Deposit only what you're prepared to spend, and set a billing alert before the expiry date rather than after.

👉 [Check the current terms on Vultr's coupon page](https://www.vultr.com/coupons?ref=9738262-9J)

## How the offer compares with DigitalOcean and Linode

The headline number favors Vultr; the clock favors its main competitor.

| Provider | New-customer credit | Typical validity | Entry price |
| --- | --- | --- | --- |
| Vultr | $300 (FLY300VULTR) | about 30 days | $2.50/mo IPv6 only, $3.50 with IPv4 |
| DigitalOcean | $200 | often 60 days | $4/mo droplet |
| Akamai (Linode) | $100 | varies by promotion | historically $5 for 1 GB |

DigitalOcean's longer window suits someone who wants to watch a workload behave across two months of real traffic. Vultr's larger balance suits a compressed sprint: a migration rehearsal, a load test, a benchmark you want finished this month. Hetzner remains cheaper in Europe with far more included traffic, but its footprint is concentrated there rather than spread across Vultr's 32 locations on six continents.

## What users actually complain about

Aggregated reviews across G2, Capterra and Trustpilot, roughly 850 of them, average about **3.5 out of 5**. The positive ones point to fast deployment, transparent hourly billing and the number of regions. The low scores cluster on Trustpilot and center on account suspensions and refund disputes, which lines up with the payment-is-final policy above. On Reddit, the consistent view is that performance and uptime are solid for the price, with the recurring gripe being aggressive fraud detection that can freeze a new account pending ID checks.

None of that changes the math on the credit. It does mean you should keep the trial workload self-contained and avoid putting anything you can't rebuild onto a brand-new account in its first week.

## Which offer fits your situation

- **You want to benchmark Vultr against your current host:** FLY300VULTR, one instance at your real production size, torn down before the expiry date.
- **You've already decided to move and will deposit money:** VULTRMATCH. Up to $100 matched on a deposit you'd make anyway, with looser expiry terms than the fixed codes.
- **You want a small server that never costs anything:** apply to the Free Tier Program and keep your expectations at lottery level. 512 MB in Miami, Seattle or Frankfurt.
- **You're running an enterprise proof of concept:** skip the $300 entirely. Vultr handles qualified enterprise engagements through a separate track with credits running up to $100,000.

Two things to confirm before you click anything: that your payment method is attached and verified, and that you've read the actual expiry date on the billing page rather than trusting a number from an article. Then deploy the size you mean to keep.

👉 [Claim the $300 new-customer credit and pick your instance](https://bit.ly/VuLtr)
