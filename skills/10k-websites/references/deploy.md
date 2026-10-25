# Deploy to Vercel/GitHub or Hostinger

Read at launch. Use the `deploy_target` selected in `.10k/plan.md`; do not switch providers silently. Preserve the user's address and publishing authorization. Continue an already authorized launch without another design review or new approval step.

## Choose and connect the selected host

### Vercel through GitHub

Use this path when `deploy_target: vercel`. Connect the user's GitHub account to Vercel and import the approved website repository. The skill's plain static site lives in `site/`; set that as the project root, use no build command, and publish the static files from that root. If the project uses a framework or build step, inspect its actual configuration and set the correct root/build/output instead of applying these defaults. Let Vercel create a preview deployment first; publish to production only when authorized. Commit/push the approved changes to the selected repository and verify the resulting deployment and live URL. Never expose tokens or change unrelated Vercel/GitHub settings.

Vercel's Hobby plan is restricted to non-commercial personal use. Before deploying a business/client website, check Vercel's current fair-use and plan terms; do not use Hobby for commercial work. Pro pricing, usage charges and tax can change, so inspect the current price before any commitment. The user signs in and approves any paid plan; never purchase it for them. Official references: https://vercel.com/docs/plans/hobby and https://vercel.com/docs/limits/fair-use-guidelines.

### Hostinger

Use the following account, connector and static-upload workflow only when `deploy_target: hostinger`.

## Accounts, costs and connection

OpenArt generation, GPT usage and hosting are separate. Follow [production.md](production.md) for GPT/media choices; Full throttle does not by itself require an oversized hosting plan. Verify current Hostinger plan features, price, renewal, domain/mailbox eligibility and site limits before recommending a purchase. A plain site needs static file serving; the real inbox also needs PHP with private writable storage. Use the appropriate existing plan when it fits. Do not promise fixed free mailbox counts or unverified discounts beyond the creator-link disclosure in SKILL.md.

If Hostinger is selected and already responds, skip setup. Otherwise use the current connector/plugin installation and authentication path exposed by the app. Run supported configuration steps yourself; the user signs in and authorizes access. Ask for a restart only if required by the actual installation state. Verify a read call returns account data. Never print access tokens or edit unrelated app configuration. Use the sign-up link and disclosure from SKILL.md when the user actually needs hosting.

## Discover narrowly, follow actual schemas

The current connector may expose `search`, `execute` and `multi_execute` rather than hundreds of direct tools. Discover only the operation needed and inspect its returned input schema. Old operation names are hints, not authoritative APIs. Do not print the full catalogue.

Typical operation purposes and recent names (verify before use):

| Purpose | Recent operation |
|---|---|
| List sites and existing plan | `hosting_websites_list`, hosting order listing returned by search |
| Inspect available domains | domain portfolio listing returned by search |
| Generate a free address | `hosting_domains_generate-free-subdomain` |
| Create on the selected plan | `hosting_websites_create` with domain and order_id |
| Wait for website setup | `hosting_websites_list-setups` for the domain |
| Upload prebuilt files | `hosting_deploy-static-website` with domain and archivePath |

Verify the account/plan and exact target before mutation. A queued/accepted response is not completion. Follow setup status with bounded waits/backoff before uploading. Do not repeat a create/deploy request simply because it is taking time. Keep progress messages short. Never overwrite an existing unrelated site or guess that an available domain belongs to this brand.

## Address and deployment package

Use the user's already chosen domain/free address on the selected host. Otherwise inspect that host's account, then offer a simple choice. A free `*.hostingersite.com` address is valid for preview/launch on eligible hosting; it does not imply a purchased domain or mailbox. Verify actual eligibility. Purchases remain the user's action.

Once the actual address exists, patch canonical, OG, structured-data and backend site URLs. Generate search files without starting a static PHP preview:

```sh
node .10k/tools/report.mjs site review --seo https://their-address --seo-only
```

Use file tools or explicit UTF-8 scripts for patches. Bump changed CSS/JS URL versions before redeployment so cached assets cannot hide the update.

Archive the CONTENTS of `site/`, with `index.html` at the top and all necessary assets beside it. Follow the current deploy tool's archive naming/schema requirements (for example `site_YYYYMMDD_HHMMSS.zip`). Inspect the archive, including hidden `.htaccess` files. With the real inbox include `api/`, protected configuration, `admin/`, `data/.htaccess` and `forms.js`; never package stored enquiries, logs, credentials unrelated to this backend, source masters, `.10k/`, node_modules, review files, or the archive itself. Preserve the existing backend secret/configuration on redeploy so private storage and passwords continue to work. Keep credentials out of version control.

For Hostinger, use the connector's prebuilt/static deploy operation for this plain site and PHP files when supported by its schema. It needs no Node build. Record the exact target, archive hash, deployment response and subsequently verified version. Wait for completion rather than equating successful upload with a live site.

## Verify independently of the deployment response

- Homepage loads over HTTPS with expected content/version.
- In image-led mode, hero and section images load with the intended phone crops. In cinematic mode, both intended video variants return successfully and phones do not download both large files.
- Actual browser forward/reverse scrub, readable captions, navigation, custom interaction, reduced motion and media fallback work without console/resource errors.
- With the real inbox, health reports writable private storage, config/data URLs do not expose source/data, and unauthenticated admin is a setup/login surface. Health does not establish email delivery.
- Run the live phone and desktop report from [launch.md](launch.md). Separately inspect the live `robots.txt`, response noindex headers and page robots tags. The selected host may apply indexing rules to preview addresses; a Lighthouse SEO score of 100 does not establish Google indexability. Describe the actual restriction without treating a user-selected preview address as a failed launch.

A new address may need time for DNS/HTTPS setup. Verify the cause and wait with backoff; do not bypass browser certificate protections. Report uncertainty honestly.

## Measure, present and hand over

Measure actual HTML/assets and, in cinematic mode, video size and arrival time. An HTML fetch alone is not total page weight or real-user speed. The site may contain a PHP inbox only on Hostinger; do not claim that PHP runs on Vercel. Lighthouse lab scores and local request times are evidence for this run, not guarantees for every connection.

Open the verified public HTTPS URL directly and label it as the live site; keep local preview and report links distinct. When an actual browser is part of the user's acceptance workflow, verify that address there when available rather than assuming a local HTML file or embedded preview represents the deployment. Open the phone report separately. Invite a check on the user's physical phone: ordinary scrolling, faster flicks, the hero, navigation and CTA; include reverse film scrubbing only in cinematic mode. Record physical-device confirmation separately from emulation.

For the real inbox, finish the distinct owner-activation and delivery steps in [backend.md](backend.md). Hand over the live site while clearly identifying any remaining owner-only action. Future authorized updates use the same target, preserve approved assets/backend state, bump versions, redeploy and verify the changed live content.
