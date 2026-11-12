If you are switching advertising agencies, settle three things before the new team makes a single change: your business holds top-level access to every ad and tracking account, you have exported the history you would otherwise lose, and everyone agrees on a cutover date and what "working" means. Most painful transitions are not strategy problems. They are access, data and timing problems discovered after the old agency is gone.

Use the checklist below with your current agency still on the account. It is easier to fix ownership while everyone is cooperative.

## 1. Confirm who owns each account

Make a list of every account that touches your ads, then check who holds the highest level of access. The goal is simple: your business should be able to remove any agency without losing the account.

| Asset | What to check | Who should hold top-level access |
|---|---|---|
| Google Ads | Your own user has Admin access. Check whether an agency manager account is the account's owner. | Your business |
| Meta ad account | The ad account sits in your business's own portfolio and the agency works through partner access. | Your business |
| Google Analytics | Your own user has the Administrator role at the account level, not only the property. | Your business |
| Google Tag Manager | At least two administrators from your organization. | Your business |
| Payment method | The card or invoice profile is in your business's name. | Your business |
| Creative and copy files | Source files and approved versions live somewhere you control. | Your business |
| Call tracking and landing pages | Numbers, forms and pages are in an account you can keep. | Your business |

Google Ads has a detail that surprises many advertisers: if an agency's manager account created your Google Ads account, that manager automatically becomes the account's owner. An owner manager can invite and remove users and transfer ownership. Your account still owns its data and can unlink the manager, but you need an Admin user of your own to do it.

Meta works on a similar principle. Only the business portfolio that owns an asset, such as an ad account or Page, can share it with another business, and if an agency shares an asset with you, you are limited to the permissions the agency assigned. If your ad account lives in the agency's portfolio rather than yours, agree with them how it will be handed over before the relationship ends.

Google Tag Manager's help center is blunter: it recommends at least two administrators and says the account should be managed by someone in your organization, not an external agency.

## 2. Export what you would otherwise lose

Ask for these before the old agency's access ends:

- Change history. Google Ads keeps account, campaign and ad group changes for two years, including who made each change. Export the period you care about.
- Search term reports and negative keyword lists.
- Audience and remarketing list definitions.
- Conversion action definitions: what counts as a lead or sale, and where each one is recorded.
- Approved creative, copy and destination URLs, with the date each version was approved.
- The last few monthly reports, plus a note on how each metric was defined.

## Don't lose leads in the handover

Leads collected inside ad platforms don't stay there forever, and they don't always go where you think. Check these while the old agency still has access.

- **Export lead-form leads before access changes, then again on cutover day.** Google Ads stores lead-form leads for 60 days, and the CSV download covers only the last 30 days. Meta Instant Form leads can be downloaded for up to 90 days after someone submits the form; after that, Ads Manager still counts them in Results, but you can't download them.
- **Check who can export.** In Google Ads you need Standard or Admin access to download leads, and a manager account can download a client account's leads only if the client account gives it ownership. If only the agency's manager account has been pulling leads, have someone with Admin access on your own account run the export.
- **List where every form sends leads today.** Google lead forms can deliver leads by CSV download, a webhook to your CRM, third-party integrations such as LeadsBridge, HubSpot, Salesforce or Zapier, or the Google Ads API. Meta's help center describes connecting a CRM, for example through Zapier, to retrieve Instant Form leads. If that destination is the agency's CRM or connector account, new leads keep going there after you leave.
- **Repoint before you revoke.** Point each form at a destination you control first, then send a test lead and confirm it arrives. For Google webhooks, Google treats any response other than HTTP 200 from your endpoint as an error, so a form that looks connected can still fail.
- **Keep website-form tracking intact.** If your site forms capture click IDs or UTM parameters in hidden fields, keep those fields through any landing-page rebuild. Leads that arrive without a source make the first month's comparison meaningless.

Lead handover worksheet (template; fill in your own details):

