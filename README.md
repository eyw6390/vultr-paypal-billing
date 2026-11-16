# Vultr PayPal: Can You Pay Without a Credit Card, Why Checkout Fails, and How to Top Up (Steps Plus Billing Rules Most Guides Skip)

Vultr accepts PayPal, and you don't need a card on file with Vultr to use it. Sign in to the Console, go to **Account → Make a Payment** under **BILLING**, select **PayPal**, pick a preset amount or click **Other** to type your own, then finish inside PayPal. Credit lands on your Vultr balance and gets drawn down as your servers run.

When it doesn't work, the cause is usually inside PayPal rather than at Vultr. PayPal won't activate a billing agreement with vultr.com unless your PayPal account has a backup funding source, meaning a credit card or a bank account already linked there. Add one in PayPal and the payment goes through.

What follows covers the full payment flow, the troubleshooting order that actually matches Vultr's own documentation, how PayPal compares with the other six ways to pay, the prices Vultr publishes for add-on services, and the billing rules that decide whether your prepaid balance lasts a month or a week.

> **Before you pay:** open PayPal first and confirm a card or bank account is linked as a backup funding source. Without it, the Vultr billing agreement can't activate no matter how many times you retry. Then fund the account from the Console: 👉 [Create a Vultr account and make your first PayPal payment](https://bit.ly/VuLtr).

## How to pay Vultr with PayPal, step by step

The path is short and it is the same one Vultr documents for credit cards and crypto.

1. Log in to the Vultr Console.
2. Open **Account**, then find **Make a Payment** under the **BILLING** heading.
3. Select **PayPal** as the payment method.
4. Choose one of the preset amounts, or click **Other** and enter a custom figure.
5. Complete the payment in the PayPal window that opens.

Two details are worth knowing before you start.

The first is that this is a top-up. You are adding credit to your Vultr account balance, and Vultr deducts hourly charges from that balance until it runs low. Vultr's payment documentation describes PayPal only through this manual route; there is no documented "link PayPal once and it charges every cycle" setup.

The second is that PayPal isn't the only wallet-style option in that menu. Alipay, UnionPay, BitPay crypto and wire transfer all sit in the same **Make a Payment** screen with the same amount picker, so if PayPal gives you trouble you can switch channels without touching your server configuration.

## Why can't I pay with my PayPal?

Vultr keeps a dedicated FAQ entry for this question, which tells you how often it comes up. The answer is one line: PayPal requires users to have a backup funding source, such as a credit card or a bank account on file, to activate billing agreements. The fix Vultr points to is to visit PayPal and review the payment methods linked to your account.

In practice that means checking three things inside PayPal, in this order:

- **A linked card or bank account.** A PayPal balance alone isn't enough for a billing agreement, even if the balance covers the amount.
- **The status of that funding source.** A card PayPal has flagged as expired, or a bank account that hasn't completed verification, won't serve as the backup.
- **Which account you're signed into.** Payments started from the Vultr Console open whichever PayPal session your browser holds.

There's a mirror-image problem that gets confused with this one. If your **credit card** was declined by Vultr, the card is the failing piece, not PayPal. Vultr's advice there is to contact your bank for the specific reason, since banks rarely pass details back through a failed transaction. Vultr then suggests attempting the transaction through PayPal or another supported payment method instead. PayPal is the fallback for a bad card, and a missing backup funding source is a separate problem inside PayPal.

One more PayPal-specific rule worth filing away: a valid credit card or PayPal account must be linked before you can register for services and qualify for promotions. If you plan to chase signup credit, PayPal counts toward that requirement.

## PayPal vs the other ways to pay Vultr

Vultr publishes the full list of accepted methods: Visa, Mastercard, American Express, Discover, JCB, BitPay (BTC, BCH, ETH, DOGE, PAX, BUSD, LTC, USDC, GUSD), Alipay, UnionPay and PayPal. Depending on where you are, PayPal itself can route through additional networks including Giropay and bank transfers.

