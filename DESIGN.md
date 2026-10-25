---
name: JinaqKit
description: An inherited working cabinet for synthetic recipe assemblies, all-or-none component debits and separate full returns.
colors:
  primary: "#126653"
  primary-hover: "#0b5343"
  navy: "#183e60"
  ink: "#172e45"
  page: "#edf3f8"
  surface: "#ffffff"
  line: "#b9cbd9"
  navigation-surface: "#dce9f3"
  muted: "#46627a"
  input-stroke: "#7894aa"
  link: "#174e7e"
  pending: "#795200"
  error: "#942721"
  error-surface: "#fff0ee"
  focus: "#bd671a"
  selection-surface: "#b7ded2"
  selection-ink: "#132f29"
typography:
  primary-heading:
    fontFamily: 'system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif'
    fontSize: "2rem"
    lineHeight: 1.15
    letterSpacing: "-0.025em"
  section-heading:
    fontSize: "1.3rem"
  brand:
    fontSize: "1.4rem"
    fontWeight: 740
  body:
    fontFamily: 'system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif'
  label:
    fontWeight: 600
  supporting:
    fontSize: "0.9rem"
  exact-json:
    fontSize: "0.85rem"
rounded:
  control: "7px"
  panel: "12px"
spacing:
  evidence-gap: "0.4rem"
  inline-gap: "0.5rem"
  action-gap: "0.6rem"
  control-inset: "0.7rem"
  table-cell: "0.9rem"
  unit: "1rem"
  page-inline: "1.25rem"
  panel-inset: "1.4rem"
  section: "2rem"
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.surface}"
    rounded: "{rounded.control}"
    padding: "0.65rem 1rem"
  button-primary-hover:
    backgroundColor: "{colors.primary-hover}"
  button-secondary:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.navy}"
    rounded: "{rounded.control}"
    padding: "0.65rem 1rem"
  button-default:
    backgroundColor: "{colors.navy}"
    textColor: "{colors.surface}"
    rounded: "{rounded.control}"
    padding: "0.65rem 1rem"
  field:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.ink}"
    rounded: "{rounded.control}"
    padding: "{spacing.control-inset}"
    width: "100%"
  panel:
    backgroundColor: "{colors.surface}"
    rounded: "{rounded.panel}"
    padding: "{spacing.panel-inset}"
  navigation-current:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.navy}"
    rounded: "{rounded.control}"
    padding: "0.65rem 1rem"
  component-table:
    backgroundColor: "{colors.surface}"
    rounded: "{rounded.panel}"
    width: "100%"
  component-table-heading:
    backgroundColor: "{colors.navigation-surface}"
    textColor: "{colors.ink}"
    typography: "{typography.supporting}"
    padding: "{spacing.table-cell}"
  exact-recipe-disclosure:
    padding: "0.7rem 0"
---

# Design System: JinaqKit

## Overview

**Creative North Star: "The Shared Work Cabinet"**

JinaqKit extends the documented TazaBatch Shared Work Cabinet. It keeps the navy identity and navigation, pale blue workspace, white labelled forms and tables, green explicit actions, system typography, and native controls. The incumbent system remains the visual authority for this bounded synthetic component ledger; the task extends an existing world.

Its character is direct, flat, and readable. A saved assembly leads with identity, version, kit count, author, timestamp and written outcome, followed by every component's before/needed/after quantities. Current return state is separate from that historical result, and current balances have their own section. The signature is a shortage that leaves every after quantity equal to before, alongside a successful whole-component debit that an administrator can return once through a separate record.

**Key Characteristics:**

- Inherited navy navigation and pale blue workspace.
- Green labelled submit actions and white bordered native forms and tables.
- System typography with a fixed-size task heading.
- Written saved outcome and every component's before/needed/after quantities.
- All-or-none shortage evidence with unchanged after values.
- Historical assembly, current return state and current balances kept distinct.
- Required administrator reason and one-time full-return action.
- Native exact-recipe disclosure with authored RU/KK language nodes and visible focus.

