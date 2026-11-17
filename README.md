# Yearly VPS Deals: What $18–$54 a Year Buys, Why "Per Year" Can Mean Three Years, and When Annual Billing Beats Hourly

Yearly VPS deals in November 2026 sit in a $18–$54 band if you need 1–3 GB of RAM on a US-based KVM box, and about $40 buys 2 vCPU, 2 GB RAM and 40 GB of NVMe. Timing matters as much as specs right now: a 50%-off annual promotion that ran October 8–10 is closed, and the next big annual window (a European host's Black Friday sale) doesn't open until November 24.

So this is a waiting-and-checking month, not a buying-everything month. Below: how to convert a "per year" sticker into a real 12-month cost, the break-even rule for annual versus hourly, which limits only appear in the terms, and where RackNerd's annual KVM specials fit into the band.

> **Quick pick:** For most readers shopping with $20–$120 to spend, a RackNerd KVM special is the straightforward fit. Every plan is KVM with full root SSH, a 1 Gbps port, and the ctrl panel for reboots, OS reinstalls, an HTML5 VNC console and one-click apps. It's unmanaged, refunds are decided case by case with no default refund once payment clears, and RackNerd rotates its specials, so confirm the current plan names and prices on the live list. 👉 [See the current RackNerd annual VPS specials](https://bit.ly/RacKnerd)

## What RackNerd includes on every annual special

RackNerd's specials change names and prices often enough that quoting one here would risk sending you to a checkout page that no longer matches. The feature set is stable, though, and it's what you're actually comparing against other hosts.

| What you get | Detail |
| --- | --- |
| Virtualization | KVM, with dedicated resources and full root SSH access |
| Network | 1 Gbps port; you choose a datacenter at checkout for lower latency |
| Control panel | ctrl: reboot, OS reinstall, HTML5 VNC console, one-click apps, network firewall rules, root password reset, plan upgrades |
| Operating systems | CentOS, Rocky Linux, AlmaLinux, Fedora, Debian, Ubuntu; custom ISO on request via ticket |
| One-click apps | AdminBolt, OpenClaw, Hermes Agent, AnythingLLM, Ollama, LibreChat, n8n, Coolify, Docker with Portainer |
| Management | Unmanaged; 24/7 support covers the platform, not your stack |
| Refunds | Case by case; no default refund once payment is received |

The one-click app list quietly decides your plan size. OpenClaw wants at least 8 GB of RAM. Hermes Agent, AnythingLLM, Ollama and LibreChat want 4 GB or more. n8n and Coolify are comfortable from 2 GB. If you're buying a box to run a local LLM front end, the cheapest tier will not do it, no matter how good the price looks.

Everything else on the list, root access and custom ISOs included, means you can install whatever stack you want over SSH. That also means nobody will configure it for you. 👉 [Pick a plan size from the current specials list](https://bit.ly/RacKnerd)

## The per-year figure: check which period it's billed over

Three hosts, three different meanings for the same two words.

**A per-year price inside a multi-year commitment.** One host's performance VPS page lists a 48 GB / 720 GB NVMe / 12 vCPU plan at $246 down to $197 "Per Year", with a footnote on the same page stating those prices are for 3-year billing cycles. That $197 is an annual slice of a bill you pay up front for three years. The deal is real; the cash-flow number you need is roughly three times the figure you first read.

**A flat price with no intro discount.** LiteKeep publishes Keep 2 at $40 a year against $48 for twelve months of hourly billing on the same specs, and states plainly that it has no cheap first year: it renews at the yearly price on your order, and later list-price changes don't touch a year you've already paid for. What you see is what year two costs.

**A recurring discount with an expiry date.** A 50%-off annual code at another host was described as recurring and permanent for eligible yearly plans, taking an Asia 2 GB plan from $57.60 to $28.80 a year. The code window closed on October 10, 2026. Permanent discount, temporary door.

Before you compare two annual prices, label each one: multi-year commitment, flat renewal, or expiring recurring discount. Comparing across those categories is how people end up surprised in month thirteen.

## When annual billing actually beats hourly

LiteKeep publishes the cleanest version of the rule. Keep 2, 6 and 8 break even at 10 months of continuous hourly billing; Keep 16 and larger break even at 11. The reasoning is simple arithmetic: a year paid upfront costs the same as 10 or 11 months of hourly billing on the same machine, and the free months are where the saving comes from.

Run it on your own numbers. Take the hourly or monthly rate, multiply by the months you expect the box to be up, and compare with the annual price. If the project might die in six months, or you're still deciding between 2 GB and 4 GB, annual billing locks in the wrong answer. LiteKeep's own advice is to spin up the same specs hourly for a few cents first, then buy the year.

Hosts without hourly billing (most of the cheap US annual providers) don't give you that test. There, the annual price is the only price, and the decision is whether the specs are right, not whether the term is.

## Refunds, renewals, and where an annual plan traps you

Annual billing removes your leverage. Four documented examples:

- **LiteKeep:** a paid year is final; no refunds. It also doesn't support in-place upgrades, so outgrowing the plan means a new machine and a migration.
- **A European host's Black Friday sale:** annual orders placed with its discount code are explicitly non-refundable, and you get one location change within 24 hours, limited to participating locations.
- **SSDNodes:** 14-day money-back guarantee on new services, no free trial.
- **RackNerd:** refunds are handled case by case, and the default outcome once payment clears is no refund. Immediate cancellation starts a 24-hour termination countdown rather than returning money already paid; wallet credit isn't refundable; a chargeback filed against a service suspended for abuse can add a $125–$250 administrative fee.

Renewal behaviour differs just as much. LiteKeep emails seven days before renewal, bills from your balance, and if the balance is short it keeps the server running on hourly billing instead of taking it offline. Typical multi-year intro deals renew at a higher regular rate. Ask which model you're buying before you compare year-one prices.

RackNerd's no-default-refund stance makes the pre-purchase check more important than the price: confirm the datacenter, the OS and the RAM tier before you pay, because a change of mind afterwards is a support conversation, not a policy right. 👉 [Check the annual KVM specials currently listed](https://bit.ly/RacKnerd)

## Limits that only show up after you pay

These are the terms that decide whether a cheap annual box is usable for your workload.

**Banned applications.** SSDNodes prohibits any media-converting software (Plex is the named example), uploading or downloading copyrighted content, and all cryptocurrency applications including mining and mining pools. If your plan was a Plex server, that $197 a year is wasted.

**Metered extras.** LiteKeep pools traffic across the whole account, charges $2 per TB beyond the pool, bills a Windows licence at $4 a month, and adds VAT for EU customers. None of that is in the headline annual price.

**Ports and PTR.** A host that blocks port 25 can't send mail, whatever the spec sheet says. One provider here explicitly opens SMTP 25, 465 and 587 and offers rDNS/PTR, plus KVM with nested virtualization and both Linux and Windows. If you're running a mail server or need reverse DNS for deliverability, that line matters more than 2 GB of extra RAM.

## Where the yearly price band sits

No links, no codes. Just the verified numbers, so you can see what your budget buys before you commit to any host.

| Provider | Annual price | vCPU / RAM / storage | Bandwidth | Worth knowing |
| --- | --- | --- | --- | --- |
| Dewlance Starter | $18/yr | 1 / 1 GB / 40 GB NVMe | 1 TB @ 1 Gbps | US only, KVM, instant setup |
| Dewlance Premium | $36/yr | 1 / 2 GB / 80 GB NVMe | 2 TB @ 1 Gbps | Same platform, one tier up |
| Dewlance Enhanced | $45/yr | 2 / 2.5 GB / 100 GB NVMe | 2.5 TB @ 1 Gbps | First tier with 2 vCPU |
| LiteKeep Keep 2 | $40/yr | 2 / 2 GB / 40 GB NVMe | 1 TB pooled | 10 Gbps port, no refunds |
| LiteKeep Keep 8 | $120/yr | 8 / 8 GB / 160 GB NVMe | 3 TB pooled | Same terms, bigger box |
| OrangeVPS US 25 GB | $38.40/yr list | 1 / 2 GB / 25 GB NVMe | 2 TB | 50% promo ended Oct 10, 2026 |
| OrangeVPS Asia 40 GB | $115.20/yr list | 2 / 4 GB / 40 GB NVMe | 4 TB | SMTP ports open, rDNS available |

Two data points worth flagging. Dewlance states an average ticket response of 18 minutes 34 seconds and a 4.9/5 rating from 12 customers; twelve reviews is too small a sample to read as a reputation, whatever the score. And the $197–$276 figures on SSDNodes' deal page sit outside this table on purpose, because they're three-year prices.

## Which one fits your case

- **A single small site, a VPN endpoint, a bot, or monitoring:** the $18–$36 annual tier is enough. 1 GB RAM runs a lightweight stack; it does not run a control panel plus a database plus a mail server.
- **Docker with a few containers, n8n, or a 4 GB one-click app:** start at 4 GB. Buying 2 GB and swapping is a false economy at these prices.
- **Anything with a Plex-style media workload or crypto software:** skip SSDNodes entirely; the terms forbid it.
- **Mail hosting:** pick a host that documents open SMTP ports and PTR control.
- **Uncertain lifespan under ten months:** pay hourly or monthly. The annual discount only exists for machines that stay up.

## Before you pay, confirm three things

1. **The billing period behind the price.** Is that annual figure one year, or one year of a three-year term?
2. **The renewal price.** Flat at the order price, or a jump after year one?
3. **The refund position.** No refunds at all, a 14-day window on new services, or case-by-case? RackNerd's policy is the third kind, which means the decision is effectively final at checkout.

Add a fourth if you're technical: does the host open the ports you need and give you PTR control? A cheaper plan that can't send mail isn't cheaper.

If those four answers line up with what you're building, an annual KVM special at $20–$60 is one of the better-value purchases in hosting right now. 👉 [Start with RackNerd's current annual VPS specials and pick your datacenter](https://bit.ly/RacKnerd)

## FAQ

**How much cheaper is annual than monthly?**
At LiteKeep, two months free on Keep 2, 6 and 8 works out to about 17% off the hourly cost of the same machine; one month free on Keep 16 and up is about 8%. Deeper discounts exist, but they usually come attached to longer commitments or expiring promo codes.

**Will the price go up when it renews?**
Depends on the model. LiteKeep renews at the yearly price recorded on your order. Multi-year intro pricing typically renews higher. RackNerd's specials rotate, so treat any annual price as the price for that term and re-check before renewal.

**Can I get a refund on a yearly VPS?**
Often no. LiteKeep states annual payments are final, one host's Black Friday code makes orders non-refundable, SSDNodes offers 14 days on new services, and RackNerd decides case by case with no default refund. Test on a monthly or hourly plan first if you're unsure.

**What can $20 a year actually run?**
A 1 GB KVM box: a static or low-traffic WordPress site, a WireGuard endpoint, a monitoring agent, a small bot, a DNS resolver. Not a panel plus database plus mail stack, and not an app that wants 4 GB or 8 GB of RAM.
