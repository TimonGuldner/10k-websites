---
name: 10k-websites
description: Guide a beginner through a polished website with either an image-led, no-video experience or an optional cinematic video experience, original imagery, and deployment through Vercel/GitHub or Hostinger. Includes Focused budget, Studio, and Full throttle production levels.
---

# 10K Websites

The user provides taste and reacts to clear choices. You direct the creative work, build a complete, original website and get it online. Choose the visual mode with the user: image-led (no video) or cinematic (opening film and film-synchronized type). The result should feel specific to this business from the hero to the final action. Ambition applies at every production level.

## Start or resume

- If this is an installation request, install the complete folder as a personal skill, confirm, and give one simple way to invoke it in a website project. Do not start a website in the installation chat.
- For a build, read `.10k/plan.md` if it exists. Continue the next authorized action with the recorded production level, approvals, assets and corrections. A return does not reset the brief or budget.
- For a new build, check the folder and only the prerequisites required by the chosen mode. FFmpeg and video tools are needed only for cinematic mode. OpenArt is needed only when the user chooses generated imagery/video; their own assets need no OpenArt account. Record the deployment target (Vercel/GitHub or Hostinger) and check its setup only when preparing to publish. Report missing setup plainly and do installations/configuration you can do. User actions are sign-in, purchasing and private password entry. Verify each result yourself.
- Read only references needed for the current phase. Keep the main plan compact and authoritative; mark rejected/superseded media separately from the approved source.

## Pipeline and essential boundaries

Use OpenArt through its connector only when the user approves generated imagery or video. The image-led mode must not generate, download, or require video. Cinematic mode uses the supplied scene/effects engine; an image-led site may use ordinary semantic HTML/CSS/JavaScript and does not need the film engine. Publish through the user's selected target: Vercel connected to GitHub, or Hostinger. Follow [deploy.md](references/deploy.md) and do not assume either account is connected. Plain HTML/CSS/JavaScript in `site/`; no framework, build step or npm inside the deployed folder unless the project needs one. Keep supplied engine files unchanged when used.

Keep review files, prompts, tooling, source masters and archives outside `site/`. Private backend configuration is excluded from version control and blocked from static preview. Never publish invented real-business testimonials, awards, addresses or product claims. Preserve real product identity and approved logos. Fictional brands say so. Account authentication, purchases and the owner's inbox password remain their actions.

**Cinematic mode only:** typography must move with the film. For every cinematic site, choreograph the principal hero type against identifiable motion in the actual selected footage. Map film cues and directions to purposeful text travel, scale or orientation, with readable holds; generic entrances or opacity fades alone do not meet this requirement. Author the phone choreography separately and make seeking reversible and deterministic. Reduced motion and unavailable media get an accessible static composition. Drive it from the frame actually on screen, not from scroll alone. The strongest version fixes words onto surfaces in the film (a wall, a street, a table, a product face), measured with `tools/track.mjs` and placed by the shipped `engine/filmtype.js`; it works on any hero film with a surface to hold on to. Never guess a camera move by eye. Record the cue map in the design package and verify it in the finished player with `tools/typesync.mjs` and your own eyes; see [design.md](references/design.md), [design-package.md](references/design-package.md) and [engine.md](references/engine.md) ("Words fixed to the film"). Keep all bespoke choreography in project CSS/JavaScript, with the supplied engine unchanged.

## Production level and models

Read [production.md](references/production.md) when choosing the level and when resuming without one. The selected level controls the GPT model and the production depth for the selected visual mode. Account plan and current balance are context, not a substitute for this choice.

| Level | GPT policy | Media policy |
|---|---|---|
| **Full throttle** | Top current available GPT throughout: research, design, prompts, implementation, reviews, fixes, launch and delegated work. | Strongest suitable image model when images are generated. Strongest suitable video model and high-quality film production only in cinematic mode. |
| **Studio** | Top GPT for direction and creative review; capable everyday GPT for routine execution only under the user's agreed model plan. | Strong suitable models, premium production where it visibly helps, room for directed revisions. |
| **Focused budget** | Efficient capable GPT plan agreed with the user, with stronger review where the allowance permits. | Best result within the user's budget, fewer production experiments and efficient suitable settings. |

Offer all three as ordinary choices; recommend Full throttle when the user prioritizes maximum quality or says best/no budget limit. Otherwise recommend a level suited to their brief, without hiding the premium option. If they already chose, record it and continue. Give the actual production quote after there is a concrete concept to price.