## Colors

The cool inherited palette uses Cabinet Navy for orientation and Working Green for explicit actions. The frontmatter owns implemented values. Sidecar tonal strips are inherited derived inspection metadata, not additional interface colors.

### Primary

- **Working Green** (`primary`, `primary-hover`): native submits and explicitly primary actions, including checking or publishing a recipe, recording an assembly outcome and recording a full return. The retained status utility also uses green; report headings communicate outcomes with text.

### Secondary

- **Cabinet Navy** (`navy`): header, baseline filled buttons, navigation text and secondary-control borders.
- **Link Blue** (`link`): links and field carets.

### Tertiary

- **Pending Amber** (`pending`): retained inherited pending utility; preview and saved outcomes use explicit written headings.
- **Error Red / Pale Error** (`error`, `error-surface`): refused-action notices, including the stale-command refusal. Saved shortage diagnostics remain readable text on the page ground.
- **Focus Amber** (`focus`): visible keyboard focus.
- **Soft Selection Green / Selection Ink** (`selection-surface`, `selection-ink`): native text selection.

### Neutral

- **Cabinet Ink** (`ink`): root text, headings and tables.
- **Cool Workspace** (`page`): page ground and scrollbar track.
- **White Surface** (`surface`): native fields, form panels, tables, ordinary notices and current navigation.
- **Divider Blue** (`line`): containers, table rows and evidence dividers.
- **Navigation Mist** (`navigation-surface`): navigation strip and table headings.
- **Supporting Slate** (`muted`): historical/current distinctions, synthetic boundary, digest and footer.
- **Field Slate** (`input-stroke`): field borders and scrollbar thumb.

**The Inherited Shell Rule.** Extend the current TazaBatch cabinet instead of replacing its palette, typography, or navigation grammar.

## Typography

The recorded system stack serves task headings, body and controls. No webfont is loaded. The main heading has a fixed size, section headings are smaller, and the brand has the recorded heavier weight. Unspecified body size, heading weights and line heights retain browser defaults. Preformatted data in the inherited settings surface uses the browser's native face at the recorded smaller size; it is not a separate display identity.

Paragraphs have maximum measure (72ch) and line height (1.6). Labels and buttons use weight (600). Tables use tabular numerals, left/top alignment and wrapping text. Authored descriptions preserve line breaks through `white-space: pre-wrap`. Written outcomes distinguish preview from saved history; they are not conveyed by color alone.

The document uses `lang="ru"`. Recipe editors mark `descriptionRu` and `descriptionKk` fields with `ru` and `kk`. `recipeView` renders both authored descriptions in separate paragraphs with their respective language attributes, including the exact original recipe disclosure. Labels, report headings and diagnostics remain Russian interface text. Authored content is neither language-detected nor translated.

**The Authored Language Rule.** Keep authored RU/KK descriptions in their own language nodes; labels, diagnostics and status copy remain Russian interface text.

## Layout

Header and navigation share inline padding (`max(1.25rem, calc((100% - 1160px) / 2))`). Main is centered with maximum width (1200px), padding (`2rem 1.25rem`) and minimum height (75vh). The header uses a spaced flex row; navigation uses the recorded inline gap. The retained optional work grid uses columns (`minmax(0, 1fr) minmax(260px, 0.8fr)`); paired rows use equal columns. Assembly detail follows a vertical reading order, with white panels reserved for available forms and white full-width native tables for component evidence.

Source declares a stacked breakpoint (700px and below): retained grids stack, main padding becomes (`1.4rem 1rem`), panel padding becomes (1rem), navigation wraps with padding (0.6rem), and the header identity aligns to the top at size (0.8rem) with maximum width (140px). At the narrow table/search breakpoint (600px and below), search tools stack, navigation buttons use `flex: auto`, table cells receive minimum width (140px), and a horizontal-scroll hint appears. A labelled focusable table wrapper owns scrolling. These are source-defined responsive rules; their rendered behavior remains unverified.

