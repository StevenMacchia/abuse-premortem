# Safeguards library

104 practical safeguards, each with an owner and an effort estimate. The pre-mortem picks the ones that matter for a product and ranks them into a launch plan.

## Product (27)

| Safeguard | Effort |
|---|---|
| In-product reporting on every user, message, post and listing, with reasons that match your policies | Small effort |
| Block and mute, where a block stops all contact and hides the person who blocked | Small effort |
| Tell users which rule they broke, what action was taken and how to appeal | Small effort |
| Limited abilities for new accounts until they build trust, such as no links or messages to strangers | Small effort |
| Blur explicit images in private messages by default, with a warning and one-tap reporting | Medium effort |
| Adults can't find or message minors they aren't connected to, and minors' accounts are private by default | Medium effort |
| Age assurance proportionate to the risk: age estimation or ID checks where the law or the harm requires it | Large effort |
| Age-appropriate defaults for under-18s: private account, limited discovery, sensitive content filtered, location off | Medium effort |
| Parental controls and visibility suited to the age group | Medium effort |
| No profiling-based advertising to minors | Small effort |
| Review the design for manipulative patterns such as streaks, endless feeds, autoplay and pressure to spend | Small effort |
| Spending limits and purchase confirmations for minors, and odds disclosure for randomized items | Medium effort |
| In-context warnings when someone asks for money, crypto, gift cards or to move off the platform | Medium effort |
| Tell users what your staff will never ask for, and label official accounts | Small effort |
| An impersonation report flow, verified badges and protected names for notable accounts and your brand | Medium effort |
| Payout holds and velocity limits for new sellers, creators, hosts and payees | Medium effort |
| Buyer protection: funds released after delivery, with a clear dispute process | Large effort |
| Cap rewards per person, device and payment method, and release them after a delay | Small effort |
| Name checks on new payees, warnings for first-time and large transfers, and cooling-off periods | Medium effort |
| Controls for people to limit who can reply to, tag, mention or message them | Medium effort |
| Crisis resources and helplines shown when self-harm content, searches or messages are detected | Small effort |
| Block or add warning screens to searches linked to self-harm, eating disorders, child abuse and extremism | Small effort |
| Clearly and repeatedly tell users they are talking to an AI | Small effort |
| Approximate location by default; precise location is opt-in, time-limited and never shown to strangers | Medium effort |
| In-app safety tools: share trip or date details, an emergency button, check-ins | Large effort |
| Two-way ratings, and removal of users who put others at risk | Medium effort |
| Limit what guests can do: no private messaging, uploads, live or payouts until they create an account | Small effort |

## Engineering (35)

