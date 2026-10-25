# Production levels and model authority

Read when agreeing the production level or restoring a build without one. This is the single source of truth for model and spending policy; other references apply it rather than inventing their own defaults.

## Choose once, carry forward

Offer **Full throttle**, **Studio**, and **Focused budget** independently of the visual mode. Recommend Full throttle for maximum quality/best-model/no-budget-limit briefs, Studio for ambition balanced with cost, and Focused budget for an explicit ceiling. Also record `visual_mode: image-led | cinematic`; default to image-led/no-video unless the user asks for a film. Never infer approval to spend the account balance. Record both choices in `.10k/plan.md` alongside actual approvals. If earlier logs only contain `MODE=astra/save`, ask about production level only if the user's existing preferences do not resolve it.

All levels get original direction, a polished working website, responsive design and accessibility. The visual mode decides whether video exists; the production level changes model choice, production depth and iterations. Image-led/no-video is a complete first-class result, not a downgrade. Do not present the budget option as a deliberately generic design.

| Decision | Full throttle | Studio | Focused budget |
|---|---|---|---|
| GPT | Top current GPT for the entire workflow and every delegated task | Top GPT for direction and creative judgment; agreed capable everyday GPT for routine execution | Agreed efficient GPT, allocating stronger review where useful |
| Image generation | Strongest current suitable generation/editing model, high quality by default | Strong model/settings, premium for visibly important assets | Best suitable quality inside the ceiling |
| Video generation | Only in cinematic mode: strongest suitable flagship, assessed from current alternatives | Only in cinematic mode: suitable motion model, premium when justified | Only in cinematic mode: reliable model inside the ceiling; image-led mode uses no video |
| Exploration | Include a curated comparison of meaningfully different visual treatments and directed refinements | Explore the consequential design choices | Concentrate on one strong direction |
| Phone | Plan responsive image and film composition early; use separate portrait assets when materially better | Plan early; crop or portrait according to result and quote | Compose responsive assets carefully for both; quote exceptions |

## Resolve the GPT model separately from media

Use the current app/host model metadata or model catalogue first; use current official OpenAI guidance if needed. Resolve the strongest current GPT actually available to this user, record its exact identifier, evidence/date and active state. Do not infer capability from a subscription label or choose the first name alphabetically. Model identifiers age; this reference intentionally does not freeze one.

In Full throttle the top GPT handles research, concepts, storyboards, generation prompts, coding, testing, reviews, fixes and publishing. Helpers inherit it or explicitly select the same model when that is supported. Do not route implementation to an everyday model. Do not switch behind the user's back or claim to change a picker without a tool that can do it. If necessary ask once for the exact picker change, then verify. Do not create a new chat solely to switch models without the user's authorization.

If top-model access or usage prevents continuation, preserve the work and offer waiting/access recovery or an explicit user-selected change. A usage threshold never silently converts Full throttle into Studio. Show actual duration/reset information; OpenArt balance and GPT limits are unrelated.

## Resolve only the media models the selected mode needs

Use user-provided assets without connecting OpenArt. If the user approves generated stills, discover the live OpenArt image catalogue, exact forms and quotes. Discover video models only for cinematic mode; begin the Full throttle assessment with the latest suitable Seedance-family flagship or successor, then consider current evidenced alternatives. Never search, quote or generate video for image-led mode. Newest, most expensive, or highest resolution alone does not prove superiority. Catalogue fields prove capabilities, not ratings.

Use current provider documentation, credible comparable quality evidence and the actual shot requirements. If evidence is inconclusive and the difference matters, run a small comparison on the real scene when covered by the approval, or quote it first. Judge the hardest detail at matched scale and verify identity/composition using [visual-validation.md](visual-validation.md). State uncertainty honestly; do not label an untested model the universal best. Record model IDs, date, required controls, exact settings and why they suit the scene. Respect an explicitly requested model unless unavailable/incompatible; discuss that rather than substituting silently.

For generated media, Generated media uses high-quality settings by default in Full throttle. Higher-resolution masters are allowed when composition, texture, output size or portrait reframing benefits. Do not apply an arbitrary per-clip ceiling, medium-quality default or blanket 4K ban. Source quality and web delivery are separate: retain masters and encode responsive lightweight assets. A costly model that cannot perform the planned shot needs a revised method/model, not hidden compromise.

## Approve a concrete production allowance

After selecting a concept, quote exact planned settings and references for the selected mode: still-image exploration and supporting pictures; add keyframes, clips and film corrections only in cinematic mode. Include phone treatment and a correction allowance. Show the total and actual balance once. Full throttle expands resources; it does not automatically authorize new purchases, unlimited retries or unrelated work. If the user explicitly chooses no fixed ceiling, still disclose the next concrete batch and obtain its spending authorization before generation. Do not force a lower tier or a cheaper concept merely because their current balance needs a top-up.

One approval covers the disclosed batch and revisions within its allowance, including expensive models. Preflight exact calls and check funds privately; give short updates for meaningful changes rather than a new permission question for every call. Small price drift inside the overall allowance is covered. A larger total, new paid scope, changed model preference or exhausted allowance needs a concrete updated choice. The user tops up or purchases; the agent never does so for them.

Track actual charges and accepted/current/rejected assets. Each retry addresses a named problem; after repeated failure diagnose before spending again. Preserve the approved story when fixing local defects. Stop when the visual objective is met and save unused allowance. A more expensive or longer result is not inherently more successful.

Track completed charges, pending commitments and the latest quoted cost to finish the remaining deliverables separately. Before another paid revision, check their combined total against the authorized ceiling and current funding. Protect the agreed phone treatment, supporting assets and necessary delivery work from being consumed by repeated repairs to one format. A funded next call does not establish a funded completion plan. If a proposed retry displaces required work, pause that spend, continue independent work and present the concrete cost/scope choice; never infer a larger ceiling from 'keep going' or a top-up alone.

Keep the active plan compact: current authorization, selected asset versions, unresolved defects, remaining cost and next action. Archive superseded detail separately. If the user elects to publish the reviewed version with disclosed limitations, record the deferred work and complete the authorized launch without reopening cancelled refinements.