Action rows wrap. Headings, identity, evidence, disclosures, footer, direct screen paragraphs and diagnostic items allow long text to wrap. Preview evidence has a top divider, unit top margin/padding and the recorded evidence gap. Detail order is assembly identity and metadata, saved outcome and complete quantity table, historical/current helper text, current return state, any available administrator return form, exact original recipe disclosure, publication digest, refresh/return actions and any allowed archive action.

The [finish review](docs/finish-review.json) records a bounded `ship` verdict for six supplied actual 1280px captures. Five current shipping JPEGs show [shortage](docs/shortage-1280.jpg), [return form before submission](docs/return-form-1280.jpg), [completed return on the original assembly](docs/returned-1280.jpg), [separate reversal](docs/reversal-1280.jpg) and [current balances](docs/balances-1280.jpg); their own synthetic origin, hashes and source aliases are in [capture provenance](docs/capture-provenance.json). The sixth is the [stale-command refusal](../../../outputs/products/jinaq-kit-stale-refusal.jpg), enumerated by the review. All six were opened as valid, nonblank JPEGs. The five shipping aliases preserve their reviewed source bytes.

Mobile/390px and 1440px remain unverified: requested viewport settings were accepted but the reported DOM width stayed 1280px. This documentation pass inspected current frontend source and the six local rasters; it did not operate a browser or rerun context, detector, interactions or backend tests. The visual verdict covers those supplied states at their actual width. It does not establish other screens, every breakpoint, hover/loading/empty/overlong content, touch, a screen-reader audit, backend correctness, concurrency, restore, transport, security, real-data suitability or a service outcome.

## Elevation & Depth

No box shadow, backdrop effect, transition or animation is defined. White panels and tables, pale fills, one-pixel borders and whitespace separate regions. Hover changes brightness and primary fill without motion. Replacing screen content and focusing a task or preview heading provides continuity without animation. No decorative raster is used. The six screenshots are evidence assets, with the supplied five shipping aliases in [capture provenance](docs/capture-provenance.json) and the complete visual-review packet in [finish review](docs/finish-review.json).

## Shapes

Controls and notices use the smaller recorded radius; panels and table wrappers use the larger one. Borders are one pixel. Textareas start at height (100px) and resize vertically. Buttons and native disclosure summaries have minimum height (44px). Native disclosure markers remain visible. Exact recipe components use an ordinary unordered list. Retained fieldset and recipient-choice rules do not define this assembly-detail composition.

## Components

### Buttons

Native labelled actions use padding (`0.65rem 1rem`) and the recorded label weight. Explicit primary and all submit buttons use Working Green with white text; hover combines the deeper primary fill with brightness (1.13). Secondary refresh, return, archive and settings actions use white with navy text and border. The retained baseline button rule is navy filled. Disabled buttons use opacity (0.55) and `cursor: not-allowed`. Focus-visible is an amber outline (3px) with offset (3px); narrow buttons have maximum width (100%). The initiating button is disabled while its request runs.

### Cards / Containers

Flat white form panels use a Divider Blue border, the panel radius and recorded inset, reduced at the stacked breakpoint. Login is capped at width (480px). Assembly metadata, saved result, current return state, exact recipe and current balance lines stay on the page ground. Preview evidence follows its form rather than opening a modal or second workspace.

### Inputs / Fields

Native inputs, selects and textareas use White Surface, Cabinet Ink, Field Slate borders and Link Blue carets. Every generated field has a connected label and ID. Archived or role-protected editors retain values through native read-only fields or disabled selectors. Integer editors use native number inputs with step (1) and configured limits; configured text bounds use `maxLength`. Assembly quantity is bounded to 1–100 kits in the form. Both receipt and full-return reasons are labelled required fields. The application contains no manual component-balance field.