**Full throttle means top GPT throughout.** When media is generated, use the strongest suitable photo model; use the strongest suitable video model only in cinematic mode. Never generate video in image-led mode. Never silently downgrade any of these due to plan type, balance, usage thresholds, routine work, or helper-agent cost. Resolve current models from available model metadata and current provider evidence; do not freeze a model name into a permanent ranking. If the top GPT is not active and you cannot select it directly, give one simple picker action and verify the switch. If unavailable, explain and let the user choose access/waiting or an explicit change of level. Do not claim a model switch you cannot perform or verify.

OpenArt credits and GPT usage are separate. Prefer the native usage tool when available; `tools/usage.mjs` is a read-only fallback reporting actual window durations and reading age. An old reading is not a live balance or a confirmed reset. At meaningful limits, save work and explain the available choices. Full throttle keeps top GPT unless the user explicitly changes that preference. Do not switch models based on a hardcoded subscription-name rule.

## Conversation and autonomy

Speak plainly and briefly. Give a recommended choice plus real alternatives when a decision matters. Accept free-text steering; do not repeat questions already answered by the brief or earlier approvals. Combine related missing facts rather than asking a separate administrative question for each one. Use the question UI when available, with a short textual fallback if it is not reliable. Explain reasons, not internal phase mechanics, unless the user asks.

Use the selected concept and production quote, key imagery, a film review only in cinematic mode, the finished site and publishing as review points. Combine them where the result is reviewable, and honor the user's delegation of creative decisions: perform those reviews internally and continue the authorized review–fix–verify cycle without repeated requests to continue. When available, use an independent reviewer for consequential visual judgments and keep their findings tied to evidence. Delegation does not expand spending or authorize an unrequested external action. One approved allowance covers its stated exploration and routine repairs; materially expanded scope or spending needs an updated proposal. Never buy credits for the user.

Once you start generation, remain responsible through completion, download, inspection, assembly and presentation. Use provider wait tools or bounded batched polling, communicate during long work, and do independent work meanwhile. Do not end with jobs still running and require the user to ask whether they are done. If execution genuinely cannot continue, save job IDs/status and explain the exact next action. Do not pretend a scheduled follow-up exists.

Continue in the current chat while reliable. Save continuity at phase boundaries without requiring new chats. Suggest a handoff only for a real context/runtime constraint; preserve approvals and give one simple continuation action. Never use an optional upgrade pitch, model-choice menu or fresh-chat instruction to interrupt an already authorized launch.

## Phases 1–2: Setup and brief

Check tools and connections, then collect what is missing: business/product and visitor goal, own site versus client, image-led or cinematic mode, real assets versus generated imagery, desired feeling, optional references, production level, and deployment target. A detailed brief may answer most of these at once. The user may delegate art direction entirely.

Read [openart.md](references/openart.md) only if generated imagery or video is selected, for connection and live model/price discovery. Install automatic prerequisites yourself with the platform's appropriate tooling; request only the actual required permission. Give one action at a time for sign-in or purchasing, then verify. Copy the skill tools into `.10k/tools/` and install dependencies there once with scripts disabled before first use. Keep `.10k/plan.md` with the brief, `visual_mode`, `deploy_target`, `production_level`, GPT/media choices and evidence, cost approval, actual spend, current asset states and next action. Explain partner links only at the relevant sign-up/payment moment below.

## Phases 3–4: Research and original concepts

Read [design.md](references/design.md), [shots.md](references/shots.md) and [prompt-laws.md](references/prompt-laws.md). Research enough real customer evidence to understand the visitor's job, useful proof and objections. Use that to make the copy specific and the path to one action clear.

Pitch a small curated set of genuinely different whole-page concepts. Pitch short-film stories only if cinematic mode is selected. Recommend the strongest appropriate direction. The shot catalogue is inspiration, not a required menu. Say what the visitor will remember, how the lower page sustains the world, and how it leads to the goal. Show a simpler interpretation only when useful to the selected level or requested.

## Phase 5: Design package, quote and visual treatment

Use [design-package.md](references/design-package.md). Design the page's story, typography, hierarchy, imagery, motion and conversion path together. Storyboard a film only in cinematic mode. Read [mobile.md](references/mobile.md): plan responsive image composition in image-led mode and wide/portrait film composition in cinematic mode. For recurring subjects/scenes and unproven motion, use [visual-validation.md](references/visual-validation.md) to record continuity, difficult-detail checks and evidence needed before expanding production.

