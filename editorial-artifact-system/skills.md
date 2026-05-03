\# Atelier Zero Style Imagegen Prompt Pack

> ⚠️ **此文件为草稿/历史版本**。规范实现已沉淀为：
>
> - Skill：`skills/editorial-collage/`（含 `SKILL.md`、`example.html`、16 张素材图）
> - Design System：`design-systems/atelier-zero/DESIGN.md`
> - Imagegen Prompt Pack：`skills/editorial-collage/assets/imagegen-prompts.md`
>
> 后续维护请改动 skill 中的版本，本文件仅作起源记录保留。

这套提示词用于稳定生成类似参考图的网页首屏、栏目页、案例页、实验 archive、能力介绍等视觉稿。核心风格是：现代编辑设计 + 包豪斯几何 + 古典雕塑拼贴 + 建筑空间 + 纸张印刷质感 + 极简 UI。

\## 1. 永久风格锚点

每次生成都先复制这一段，再接后面的变量和版式模板。

\`\`\`text

Use case: ads-marketing

Asset type: editorial website hero / creative studio landing page visual

Primary request: Generate a refined editorial web page composition in the same visual language as a high-end creative AI research studio.

Style/medium: sophisticated digital collage, modern Swiss editorial layout, Bauhaus geometric composition, classical plaster sculpture fragments, brutalist/minimal architecture, art-direction website mockup, premium agency aesthetic.

Scene/backdrop: warm off-white handmade paper background with subtle grain, faint vertical folds, scanned paper fibers, lightly aged print texture, thin drafting lines and registration marks.

Subject: a surreal collage combining a cropped classical plaster head or face fragment, abstract architectural blocks, archways or stairs, sky cutouts, one small human figure, a delicate tree or botanical element, and geometric color planes.

Composition/framing: wide 16:9 web page layout, strong asymmetrical grid, generous negative space, large typography area on the left or top-left, collage focal object on the right or center-right, precise alignment, thin divider lines, small UI navigation details.

Lighting/mood: soft diffused daylight, museum-like calm, intelligent, restrained, tactile, poetic, premium, research-driven.

Color palette: warm ivory, stone beige, soft concrete gray, deep black text, muted charcoal, washed coral-red accent, occasional mustard-yellow accent, pale sky blue only inside small sky/image cutouts.

Materials/textures: matte plaster, limestone, travertine, concrete, rough torn paper edges, halftone print grain, translucent vellum-like overlays, fine grid paper, dotted matrix patterns.

Typography: large clean grotesk sans-serif for main headline, elegant high-contrast italic serif for emphasized words, tiny uppercase coral labels, compact UI microcopy. Text must be crisp, readable, and spelled exactly as provided.

Graphic details: thin hairline circles, partial arcs, crosshair marks, small black dots, dotted grids, fine coordinate lines, numbered annotations, small arrow buttons, simple pill buttons, minimal logo mark.

Constraints: preserve a high-end editorial web design feel; make the page look usable as a real website mockup; keep spacing elegant and uncluttered; no cartoon style; no neon colors; no glossy 3D; no busy gradients; no generic stock-photo look.

Avoid: distorted typography, misspelled text, extra random words, heavy shadows, childish illustration, cyberpunk, saturated purple/blue palette, plastic materials, overly decorative UI cards, cluttered composition, low-resolution textures, watermark.

\`\`\`

\## 2. 可替换变量槽位

把尖括号里的内容替换为你的项目内容。

\`\`\`text

Brand/logo text: "&lt;BRAND_NAME&gt;"

Navigation text: "&lt;NAV_1&gt;", "&lt;NAV_2&gt;", "&lt;NAV_3&gt;", "&lt;NAV_4&gt;", "&lt;NAV_5&gt;"

Small eyebrow label: "&lt;EYEBROW&gt;"

Main headline, verbatim: "&lt;MAIN_HEADLINE&gt;"

Italic emphasis words, verbatim: "&lt;ITALIC_WORDS&gt;"

Body copy, verbatim: "&lt;BODY_COPY&gt;"

Primary button, verbatim: "&lt;PRIMARY_CTA&gt;"

Secondary button, verbatim: "&lt;SECONDARY_CTA&gt;"

Footer/micro labels, verbatim: "&lt;FOOTER_LABELS&gt;"

Main collage subject: &lt;plaster head / eye / hand / architectural arch / staircase / product / landscape / plant / custom object&gt;

Inserted image/texture motifs: &lt;sky, mountain, ocean, eye close-up, dancer, stone, fabric, UI screenshot, map, grid, handwritten note&gt;

Accent color: &lt;washed coral red / mustard yellow / pale blue / muted sage&gt;

Page type: &lt;hero / testimonials / projects carousel / method timeline / archive grid / capabilities cards / about studio&gt;

\`\`\`

\## 3. 英文通用生成模板

适合直接给图像模型使用。文字部分尽量用英文，图像模型对英文排版更稳。

\`\`\`text

Use case: ads-marketing

Asset type: &lt;PAGE_TYPE&gt; for a creative AI studio website

Primary request: Create a 16:9 high-end editorial website mockup inspired by the supplied reference style, with customizable typography and surreal architectural collage.

Brand/logo text: "&lt;BRAND_NAME&gt;"

Navigation text: "&lt;NAV_1&gt;", "&lt;NAV_2&gt;", "&lt;NAV_3&gt;", "&lt;NAV_4&gt;", "&lt;NAV_5&gt;"

Small eyebrow label: "&lt;EYEBROW&gt;"

Text (verbatim): main headline "&lt;MAIN_HEADLINE&gt;"; italic emphasis words "&lt;ITALIC_WORDS&gt;"; body copy "&lt;BODY_COPY&gt;"; primary button "&lt;PRIMARY_CTA&gt;"; secondary button "&lt;SECONDARY_CTA&gt;".

Scene/backdrop: warm ivory handmade paper canvas with subtle grain, faint fold lines, tactile printed texture, fine drafting marks.

Subject: &lt;MAIN_COLLAGE_SUBJECT&gt; integrated with classical plaster fragments, minimal concrete architecture, arch or stair geometry, delicate tree/botanical element, small human figure, and layered cutout textures: &lt;INSERTED_TEXTURES&gt;.

Style/medium: premium Swiss editorial web design, surreal art-directed collage, Bauhaus geometry, museum catalog restraint, tactile print finish.

Composition/framing: &lt;COMPOSITION_DIRECTION&gt;. Use a clear grid, large readable headline, precise micro UI, thin lines, circles, dotted matrices, numbered annotations, and small arrow/pill controls.

Lighting/mood: soft natural daylight, calm, intelligent, refined, slightly poetic.

Color palette: ivory paper, black typography, stone beige, concrete gray, charcoal, &lt;ACCENT_COLOR&gt; accent, occasional mustard yellow accent, restrained pale blue sky cutouts.

Materials/textures: matte plaster, rough stone, concrete, torn paper, halftone grain, translucent overlays, fine grid paper.

Typography: clean modern sans-serif for the main headline; elegant italic serif for selected emphasis words; tiny uppercase coral labels; compact UI text. Render all provided text exactly and legibly.

Constraints: realistic website mockup, balanced negative space, no clutter, no extra copy, no misspellings, no watermark.

Avoid: generic templates, stock-photo hero, shiny 3D, cartoon illustration, neon colors, heavy gradients, unreadable UI text, random symbols, extra logos.

\`\`\`

\## 4. 中文项目输入模板

中文内容建议先转成英文或短中文。若必须保留中文，尽量减少字数，并要求「verbatim」。

\`\`\`text

请生成一张 16:9 横版网页视觉稿，风格为高级创意 AI 工作室官网：现代瑞士编辑排版、包豪斯几何、古典石膏雕塑拼贴、极简建筑、手工纸张肌理、细线工程制图标记。

品牌文字："&lt;品牌名&gt;"

导航："&lt;导航1&gt;", "&lt;导航2&gt;", "&lt;导航3&gt;", "&lt;导航4&gt;"

小标签："&lt;小标签&gt;"

主标题必须逐字渲染："&lt;主标题&gt;"

需要使用优雅斜体衬线强调的词："&lt;强调词&gt;"

正文必须逐字渲染："&lt;正文&gt;"

按钮文字："&lt;按钮1&gt;", "&lt;按钮2&gt;"

画面主体：&lt;主体描述&gt;

贴图和元素：&lt;天空/石材/植物/人物/眼睛/舞者/山脉/水面/UI 截图等&gt;

构图：&lt;左文右图 / 右文左图 / 顶部大标题下方横向卡片 / 中央拼贴 / 时间线分栏&gt;

色彩：暖象牙白纸张、黑色文字、石灰/混凝土灰、炭黑、低饱和珊瑚红点缀、少量芥末黄或浅天蓝。

限制：文字清晰可读，不添加多余文字，不要水印，不要卡通，不要霓虹，不要厚重阴影，不要俗套科技蓝紫渐变。

\`\`\`

\## 5. 版式模板

\### A. Hero 首屏

\`\`\`text

Composition/framing: left side contains a large stacked headline with selected italic serif words, small coral eyebrow above, short body copy and two pill buttons below; right side contains a large surreal collage of a cropped plaster head with an open top, sky and architecture inserted into the head, a tree growing through the composition, coral sun disk behind it, mustard accent circle near the base, and thin technical drawing marks around it.

Page type: hero landing page.