Recipe description editors carry explicit RU/KK language attributes. The one-time full-return form has its own required reason textarea and explicit submit label. Failed requests preserve the form and focus the shared polite status notice. The stale-refusal capture shows the recovery message and retained return reason; neither the reason nor the visible action establishes a saved return.

### Navigation and Notices

The linked brand and current user/role lead the navy header. Inactive section controls are transparent on the pale strip; the current collection is white bordered with `aria-current="page"`. The initial collection is assemblies (`assemblies`). The skip link becomes visible on focus. Task/detail changes focus the leading heading using `tabindex="-1"`; successful previews focus their result heading. The shared notice has `role="status"`, `aria-live="polite"` and a programmatic focus target. Empty notices are hidden. Refused-action notices use Pale Error and Error Red; ordinary notices use White Surface. These source semantics and the supplied focus state do not establish a complete keyboard or screen-reader audit.

### Publication and Assembly Preview

Publication preview uses a labelled recipe selector and **Проверить рецепт**, then renders saved-candidate code/version, title, both authored descriptions and component quantities. **Опубликовать эту версию** follows that evidence. Selector changes clear the preview; a generation guard ignores obsolete responses.

The assembly form uses a publication selector, kit quantity, reason and **Проверить все компоненты**. The result identifies recipe/version and kit count, then states **Все компоненты доступны · пока не записано** or **Нехватка · пока не сохранена**. It presents every component's before/needed/after and says that preview does not change balances. **Явно записать этот исход** is a separate explicit action even when the report is a shortage. Editing any form value clears the old preview, and a generation guard prevents an obsolete response from appearing current. This behavior is documented from source; no preview raster was supplied for the finish verdict.

**The Preview Boundary Rule.** Keep preview wording, complete component evidence and the separate explicit record action together; a preview neither reserves components nor establishes a saved outcome.

### Saved Outcome and All-or-None Component Table

Assembly detail leads with sequence and recipe code, saved recipe version, kit count, original actor, server time and reason. The persisted report follows as **Весь расход записан** or **Нехватка — списаний нет**. Its table has column-scoped headers **Компонент**, **Было, шт.**, **Нужно / вернуть, шт.** and **Стало, шт.**. The focusable wrapper has a horizontal-scroll label. Each table preserves every saved line with its saved component code/name and numeric before/needed/after values.

A shortage explains that at least one component is unavailable, lists each shortage and states that all balances remain unchanged with no partial debit. The supplied shortage #4 identifies PACK missing 1; CARD remains 8→8 with need 6 and PACK remains 2→2 with need 3. The successful assembly #3 retains CARD 10→8 with need 2 and PACK 3→2 with need 1, including after a later full return. Historical helper text directs the reader to **Компоненты** for current balances.

**The All-or-None Rule.** Keep the written shortage, every shortage amount and every component's unchanged after quantity together; available components must not appear debited by a rejected assembly.

### Current Return State and Explicit Full Return

**Текущее состояние возврата** follows saved assembly evidence. A shortage says there is nothing to return because it debited nothing. An unreturned successful assembly shows an administrator-only white form titled **Один полный локальный возврат**, the local-only boundary, required **Основание полного возврата** and **Вернуть все компоненты один раз**. Staff receive the administrator explanation. A visible form or entered reason remains a before-submission state.

After completion, the form is replaced by the separate reversal's sequence, actor, time, reason and **Открыть полный возврат**. In the supplied completed state, assembly #3 retains its original debit table and links to separate return #5. Return detail shows the historical return table: CARD 8→10 with return 2 and PACK 2→3 with return 1. **Исходная сборка** links back. The result is a distinct local record; the original assembly is unchanged.

**The Full Return Rule.** Keep the required administrator reason and explicit one-time action for all original components; completed return identity replaces the form while the original saved assembly remains intact.

### Exact Original Recipe and Current Balances