| Safeguard | Effort |
|---|---|
| Log every enforcement action (what, why, who, when) for audits and transparency reports | Medium effort |
| Rate limits on posting, messaging, invites and account actions, stricter for new accounts | Small effort |
| Bot friction at sign-up (e.g. Cloudflare Turnstile or reCAPTCHA) and blocking of disposable emails | Small effort |
| Email or phone verification before posting, messaging or claiming rewards | Small effort |
| Device, network and behavior signals to link duplicate, banned and fake accounts | Medium effort |
| Automated screening of text for abuse, spam and scam patterns, routed to human review | Medium effort |
| Check links against phishing and malware lists (e.g. Google Safe Browsing) before they are clickable | Small effort |
| Malware scanning of uploaded files and blocking of executable file types | Small effort |
| Nudity, violence and gore detection on uploads, with sensitive media behind a warning screen | Medium effort |
| Hash-match every image and video against known CSAM (e.g. PhotoDNA, Thorn's Safer, NCMEC and IWF hash lists) | Medium effort |
| Detection of grooming signals: adults contacting many minors, requests to move apps, gifts or money to minors | Large effort |
| Point teens to NCMEC's Take It Down and adults to StopNCII.org, and hash-match those submissions | Medium effort |
| Detect sextortion patterns (new accounts requesting images, then payment demands) and warn targets | Large effort |
| Scam-pattern detection across messages and profiles: scripts, reused photos, payment requests | Large effort |
| Screen listings for prohibited, counterfeit and misleading items when they go live | Medium effort |
| Payment risk scoring, strong customer authentication (3-D Secure) and chargeback monitoring | Medium effort |
| Multi-factor authentication, with stronger options than SMS for high-value accounts | Medium effort |
| Block breached passwords and detect credential-stuffing attacks | Small effort |
| Hardened account recovery, with alerts for new devices and changes to email, phone or payout details | Medium effort |
| Only verified customers can review, with detection of review bursts, swaps and linked reviewers | Medium effort |
| Detect money-mule behavior: funds passing straight through, many unrelated senders, recruitment messages | Large effort |
| Hash-sharing for terrorist content (e.g. GIFCT) and a crisis protocol for live attacks | Medium effort |
| Keep borderline and sensitive content out of recommendations, especially for teens | Medium effort |
| Input and output filters for disallowed generations: sexual content involving minors, real-person sexual imagery, weapons | Large effort |
| Screen training and fine-tuning data for CSAM and non-consensual imagery | Medium effort |
| Label AI-generated media and attach provenance data (e.g. C2PA content credentials) | Medium effort |
| Detect crisis signals in conversations, route people to help, and block romantic or sexual roleplay with minors | Large effort |
| Limit what AI agents and tools can do, and keep untrusted content separate from instructions | Medium effort |
| Strip GPS and device metadata from uploaded photos | Small effort |
| Anti-scraping controls: rate limits, bot detection and limits on bulk profile access | Medium effort |
| API access review, keys, quotas and developer terms you actually enforce | Medium effort |
| Least-privilege access to user data and review tools, with audit logs | Medium effort |
| Periodic selfie re-verification to stop accounts being shared or rented | Medium effort |
| Detection of coordinated networks of fake or controlled accounts | Large effort |
| Session, device and network signals to rate-limit and block abusive guests, since there is no account to ban | Medium effort |

## T&S Ops (17)

| Safeguard | Effort |
|---|---|
| A review queue with a named owner, response times by severity and an escalation path | Medium effort |
| Appeals for enforcement decisions, reviewed by someone other than the original reviewer | Medium effort |
| Quality sampling of moderation decisions to catch errors and inconsistency | Medium effort |
| A restricted escalation path for child-safety cases, handled by specially trained and supported reviewers | Medium effort |
| A way to report suspected under-age accounts and remove them | Small effort |
| A fast-track removal process for intimate images shared without consent (48 hours under the US TAKE IT DOWN Act) | Medium effort |
| Train reviewers on trafficking indicators and set up referral paths to law enforcement and NGOs | Medium effort |
| Ability to remove terrorist content within one hour of an EU removal order | Medium effort |
| Eligibility rules for going live, instant stream shutdown and 24/7 on-call coverage | Medium effort |
| A protocol for imminent-risk cases, including referral to emergency services | Medium effort |
| Monitoring for emerging harmful trends and challenges | Medium effort |
| Red-team before launch and after each model update, and track the jailbreak success rate | Medium effort |
| Monitor for abuse patterns and act against accounts, not just single prompts | Medium effort |
| A response process for offline harm, with victim support and law-enforcement liaison | Medium effort |
| Advertiser verification and ad review for scams, prohibited categories and discriminatory targeting | Medium effort |
| One named owner for safety, plus an on-call rotation for urgent escalations | Small effort |
| Moderator wellness: exposure caps, blurred or grayscale review tools and counseling | Medium effort |

## Policy (10)

| Safeguard | Effort |
|---|---|
| Written community guidelines that cover these harms, with examples of what crosses the line | Small effort |
| A review-moderation policy that never suppresses genuine negative reviews | Small effort |
| A vulnerable-customer policy for spotting signs of financial difficulty or coercion and adjusting treatment | Medium effort |
| A private-information policy with fast removal of doxxing, and detection of posted addresses and phone numbers | Small effort |
| Authoritative health information and a clear medical-misinformation policy | Medium effort |
| Block sexual or deceptive generations of real, identifiable people | Small effort |
| Rules requiring hosts to disclose any cameras, with fast reporting for guests | Small effort |
| An anti-discrimination policy, with testing of algorithms and of host or provider decisions | Medium effort |
| An elections integrity plan, with verification for political ads and a misinformation policy | Medium effort |
| A prohibited goods and services policy, with keyword and image screening | Small effort |

## Legal & Compliance (15)

| Safeguard | Effort |
|---|---|
| A notice channel for illegal-content reports from users, authorities and trusted flaggers | Small effort |
| A documented process to report apparent CSAM to NCMEC (US) and national authorities, preserving evidence | Medium effort |
| Verifiable parental consent before collecting personal data from under-13s | Medium effort |
| Collect only the personal data the feature needs, with retention limits | Small effort |
| Verify the identity, age and consent of everyone who appears in sexual content before it is published | Large effort |
| Verify high-volume sellers' identity, business and bank details | Medium effort |
| Identity verification (KYC) before money can be sent, received or paid out | Large effort |
| Transaction monitoring for laundering and mule patterns, with suspicious activity reporting | Large effort |
| Sanctions screening of users and counterparties (e.g. OFAC, EU and UK lists) plus geo-restrictions | Medium effort |
| Affordability and suitability checks before credit or high-risk products | Medium effort |
| An escalation path for credible threats, including emergency disclosure to law enforcement | Medium effort |
| Identity verification for people offering in-person services, plus background checks where lawful | Large effort |
| Notice-and-takedown for copyright and trademark (e.g. DMCA), with a repeat-infringer policy | Small effort |
| A law-enforcement request process: published guidelines, emergency disclosure and data preservation | Medium effort |
| Keep guest session records long enough to investigate reports and answer law-enforcement requests | Small effort |

---

Part of [T&S Workbench](https://github.com/stevenmacchia/ts-workbench) by [Steven Macchia](https://www.linkedin.com/in/stevenmacchia). Content licensed [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/): reuse it freely with credit.