| Lead source | Platform keeps it | Who exports | Sent to today | New destination tested |
|---|---|---|---|---|
| Google lead form | 60 days (CSV: last 30) | | | |
| Meta Instant Form | 90 days | | | |
| Website form | Your CRM | | | |

## 3. Write down what "working" means

Before the new team starts, record a baseline for the last 8–12 weeks: weekly spend, qualified leads or sales, cost per qualified result, and any weeks that looked unusual. Agree which conversion actions count. If the old and new teams define a lead differently, the first month of reporting will look like a change in performance when it is really a change in definition.

## 4. Plan the cutover

- Pick a cutover date and decide who is allowed to edit campaigns before and after it.
- Decide which campaigns keep running unchanged during the handover.
- Confirm the payment method and budget caps in the account, not only in the contract.
- Remove the old agency's access after the cutover date and confirm the new team can see everything they need.

## 5. Give the new team an audit window before a rebuild

A new manager will usually want to restructure. Ask for a written audit first: what they found, what they will change, and in what order. Agree that every change gets a short reason in a change log. Avoid changing conversion goals, bidding and campaign structure in the same week; if results move, nobody will know why.

## 6. Agree on approvals

Decide who approves creative and who authorizes spend. An approved ad and an approved launch are separate decisions. If you use a platform as well as an agency, the [agency platform checklist](/blog/agency-ai-marketing-platform-checklist) covers how to test the approval step before moving client work. Before anything relaunches, the [campaign launch checklist](/blog/ai-campaign-launch-checklist) is a useful final pass.

## Transition worksheet

| Item | Owner today | Action | Done by | Confirmed |
|---|---|---|---|---|
| Google Ads admin user | | | | |
| Google Ads manager ownership | | | | |
| Meta ad account location | | | | |
| Analytics Administrator | | | | |
| Tag Manager administrators (2+) | | | | |
| Payment method | | | | |
| Change history export | | | | |
| Conversion definitions | | | | |
| Lead export and form destinations | | | | |
| Creative and copy archive | | | | |
| Cutover date | | | | |

### Example: a handover gap

Here is an illustrative example, not a customer story. A clinic replaces its agency and the new team cannot edit the Google Ads account. The agency's manager account created it years ago and still owns it. The clinic's office manager has read-only access. The fix is not complicated, but it needs the old agency's cooperation to grant Admin access or transfer ownership, which is why this check comes first.

## If you are moving to a platform instead of an agency

Ask a software platform the same questions you would ask an agency: whose account the ads run in, who can see spend, and what you can export if you leave. Adessa launches campaigns on supported managed channels without client ad-account setup, and connects a client-owned account on other channels; reports export to PDF and CSV. Ask us the same ownership questions you would ask anyone else. Agencies evaluating Adessa can start with the [agency overview](/agencies).

## Sources

Checked October 27, 2026:

- Google Ads Help: [About ownership of client accounts](https://support.google.com/google-ads/answer/7456532), [About access levels](https://support.google.com/google-ads/answer/9978556) and [About change history](https://support.google.com/google-ads/answer/19888)
- Google Analytics Help: [Add, edit, and delete users](https://support.google.com/analytics/answer/9305788)
- Tag Manager Help: [Managing users and permissions](https://support.google.com/tagmanager/answer/6107011)
- Meta Business Help Center: [Give a partner access to business assets](https://www.facebook.com/business/help/1717412048538897) and [Add people to a business portfolio and assign a business asset](https://www.facebook.com/business/help/2169003770027706)

Lead-handover section checked November 12, 2026:

- Google Ads Help: [About lead form assets](https://support.google.com/google-ads/answer/9423234), [Download leads](https://support.google.com/google-ads/answer/10089020) and [How to set up a webhook integration for a lead form](https://support.google.com/google-ads/answer/16729613)
- Meta Business Help Center: [About expired leads](https://www.facebook.com/business/help/1526849577619206)