**Точный исходный рецепт** is a native `details`/`summary` after current return state. It retains the assembly's saved code/version, title, RU/KK authored descriptions and component code/name/quantity list. It is closed by default in source. The publication SHA256 follows outside it. Current draft recipe edits and current component renames do not replace the saved recipe display. The digest is inspectable consistency evidence, not a signature or security guarantee.

The **Компоненты** collection shows **Текущие синтетические остатки, шт.** before search and records. Its supplied capture displays archived renamed NEW_CARD at 10 and PACK at 3 while historical assembly and return screens retain CARD and the original name. The current summary includes the archived component; the record table still obeys the archive-visibility filter. There is no editable balance field. Archive controls state that visibility changes do not change quantities or history.

**The Historical Snapshot Rule.** Keep saved assembly quantities and exact original recipe separate from current return state and current balances; current names or recipe edits must not overwrite historical evidence.

### Tables and Data Disclosure

Native record tables use collapsed borders, left/top aligned cells, padding (0.9rem), wrapping values, maximum cell width (28ch) and pale headings. Headers have column scope; each record has a labelled open action. The last row removes its bottom divider. Search and the archive checkbox retain native labels; an empty result has explanatory text. Assembly list cells add the current returned label to the stored report status.

The inherited data/access surface uses native account fields, labelled download/journal actions, a native recent-event disclosure and a file input followed by an explicit restore-confirmation panel. Its copy states the shared workspace, absent password/session-recovery UI and unsigned-copy boundary. These source-visible controls do not establish tenant isolation, backup authenticity, security certification or a complete settings review. The list and footer preserve the synthetic/shared-area boundary and make no physical-stock, order, payment or Make-connectivity claim.

The sources of this scan are [app.js](public/app.js), [styles.css](public/styles.css) and [index.html](public/index.html), with product truth in [PRODUCT.md](PRODUCT.md), the preserved six-block direction in [public-app-js.md](.impeccable/surfaces/public-app-js.md), and inherited visual authority in [TazaBatch DESIGN.md](https://github.com/wpalish/taza-batch/blob/778cd3b176be02f79a274484d9b9f6987eac7c61/DESIGN.md). [.impeccable/design.json](.impeccable/design.json) contains ten self-contained static visual examples, extension metadata and this document's narrative; the examples have no application handlers or backend execution.

## Do's and Don'ts

### Do:

- **Do** inherit the navy header, pale workspace, white native forms/tables and green primary action.
- **Do** keep connected labels, column-scoped table headers, native disclosure markers and visible focus.
- **Do** preserve authored RU/KK descriptions within Russian interface copy.
- **Do** distinguish unsaved preview, saved assembly outcome, current return state and current balances.
- **Do** show every component's exact saved before/needed/after quantities with the written outcome.
- **Do** keep shortage amounts and every unchanged after quantity together.
- **Do** keep the required administrator reason and explicit one-time full-return action with its local boundary.
- **Do** preserve the original recipe snapshot and separate saved return identity.
- **Do** retain draft input and show the recovery message after a stale-command refusal.
- **Do** allow long descriptions, timestamps, component names and SHA256 digests to wrap.

### Don't:

- **Don't** replace the inherited cabinet with a new visual identity, ornamental assets or animation.
- **Don't** hide labels or replace native tables and disclosures with decorative imitations.
- **Don't** present a preview or entered return reason as a saved quantitative operation.
- **Don't** imply a partial component debit for a shortage or a partial/repeated full return.
- **Don't** substitute current component names, balances or recipe drafts for historical snapshots.
- **Don't** present archive visibility as deleting quantities or cancelling the original operation.
- **Don't** imply Make connectivity, a physical warehouse, orders, payments, external writes or delivered service outcomes.
- **Don't** present a SHA256 digest or this bounded visual verdict as a signature or security certification.
- **Don't** claim mobile or 1440px verification from captures whose actual width remained 1280px.