| Method | What it needs | How the money arrives | Worth knowing |
| --- | --- | --- | --- |
| Credit or debit card | Card details and a billing address | Instant; can become the default and auto-charge each cycle | Linking a card triggers a small temporary authorization that expires on its own |
| PayPal | A PayPal account with a card or bank account on file | Manual top-up through Make a Payment | Extra networks such as Giropay available in some regions |
| BitPay | A crypto wallet | Manual top-up | Nine supported coins, from BTC and ETH to USDC and GUSD |
| Alipay / UnionPay | The respective account | Manual top-up | Same amount picker as PayPal |
| Wire transfer | Bank details | Typically 3–5 business days | Your account email must appear in the wire memo; open a ticket if funds haven't landed within seven business days |

The practical split comes down to automation. A saved card can be set as your default and charged automatically each billing cycle. Top-ups through PayPal, crypto or Alipay are manual by nature, which means the balance is finite and you decide when to refill it.

## What you'll pay: the prices Vultr publishes

Every server bills hourly, with a one-hour minimum, and accumulated charges are invoiced on the 1st of each month. Most instances cap at 672 billed hours per month; GPU servers and VX1 Cloud Compute use a 730-hour monthly model converted to the actual hours in the calendar month, so a 30-day month bills up to 720 hours and a 31-day month up to 744.

Per-location pricing for compute plans can differ, because network, hardware, labor and tax costs vary by region, and Vultr states that current data center pricing is always shown in the Control Panel. The add-on services below have fixed prices published in Vultr's own FAQ.

**Object Storage** — every tier includes 1,000 GB of file storage, free inbound transfer and 1,000 GB/month of outbound transfer. Additional outbound traffic costs $0.01/GB across the board.