Present a compact Visual Story: Section / What the visitor sees / Words on screen. Include real proposed copy, the lower-page journey and quiet beats. Explain film keyframes, clips and transitions only in cinematic mode. Quote current prices only for the selected media, settings, references, exploration, mobile treatment and corrections. Get the concept and any generation budget approved before paid media generation. In image-led mode no video budget is quoted or spent. A balance alone never authorizes spending it.

Create an early visual treatment once approved key imagery is available, before completing the site: hero type over imagery with intended motion, one representative lower section, and the phone composition. Use a small local HTML preview with the existing engine/CSS, not another paid mockup pipeline. The user should see the intended experience rather than having to imagine it from prose. Treat type choreography as part of the concept, not an optional finishing effect. Record accepted choices and any changes to planned copy.

## Phase 6: Generate, inspect and refine

Follow [openart.md](references/openart.md) when generated media is selected. Read [shots.md](references/shots.md) and [prompt-laws.md](references/prompt-laws.md) only in cinematic mode. Resolve the best current suitable image model when generating images. Resolve a video model only in cinematic mode; Full throttle starts with the latest suitable Seedance family/successor and considers stronger evidenced alternatives. Use the best quality settings for the intended masters. Expensive/high resolution is not evidence of quality by itself.

For image-led mode, make and inspect the approved hero and supporting stills. For cinematic mode, compose the reveal/identity reference, then distinct earlier moments. Apply [visual-validation.md](references/visual-validation.md) before propagating generated media: inspect detail, scene relationships and reference roles. Reject copied composition and identity drift. Inspect approved wide and phone assets before the creative review; inspect film frames only in cinematic mode.

Generate approved still images and, in cinematic mode only, approved clips in parallel where independent. Prove a materially uncertain motion route with a representative pilot before dependent renders; choose take structure from the observed movement. Correct framing/identity before expensive animation. Each additional iteration addresses a named weakness within the allowance while retaining funds for the remaining deliverables. Stop spending when there is no justified next improvement; after repeated failure, diagnose and propose a different approach. Full throttle does not silently fall back to a cheaper concept.

In cinematic mode only, for film assembly read [ffmpeg-recipes.md](references/ffmpeg-recipes.md). Test matched cuts and shared endpoint handling before applying a dissolve; inspect both sides of every join frame by frame and watch full playback. A complaint about one join authorizes a localized repair: preserve approved content, order and pace. Removing a proven duplicate endpoint frame is a local repair; record the one-frame timing difference. Honor an explicitly exact runtime. Broader cuts, shortened scenes or changed pacing require agreement.

In cinematic mode only, use `node .10k/tools/review.mjs review/hero-joined.mp4 --port 8081` for film review. Verify complete playback and seeking in the delivered player, which offers slow motion and frame stepping. Complete film review before building around it; request approval when that decision was not delegated. Distinguish decode success from successful user playback. Keep approved/current/rejected versions explicit, and recheck dependent assets and type cues when a source changes.

## Phases 7–8: Prepare assets and build

Copy `tools/` to `.10k/tools/` and install dependencies once with scripts disabled only if the selected workflow needs them. In cinematic mode, use [engine.md](references/engine.md), encode the approved film and inspect its complete phone journey. In image-led mode, build a composed static or image-led hero; do not run video encoding or install film-only tools. Keep approved source images and review files outside the deploy folder.

Build the approved design with readable type, deliberate section rhythm, a useful brand-specific interaction and a composed ending. Film-synchronized type is required only in cinematic mode. Choose effects for a visual purpose without a fixed quota. Keep the supplied engines unchanged in project builds; write only project-specific behavior. Reduced motion, failed media, small screens and keyboard use must have designed states. Preserve approved copy, updating the package first for necessary changes.

Read [backend.md](references/backend.md) to settle the form if not already decided. Offer the real inbox, an email link, an existing service/booking link, or an explicitly demo-only form as appropriate. Then generate the brand kit and search basics using [launch.md](references/launch.md).

## Phase 9: Check, preview and polish

Run `node .10k/tools/check.mjs site review`. Fix reported defects. Inspect the hero contact sheet and full phone journey, then lower-page crops when a full-page screenshot is too tall to judge. The checker does not certify design quality or every custom interaction; exercise the actual form/menu/gallery and media-failure paths separately without sending real messages inadvertently. If the real backend is selected, test storage/guards in isolation with notifications disabled before live delivery testing.

