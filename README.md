# bright data pricing: compare proxy costs, bandwidth limits, and a fixed-price ISP alternative

“Bright Data pricing” can mean very different things depending on what you are buying. A rotating residential proxy is billed by gigabyte. Static ISP and datacenter proxies are billed per IP. Web Unlocker and SERP API are billed per successful request. Put those models in one mental bucket and the invoice gets confusing fast.

The practical question is simpler: **what are you trying to run, how much traffic will it create, and do you need global rotation or stable U.S. IPs?**

Bright Data is built as a broad data-collection platform. It offers residential, ISP, datacenter, and mobile proxy networks alongside scraping APIs and browser products. That breadth is useful when a project needs granular targeting across many regions or several data-collection tools under one account.

But a wide platform is not automatically the lowest-cost choice for every workload. If the job is U.S.-focused and needs long-lived static residential IPs, it is worth comparing Bright Data’s per-IP plans and fair-use terms with an ISP-only provider such as HypeProxies.

This guide breaks down the current public Bright Data pricing structure, explains what the numbers actually cover, and shows where HypeProxies may make more financial sense.

## Bright Data pricing at a glance

Bright Data’s public pricing is organized around product type rather than a single subscription. That is sensible, but it means the lowest advertised rate may not apply to the proxy type you need.

| Bright Data product | Current public entry pricing | Billing model | Best fit |
| --- | ---: | --- | --- |
| Residential proxies | $4/GB with the displayed RESIGB50 promotion; regular listed rate $8/GB | Traffic usage | Rotating residential traffic and detailed geo-targeting |
| Residential monthly commitment | $499/month for 141 GB; promotional displayed rate $3.50/GB | Monthly commitment | Predictable residential-proxy usage |
| ISP proxies, shared pool | $18/month for 10 IPs ($1.80/IP) | Per IP, monthly | Static residential IPs with broader location options |
| ISP proxies, dedicated pool | $35/month for 10 IPs ($3.50/IP) | Per IP, monthly | Exclusive static ISP IPs |
| Datacenter proxies | $14/month for 10 IPs ($1.40/IP) | Per IP, monthly | Lower-cost server-based proxy traffic |
| Web Unlocker | Free tier: 5,000 requests; then $1.50 per 1,000 successful requests | Per successful request | Teams that prefer an API over proxy management |
| SERP API | Free tier: 5,000 requests; then $1.50 per 1,000 requests | Per request | Search-result monitoring and localized SERP collection |

The big distinction is between **metered traffic** and **per-IP pricing**.

A $4-per-GB residential plan can be inexpensive for a brief or low-volume task. At sustained volume, however, bandwidth becomes the primary cost driver. Per-IP pricing is easier to forecast when each proxy can carry the required traffic without triggering a fair-use threshold or an overage.

> Bright Data’s displayed “unlimited” static ISP and datacenter proxy plans include a 100 GB fair-use allowance per IP per month. Check expected transfer volume, not just the monthly price per IP.

## Bright Data residential proxy pricing: flexible, but watch the minimum commitments

Bright Data’s rotating residential proxies are the part of the catalog most people mean when they search for Bright Data pricing. The network is designed for projects that need rotating IP addresses and location selection at country, state, city, ZIP-code, or ASN level.

The currently displayed residential plans are:

| Plan | Included traffic / rate | Price and billing |
| --- | ---: | ---: |
| Pay As You Go | $4/GB shown with promotion; $8/GB listed regular rate | No commitment |
| Monthly tier 1 | 141 GB at $3.50/GB shown with promotion; $7/GB listed regular rate | $499 billed monthly |
| Monthly tier 2 | 332 GB at $3/GB shown with promotion; $6/GB listed regular rate | $999 billed monthly |
| Monthly tier 3 | 798 GB at $2.50/GB shown with promotion; $5/GB listed regular rate | $1,999 billed monthly |
| Enterprise | Custom traffic and rate | Contact sales |

The displayed code is **RESIGB50**, which Bright Data says provides 50% off residential proxies for three months. Treat it as a time-limited checkout promotion, not as the permanent unit price for a long-term budget.

The pay-as-you-go route is the cleanest way to test whether a residential network works for a legitimate data-collection use case. There is no monthly commitment, so a small project does not need to start at $499.