| Tier | Monthly price | Extra storage | Get started |
| --- | --- | --- | --- |
| Standard | $18.00 | $0.018/GB | [ Deploy Standard object storage](https://bit.ly/VuLtr) |
| Premium | $36.00 | $0.036/GB | [ Deploy Premium object storage](https://bit.ly/VuLtr) |
| Performance | $50.00 | $0.050/GB | [ Deploy Performance object storage](https://bit.ly/VuLtr) |
| Accelerated | $100.00 | $0.100/GB | [ Deploy Accelerated object storage](https://bit.ly/VuLtr) |
| Archival | $6.00 | $0.006/GB | [ Deploy Archival object storage](https://bit.ly/VuLtr) |

**cPanel licenses** are billed separately from the instance, at a monthly rate that depends on how many accounts you need.

| Package | Accounts | $/month | Add to your account |
| --- | --- | --- | --- |
| Admin | Up to 5 | $31.99 | [ Add the Admin cPanel license](https://bit.ly/VuLtr) |
| Pro | Up to 30 | $45.99 | [ Add the Pro cPanel license](https://bit.ly/VuLtr) |
| Plus | Up to 50 | $55.99 | [ Add the Plus cPanel license](https://bit.ly/VuLtr) |
| Premier | Up to 100 | $63.99 | [ Add the Premier cPanel license](https://bit.ly/VuLtr) |
| Premier + Bulk | 100+ | $63.99 + $0.47 per extra account | [ Add the bulk cPanel license](https://bit.ly/VuLtr) |

## Billing rules that decide how long a PayPal top-up lasts

Prepaying changes your relationship with the invoice, but it doesn't change how Vultr counts usage. These are the rules most likely to catch someone who funded $20 through PayPal and expected it to sit there.

**A stopped instance still bills.** Shutting a server down doesn't stop the meter, because it keeps reserving RAM, SSD storage, IP aliases and vCPU. Charges continue until you use **DESTROY** in the customer portal. Stopped bare metal behaves the same way and needs to be released. A forgotten test server is the fastest way to watch a prepaid balance drain without deploying anything new.

**The newest payment method becomes the default.** When several methods are saved, the most recently added one is charged automatically each billing cycle and the older ones are marked as backups. You can delete a saved method from its **…** menu, but the default method cannot be removed. If you'd rather pay by hand, Vultr supports topping up in advance or when a funding notice arrives, and its system won't initiate an auto-payment in that case.

**Tax is added on top of the listed price.** Website prices exclude tax, which appears as a separate invoice line. Rates vary widely by jurisdiction: EU countries range from 17% to 27%, the UK sits at 20%, Japan 10%, Singapore 9%, India 18%, Canada 5% to 15% for services from Canadian data centers, and Texas charges 6.25% to 8.25% on 80% of the invoice. Your tax location normally follows your account address, which starts as the billing address of your primary payment method, and later changes apply only to future finalized invoices, never retroactively.

**Invoices are USD only.** Vultr uses USD as its functional currency and doesn't issue invoices in other currencies, deliberately, so pricing doesn't swing with exchange rates. Files come as CSV or PDF.

**Bandwidth doesn't roll over.** Each account gets 2 TB of free outbound transfer per month with no carryover, and instance bandwidth accrues hour by hour. Overages apply the moment your total outbound traffic passes what has been allocated so far, at $0.01/GB.

**Upgrades split across line items.** If you resize mid-cycle, each plan gets its own invoice line billed at its hourly rate for the time it was active. The line items may add up to more than 672 hours combined; the total never exceeds the real hours in the month.

If you want to see where your balance actually stands, it's on the same screen you used to pay: 👉 [Check your Vultr credit balance and billing settings](https://bit.ly/VuLtr).

## Promo codes: what PayPal users actually qualify for

Promo codes are redeemed in the **Gift Code** section of the customer portal, not at checkout. Vultr's conditions are specific: a valid credit card or PayPal must be linked to register for services and be eligible for promotions, it's one promo per user, and credits from promo codes expire.

The Vultr coupons page currently lists four new-customer offers, among them **FLY300VULTR** for $300 in free credit, **FLYTWOHUNDRED** for $200, **250VULTRFLY** for $250, and **VULTRMATCH**, which matches your first deposit dollar for dollar up to $100. Each carries the same fine print: promotional credit applies to select products only, can't be combined with other offers, and is limited to new customers. Treat the code page as the authority on eligibility and expiry rather than any summary, including this one.

That matters for the PayPal crowd in one concrete way. The requirement is a valid card **or** PayPal, so a PayPal account with a backup funding source satisfies the linking condition. Whether the credit covers the specific product family you want to run is a separate question answered only by the terms on the code page.

👉 [Check the current Vultr promo codes before you fund your account](https://www.vultr.com/coupons/?ref=9738262-9J).

## Quick answers

**Can I use Vultr with only PayPal and never add a card to Vultr?** Yes. Vultr's promotion rule accepts a card or PayPal, and the payment flow never forces you to store card details with Vultr. PayPal itself will still want a card or bank account on file as a backup funding source, so "no card anywhere" isn't achievable through this route.

**Can I pay an amount that isn't on the preset list?** Yes, click **Other** and type your own amount. Custom amounts are available for PayPal, crypto and Alipay alike.

**Why did a small charge show up when I linked a card?** It's a temporary authorization to validate the card, not a real charge. It typically expires within a few days depending on your bank's policy.

**Can I get an invoice in euros or pounds?** No. Invoices are issued in USD only, in CSV or PDF.

**My card works everywhere else but Vultr declines it. What now?** Ask your bank why the specific transaction failed, then retry through PayPal or one of the other supported methods, which is the alternative Vultr itself recommends.

**Do I need to destroy servers before I stop using them?** Yes, if you want billing to end. Stopped virtual machines and stopped bare metal servers keep incurring charges until destroyed or released.

## Which payment route fits you

If speed is the only thing that matters and you're comfortable storing the card, pay by credit card: it clears instantly, can be set as the default, and won't leave you manually refilling a balance.

If you'd rather not hand Vultr your card details, or your card lives in a country where the charge keeps getting flagged, PayPal is the better fit, provided the backup funding source is already in place at PayPal before you start.

If Vultr already declined your card, don't keep retrying it. Call the bank for the reason, then route the payment through PayPal or another supported channel.

Two things are worth checking before you place the order. Confirm the tax location and rate attached to your account, since it's added on top of the listed price and follows your billing address. Then look through your instance list for anything sitting in a stopped state, because that's the line item that quietly eats a prepaid balance.

👉 [Start on Vultr and fund your account with PayPal](https://bit.ly/VuLtr).