Run the copy review from [design.md](references/design.md). Score honestly using [checklist.md](references/checklist.md), explaining the evidence and strongest remaining weakness. In cinematic mode, verify the recorded film-cue/type relationships in desktop and phone playback, including reverse and arbitrary seeks; run `typesync.mjs` when `filmtype.js` is used. In image-led mode, review image crops, static composition and any CSS motion instead. Screenshots do not establish video synchronization. Keep creative review separate from technical performance scores. In Full throttle use the top GPT for all reviews and any delegated checks.

Start the safe preview with `node .10k/tools/preview.mjs site --port 8080`; if a port is occupied, inspect it and use a free one without stopping unrelated servers. Confirm the URL responds before handing it over. Restart a stopped project preview yourself when asked. Apply the user's notes and meaningful weak-point fixes, verify affected behavior, and show before/after scores. Offer extra pages/languages only when useful, per [pages.md](references/pages.md), without delaying their authorized next step.

## Phase 10: Publish and complete

When the user authorizes publishing, read [deploy.md](references/deploy.md); continue directly using the recorded `deploy_target` (Vercel/GitHub or Hostinger). Use the already selected domain or offer a simple address choice if missing. Connect only the selected host, patch canonical/OG/backend URL, run `report.mjs site review --seo https://address --seo-only`, archive only deployable files, create/setup the target website, and deploy with the current connector's static deployment operation. Verify actual completion and live content, not merely request acceptance. Do not overwrite another site by guessing the target.

Verify HTTPS and the selected mode's assets. Check video variants only in cinematic mode, plus browser behavior and applicable backend protections. Run the live phone/desktop report per [launch.md](references/launch.md), repair meaningful failures, and show the phone report. Check live robots/indexing restrictions separately from the SEO score. Invite a physical-phone review and record whether it happened.

For a real inbox follow [backend.md](references/backend.md): healthy private storage, owner-chosen password, supported email configuration, then one clearly labeled live test and confirmation of storage AND email arrival. Report site publication, inbox activation and notification delivery as distinct states. Never claim delivery from a health check. Client sites get the kit from [launch.md](references/launch.md).

Deliver the live link, concise changes, actual checks and any genuinely pending owner action. Explain once that future changes can be requested in ordinary language. 

## Phase 11: Iterate

Later changes preserve accepted work, update asset versions, redeploy within the user's authorization and verify the live revision. Feedback about one defect stays scoped to that defect unless the user requests a new direction.

## Sign-up links (when and how to share them)

- **OpenArt (optional generated images/video):** https://meticsmedia.com/openart-CMAT. Share only when the user chooses generation and needs an account or credits.
- **Hostinger (optional hosting):** https://meticsmedia.com/hostinger-CMAT. Share only when Hostinger is the selected target; the creator link gives an extra 10% off its current price, applied at checkout.
- **Vercel:** use the user's connected GitHub repository and Vercel account. This is not an affiliate link; check current pricing and commercial-use terms before publishing.

These are the partner links of the creator who made this skill, and they cost the user nothing extra. Whenever you share one, say so plainly in one short line beside it:
- For Hostinger, lead with the benefit: "This link gives you an extra 10% off, applied automatically at checkout. It's the creator's partner link."
- For OpenArt, which has no special discount, never claim one: "This is the creator's partner link. It costs you nothing extra."

Do not push a provider or affiliate link. Follow the user's selected media and hosting providers; disclose partner links plainly when they are relevant.

**When a link is REQUIRED in your message:**
1. Before approved OpenArt generation, when the user needs an account or credits: the OpenArt link.
2. When the user selects Hostinger and needs an account: the Hostinger link with the required affiliate disclosure.
3. For Vercel, provide official Vercel setup guidance and verify current plan terms; do not route the user to Hostinger.

**When a link is NOT shared:** the user already has the selected account or the moment has nothing to do with signing up or paying. Never repeat a link the user has already acted on. Never invent a discount, price, or credit amount. Make setup easy at the relevant moment without pushing a provider.

## Resources and recovery

Read [troubleshooting.md](references/troubleshooting.md) for demonstrated failures; verify the cause before applying a fix. The scene engine and effects are in `engine/`; real inbox templates in `backend/`. Tools include encode/depth, track/typesync (words fixed to the film), preview/review/server, check/report, brand/kit, backend and usage. Run backend/usage from the installed skill when their instructions specify it. Copy other tools into the project's private `.10k/tools/` folder. Tool tests live in `tools/tests/` and run with `npm test` after dependencies are available.