The commitment tiers make more sense when monthly traffic is genuinely predictable. At that point, the lower per-GB price matters. The catch is that Bright Data states active monthly commitments do not roll unused value into the next billing month. If usage turns out lower than expected, the effective cost per GB rises quickly.

### What counts toward residential bandwidth?

Bandwidth is calculated from traffic moving both directions: request headers, request body, response headers, and response body. That sounds minor until a scraper starts downloading heavy pages, images, scripts, or large API responses.

Before choosing a residential tier, estimate:

1. Average response size after any filtering or blocking of nonessential assets.
2. Requests per day and expected peak periods.
3. Whether retries, redirects, and failed requests could add traffic.
4. Whether session persistence is required or rotation is acceptable.

A workload that sounds like “a few million requests” can be tiny or enormous in gigabytes. The average response payload decides which.

## Bright Data ISP proxy pricing: shared, dedicated, and usage-based options

ISP proxies are static residential IPs hosted on server infrastructure. They are useful when a workflow needs a stable address for an extended session rather than a constantly rotating exit IP.

Bright Data publicly displays three ways to buy ISP access: a shared pool, a dedicated pool, and traffic-based plans.

### Shared ISP pool

| IP quantity | Price per IP | Total monthly price |
| ---: | ---: | ---: |
| 10 | $1.80 | $18 |
| 100 | $1.45 | $145 |
| 500 | $1.40 | $700 |
| 1,000 | $1.30 | $1,300 |
| More than 1,000 | Custom | Custom |

### Dedicated ISP pool

| IP quantity | Price per IP | Total monthly price |
| ---: | ---: | ---: |
| 10 | $3.50 | $35 |
| 100 | $2.75 | $275 |
| 500 | $2.60 | $1,300 |
| 1,000 | $2.50 | $2,500 |
| More than 1,000 | Custom | Custom |

### ISP traffic-based plans

| Plan | Included traffic / rate | Monthly price |
| --- | ---: | ---: |
| Pay As You Go | $8/GB | No commitment |
| Commitment tier 1 | 71 GB at $7/GB | $499 |
| Commitment tier 2 | 166 GB at $6/GB | $999 |
| Commitment tier 3 | 399 GB at $5/GB | $1,999 |
| Enterprise | Custom | Custom |

For the per-IP plans, Bright Data says every IP has a **100 GB monthly fair-use allowance**. The allowance is pooled across the IPs in the purchase. Ten IPs therefore come with a total 1 TB allowance, which can be distributed across those ten IPs.

That pooling is useful if some IPs are busy and others are not. Still, it does not change the core budgeting issue: a high-throughput team can exceed the included allowance. Bright Data says additional charges may apply after the allowance is used.

If you need broad country coverage, city targeting, or static IPs in multiple regions, Bright Data’s ISP offering deserves serious consideration. If you only need U.S. static ISP proxies and each IP will transfer substantial traffic, the price per IP is only half the calculation.

## Bright Data datacenter proxy pricing

Datacenter proxies are usually the lowest-priced static option. Bright Data’s current public tiers are:

| IP quantity | Price per IP | Total monthly price |
| ---: | ---: | ---: |
| 10 | $1.40 | $14 |
| 100 | $1.00 | $100 |
| 500 | $0.95 | $475 |
| 1,000 | $0.90 | $900 |
| More than 1,000 | Custom | Custom |

These plans also display a 100 GB monthly fair-use allowance per IP. Datacenter IPs can be a sensible fit for permitted high-volume crawling of targets that do not require residential classification. They are not a drop-in replacement for static residential or mobile IPs when the target specifically expects those network types.

A cheap proxy that cannot handle the intended workflow is not cheap. It is just a very efficient way to burn an afternoon.

## Bright Data Web Unlocker and SERP API prices

Bright Data also sells managed APIs, which changes the cost model entirely.

### Web Unlocker

The current public Web Unlocker options include:

- **Free tier:** 5,000 requests per month.
- **Pay as you go:** $1.50 per 1,000 successful requests.
- **Scale:** $499 per month, including 383,000 requests; additional requests are $1.30 per 1,000.
- **Enterprise:** custom quote.

The service includes proxy management, rendering, automatic retries, and CAPTCHA handling. It is generally easier to operate than maintaining a proxy pool, but the relevant unit is successful requests, not IP count or gigabytes.

### SERP API

The public SERP API structure is similar:

- **Free tier:** 5,000 records per month.
- **Pay as you go:** $1.50 per 1,000 requests.
- **Scale:** $499 per month, including 380,000 requests; additional requests are $1.30 per 1,000.
- **Enterprise:** custom quote.

For both products, Bright Data’s general free tier uses a shared 5,000-credit monthly allocation across eligible API products. Proxy networks are not covered by that monthly free-credit allowance, though Bright Data states that new accounts can receive separate proxy trial credit.

## Where Bright Data is worth the money

Bright Data is not simply “expensive” or “cheap.” It is broad, configurable, and priced accordingly. It is a sensible candidate when your project needs one or more of these things:

- Rotating residential IPs across many countries.
- State, city, ZIP-code, or ASN targeting for residential traffic.
- Static ISP IPs outside the United States.
- Managed data-collection APIs instead of a raw proxy endpoint.
- Browser automation or scraping products in the same platform.
- A small pay-as-you-go starting point before traffic volume is known.
- A compliance process that suits an established business workflow.

Residential and mobile proxy users should also expect a compliance review. Bright Data states that access to its residential and mobile networks may require KYC verification, potentially including a short video call and verification of business or personal information.

That process may be entirely appropriate for a company with a legitimate, documented use case. It may also be more overhead than a small U.S.-only project needs.

## When a fixed-price ISP alternative is easier to budget

HypeProxies is the relevant alternative here because its publicly listed ISP plans use a different model: **fixed per-IP pricing with unlimited bandwidth**, rather than a listed 100 GB fair-use allowance per IP.

The service focuses on static residential ISP proxies, with U.S. locations, 10 Gbps infrastructure, unlimited threads, and 24/7 support. It is not positioned as a replacement for Bright Data’s global rotating residential network, mobile network, or managed APIs.

It can be a practical alternative when the requirement is narrower:

- Static U.S. residential-classified IPs.
- Long-lived sessions that benefit from a consistent IP address.
- High bandwidth per IP.
- A known monthly IP requirement.
- A preference for quarterly billing when the project is stable.

Here are **all publicly displayed HypeProxies ISP proxy packages** in the current ISP store category.

| HypeProxies package | Core configuration | Price | Billing period | Purchase |
| --- | --- | ---: | --- | --- |
| 50 ISP Proxies | 50 U.S. static residential ISP proxies; unlimited bandwidth; 10 Gbps network | $65 | Monthly | [ Choose 50 monthly ISP proxies](https://bit.ly/Hypeproxies) |
| 50 ISP Proxies (Quarterly) | 50 U.S. static residential ISP proxies; unlimited bandwidth; 10 Gbps network | $175 | Quarterly | [ Choose 50 quarterly ISP proxies](https://bit.ly/Hypeproxies) |
| 100 ISP Proxies | 100 U.S. static residential ISP proxies; unlimited bandwidth; 10 Gbps network | $125 | Monthly | [ Choose 100 monthly ISP proxies](https://bit.ly/Hypeproxies) |
| 100 ISP Proxies (Quarterly) | 100 U.S. static residential ISP proxies; unlimited bandwidth; 10 Gbps network | $336 | Quarterly | [ Choose 100 quarterly ISP proxies](https://bit.ly/Hypeproxies) |
| /24 (254) ISP Proxy Subnet | 254 U.S. static residential IPs in a /24 subnet; unlimited bandwidth; 10 Gbps network | $300 | Monthly | [ Choose a monthly /24 ISP subnet](https://bit.ly/Hypeproxies) |
| /24 (254) ISP Proxy Subnet (Quarterly) | 254 U.S. static residential IPs in a /24 subnet; unlimited bandwidth; 10 Gbps network | $810 | Quarterly | [ Choose a quarterly /24 ISP subnet](https://bit.ly/Hypeproxies) |

The monthly rates work out to roughly $1.30 per IP for 50 proxies, $1.25 per IP for 100 proxies, and about $1.18 per IP for the 254-IP subnet. Quarterly billing lowers the effective monthly price further.

[👉 Check current HypeProxies ISP availability and plan options](https://bit.ly/Hypeproxies)

## Bright Data vs. HypeProxies: the decision is mostly about scope and traffic

| Decision factor | Bright Data | HypeProxies |
| --- | --- | --- |
| Primary strength | Broad proxy and data-collection platform | U.S.-focused static ISP proxy plans |
| Residential rotation | Yes | Static ISP plans are the relevant offering here |
| Global targeting | Extensive, including country, city, ZIP, and ASN options on supported networks | U.S. static ISP focus |
| Static ISP pricing | Shared pool from $1.80/IP; dedicated pool from $3.50/IP for 10 IPs | From $1.30/IP on the 50-IP monthly plan |
| Bandwidth model for static IP plans | 100 GB per IP monthly fair-use allowance; additional charges may apply | Unlimited bandwidth listed on every ISP plan |
| Small starting commitment | $18 for 10 shared ISP IPs or pay-as-you-go for traffic-based products | 50-IP package at $65 monthly |
| Managed scraping tools | Web Unlocker, SERP API, browser and scraper products | Proxy service focus |
| KYC for residential/mobile | May be required | Check current order requirements before purchase |

The lower entry point for Bright Data’s shared ISP pool is useful if you need only ten IPs. HypeProxies begins at 50 IPs, so it is not the better fit for every small project.

The comparison changes at higher traffic. For example, a team using 100 static IPs with traffic above 10 TB per month is beyond Bright Data’s combined 100 GB-per-IP fair-use allowance. A fixed-price plan with unlimited bandwidth may be easier to model, provided U.S. coverage and static ISP IPs meet the project requirements.

## A simple way to choose without overthinking it

Use this checklist before paying for anything:

1. **Need rotating residential IPs or location granularity outside the U.S.?** Start with Bright Data’s residential network and test at pay-as-you-go rates.
2. **Need static IPs in many countries?** Bright Data’s ISP options have broader geographic reach.
3. **Need only a small static ISP pool?** Bright Data’s 10-IP shared plan has the lower initial commitment.
4. **Need 50 or more static U.S. ISP IPs with heavy monthly transfer?** Compare HypeProxies first, because unlimited bandwidth changes the total-cost picture.
5. **Need data returned through an API rather than to manage proxies yourself?** Price Web Unlocker or SERP API by expected successful requests.
6. **Expect usage to fluctuate?** Avoid a large monthly traffic commitment until you have measured real consumption.

For U.S.-based static ISP workloads, the 50-IP HypeProxies plan is a reasonable starting point. It costs $65 monthly, uses a predictable fixed-price model, and avoids having to calculate a per-IP traffic allowance before the project has even warmed up.

[👉 View the HypeProxies 50-, 100-, and 254-IP ISP plans](https://bit.ly/Hypeproxies)

## Bright Data pricing FAQ

### Is Bright Data free?

Bright Data offers a recurring free tier of 5,000 credits per month for eligible API products, including Web Unlocker, SERP API, Web Scraper API, Scraper Studio, and Browser API. Its residential, ISP, and datacenter proxy networks are not included in that recurring free tier.

### Does Bright Data offer pay-as-you-go proxy pricing?

Yes. Bright Data publicly lists pay-as-you-go options for residential, ISP, datacenter, and mobile proxy products. The unit and rate depend on the product type. Residential access is priced by GB, while some static proxy plans are available per IP or by bandwidth.

### What is the cheapest Bright Data proxy plan?

For static ISP proxies, the smallest public shared-pool tier is 10 IPs for $18 per month. For datacenter proxies, the smallest listed tier is 10 IPs for $14 per month. The cheapest option is not necessarily the right one; proxy type, location, session needs, and traffic volume matter more than the headline price.

### Does Bright Data’s “unlimited” ISP plan have a bandwidth limit?

Bright Data states that static ISP proxies include a 100 GB fair-use allowance per IP per month. The allowance is pooled across the IPs purchased, and additional charges may apply after the allowance is exceeded.

### Is HypeProxies cheaper than Bright Data?

For a small 10-IP requirement, Bright Data’s shared ISP plan starts at a lower total monthly price. For 50 or more U.S.-focused static ISP IPs, HypeProxies has lower listed per-IP pricing and includes unlimited bandwidth. It is not a direct substitute for Bright Data’s global rotating residential network, mobile proxies, or managed scraping APIs.

### Should I choose monthly or quarterly HypeProxies billing?

Choose monthly if you are testing a workflow, ramping up a new project, or uncertain about how many IPs are needed. Quarterly pricing reduces the effective monthly cost, but it makes more sense after traffic and IP-count requirements are stable.

[👉 Compare HypeProxies monthly and quarterly ISP proxy packages](https://bit.ly/Hypeproxies)
