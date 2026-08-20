# Cogwheel's List marketing assessment

## Executive assessment

There is a real but deliberately narrow need for a macOS relay that keeps Apple
Contacts and one Google Sheet synchronized in both directions without adding a
third editing surface. The strongest use case is a person or small organization
that treats Contacts.app as its canonical human editing surface, but needs the
same structured records in a Sheet for planning, review, reporting, or a
lightweight operational workflow. The product is differentiated by its narrow
boundary: it connects two existing homes for data, makes conflict behavior
visible, and does not ask users to maintain a second contact editor.

The opportunity is not “another contacts app.” It is a controlled bridge for
users who already have Apple Contacts and Google Sheets in their workflow and
want the two to agree. The Hummingbird License materially narrows the initial
commercial market, so the most credible early audiences are individuals,
qualifying educational organizations, qualifying 501(c)(3) organizations, and
commercial organizations during the license's one-time evaluation period or
after a separate commercial license.

## Who needs this relay?

### Individuals and households

People who keep a personal address book in Apple Contacts but use a Google
Sheet for trip planning, household administration, volunteer rosters, or a
small personal index can benefit from bidirectional synchronization. They do
not need another editor; they need consistent copies in the two tools they
already use.

### Educators and educational organizations

Teachers and qualifying universities, schools, or community colleges may need
to review a contact set in a Sheet while retaining Contacts.app as the editing
surface. The license's exact definition of “Educational Organization” and its
noncommercial educational-purpose condition must be checked for each proposed
use; this assessment does not expand that grant.

### Qualifying 501(c)(3) organizations

A qualifying nonprofit may have a direct educational or teacher-support use for
a shared Sheet view of contacts while keeping the source workflow in Apple
Contacts. The license permits commercial use by a 501(c)(3) only when the use
directly benefits an educational organization or accredited teacher. That
condition is a market qualification, not a general nonprofit exemption.

### Commercial evaluators and licensed commercial users

A commercial organization can use the product for the single 30-consecutive-
day commercial evaluation period described in the license. After that period,
continued commercial use requires a separate paid license managed by Business
Handyman, LLC on behalf of the licensors. A commercial buyer should therefore
evaluate the operational fit and licensing path together.

## Problem and positioning

The product answers a specific workflow problem:

1. Apple Contacts is convenient for human contact management on macOS.
2. Google Sheets is convenient for shared tabular review and operational work.
3. Manual copying creates stale records, duplicate edits, and unclear ownership.
4. A one-way export solves only the first handoff; it does not keep both sources
   current.
5. A third editor creates another place where values can diverge.

Positioning should emphasize “bidirectional relay, two existing editing homes,
one selected Sheet, visible safety stops.” It should not promise universal CRM
replacement, a contact database, or a spreadsheet editor. The locked product
shape also gives the marketing story a trust angle: when the system cannot
reconcile safely, it exposes the condition rather than silently choosing a
winner.

## Competitor and alternative assessment

The following are named alternatives or categories. The comparison describes
the workflow difference relevant to Cogwheel's List; it is not a claim that
every version or configuration of a named product has identical behavior.

| Alternative | What it is good at | Difference from Cogwheel's List |
| --- | --- | --- |
| iCloud Contacts | Native Apple-device contact synchronization inside Apple's ecosystem. | It is not primarily an Apple Contacts to one Google Sheet relay. Cogwheel targets the cross-ecosystem bridge while leaving Contacts.app as the human UI. |
| Google Contacts | Contact management and synchronization within Google's ecosystem. | It does not by itself provide the narrow Apple Contacts to selected Google Sheet workflow. Cogwheel connects the Apple source to a Sheet rather than replacing Contacts.app with a Google contact editor. |
| CardDAV | An open protocol and server pattern for synchronizing address books among compatible clients and services. | CardDAV is a protocol/service interoperability route, not a purpose-built one-Sheet operational view. Cogwheel's value is the Apple Contacts ↔ Google Sheet boundary and its explicit conflict/safety rules. |
| Contacts-sync utilities | Utilities that move or synchronize contacts between address books, accounts, or services. | Some may be closer functional substitutes, but they vary by direction, target, conflict handling, UI, and service support. Cogwheel is intentionally limited to a bidirectional relay with no editing UI and one specified Sheet. |
| Zapier / Make | Broad automation platforms connecting many apps through triggers, actions, and workflows. | They are general-purpose automation layers and may introduce cloud workflow configuration, task limits, or a separate operational surface. Cogwheel is a dedicated local macOS relay with a defined two-source model, not a general automation builder. |
| CSV export tools | Simple one-time or batch extraction into a portable tabular file. | CSV export is a handoff, not an ongoing bidirectional sync. It does not maintain an ancestor or represent a live conflict freeze between Contacts and a Sheet. |

### Competitive takeaway

The nearest substitute is not one product; it is a stack of manual export,
general automation, native ecosystem sync, or a contacts-sync utility. The
message should lead with the specific two-tool workflow and the absence of a
third editor. Feature comparisons should stay honest about the narrower target:
Cogwheel trades breadth for a legible boundary and explicit fail-closed/fail-
stop behavior.

## Hummingbird License v1.6, U.S. Edition: full review

This section is a plain-language marketing reading of the checked-in
`LICENSE`, not legal advice. The license text controls.

### Ownership and scope — section 1

The Software is defined broadly: source, object and executable code, documents,
specifications, templates, media, data, and other associated or distributed
artifacts. Ownership is stated as joint and equal among Jonny Bass Foundation,
Josef Strand Foundation, and Business Handyman, LLC. Business Handyman, LLC is
the designated organization to manage license agreements.

Marketing implication: a buyer or partner should treat the whole distributed
package, not only the executable, as within the license scope and should route
commercial licensing questions to the stated manager.

### Grant — section 2

The grant is free, nonexclusive, and nontransferable, but purpose and user type
matter:

- Individuals may use, copy, modify, merge, publish, and distribute for
  personal, non-business use.
- Defined educational organizations may do the same for noncommercial
  educational purposes. Private K-12 schools are excluded unless prior written
  permission is given.
- A 501(c)(3) may use, copy, modify, merge, publish, and distribute, including
  commercially, only when the use directly benefits an educational
  organization or accredited teacher.
- Another commercial organization receives one nonrenewable, nonperpetual,
  consecutive 30-day commercial evaluation license beginning at first use.

After the evaluation period, commercial use requires a separate paid license.
The license expressly lists commercial advantage examples such as sale,
subscription, advertising-supported use, fee-based services, and integration
into commercial products.

Marketing implication: “free” cannot be used as a blanket commercial pricing
claim. The product can be marketed to qualified users under the stated grants,
and to other commercial organizations as an evaluation followed by a paid
licensing conversation.

### Redistribution — section 3

Redistribution in source, binary, or other form must retain the copyright notice,
conditions, and disclaimers.

Marketing implication: a distributor, integrator, or educational recipient must
preserve the license material with redistributed Software. Packaging should not
remove or obscure those notices.

### Contributors — section 4

Contributors retain copyright in their contributions, but grant the licensors
and all recipients a perpetual, worldwide, royalty-free license to use, modify,
and distribute those contributions under the same license terms. Exceptions
must be negotiated before contribution.

Marketing implication: contributors can retain copyright, but should understand
the downstream license grant before submitting work. Contribution terms should
not be described as a typical permissive inbound assignment or as a promise of
exclusive ownership by the contributor.

### Termination — section 5

Rights terminate automatically when a licensee violates a term or condition.
After termination, all granted rights cease and use and distribution must stop.

Marketing implication: compliance is not optional housekeeping. Commercial
users need an explicit license path before continuing beyond the permitted
evaluation or outside an applicable qualified-user grant.

### Disclaimer, governing law, severability, entire agreement — sections 6–9

The Software is provided “as is” with broad warranty disclaimers and liability
limits. California law governs. Invalid provisions do not invalidate the rest,
and the license is the entire agreement concerning its subject matter.

Marketing implication: claims should focus on the documented product boundary
and observed behavior, not warranties or guarantees that the license disclaims.
The California governing-law provision and the entire-agreement language are
reasons to send bespoke commercial arrangements through the designated licensor
representative.

## Source-available implications versus MIT and GPL

“Source-available” is the useful market description here: the source and
artifacts are visible, but the license does not grant the broad, unrestricted
commercial freedoms commonly associated with MIT, and it is not a copyleft
license that generally conditions distribution on releasing derivative source
under GPL terms.

| Topic | Hummingbird v1.6 U.S. Edition | Typical MIT terms | Typical GPL terms |
| --- | --- | --- | --- |
| Commercial use | Restricted by user type, purpose, and time; most commercial use after the one-time evaluation needs a paid license. | Generally permitted, including commercial products, subject to notice/disclaimer conditions. | Generally permitted, but distribution of covered derivative works carries copyleft obligations. |
| Modification and distribution | Granted for the qualified personal, educational, 501(c)(3), or evaluation use; redistribution must retain specified notices, conditions, and disclaimers. | Broadly permitted with copyright and permission notice. | Permitted with source and same-license obligations when the GPL's distribution conditions apply. |
| Source disclosure | No general copyleft source-release requirement stated. | No general source-release requirement. | Source availability and corresponding-license obligations are central to covered distribution. |
| Transferability | Grant is expressly nontransferable. | Typical MIT grants are broad and do not use this purpose/user gate. | Typical GPL grants are broad to recipients, subject to copyleft conditions. |
| Contributor position | Contributor keeps copyright but grants a perpetual worldwide royalty-free license to licensors and recipients under the same terms; exceptions must be agreed in advance. | Usually governed by the repository's contribution terms, not by MIT itself. | Usually governed by the project’s contribution terms; GPL affects downstream distribution. |
| Compliance risk | Automatic termination on violation and a clear commercial-license boundary. | Primarily notice/disclaimer compliance. | Copyleft compliance and source/corresponding-license requirements on distribution. |

These are category comparisons, not a substitute for counsel reviewing a
particular distribution, hosted service, integration, or contribution.

## What a buyer or contributor can and cannot do

### A buyer or user can, when an applicable grant covers the use

- Use the Software within the applicable personal, non-business,
  noncommercial-educational, qualifying 501(c)(3), or 30-day commercial
  evaluation scope.
- Copy, modify, merge, publish, and distribute within that scope, while
  preserving the required notices, conditions, and disclaimers.
- Ask Business Handyman, LLC about a separate paid commercial license when the
  use is not covered or the evaluation period is ending.

### A buyer or user cannot assume

- That source visibility means unrestricted commercial use.
- That a commercial evaluation renews, becomes perpetual, or continues after
  30 consecutive days without a separate paid license.
- That a private K-12 school qualifies as an Educational Organization under the
  text without prior written permission.
- That a 501(c)(3) exemption applies to commercial use unrelated to directly
  benefiting an educational organization or accredited teacher.
- That the grant is transferable to another organization.
- That redistributed packages may omit the copyright notice, conditions, or
  disclaimers.
- That the license provides a warranty or permits continued use after a
  violation terminates the grant.

### A contributor can and should understand

- The contributor retains copyright in the contribution.
- By contributing, the contributor grants the licensors and all recipients a
  perpetual, worldwide, royalty-free license to use, modify, and distribute the
  contribution under the Hummingbird terms.
- Any exception must be negotiated before the contribution is made.

## Go-to-market implications

1. Lead with the narrow workflow: Apple Contacts ↔ one Google Sheet,
   bidirectional, no third editor.
2. Segment messaging by license eligibility instead of calling the product
   universally free.
3. Make the 30-day commercial evaluation and paid-license path visible before
   a commercial trial starts.
4. Treat educators and qualifying nonprofits as important audiences, but avoid
   implying that every school or nonprofit is covered.
5. Compare against workflows and named alternatives on boundary, direction,
   editing surface, and conflict visibility; avoid unsupported feature claims.
6. Preserve license notices in downloads, copies, and partner packages.
7. Present conflict freeze, size-bound fail-closed, and second-instance
   fail-stop as trust and safety differentiators, not as guarantees of data
   perfection.

## Bottom line

Cogwheel's List has a credible niche where Apple Contacts is the human editing
home and Google Sheets is the shared operational view. Its strongest message is
the disciplined bridge: two existing editing surfaces, one selected Sheet, and
explicit behavior when synchronization is unsafe. The principal marketing
constraint is the Hummingbird License v1.6 U.S. Edition: it is source-available
with no carve-outs in the project specification, but it is not MIT-like free
commercial licensing. Qualified users have defined grants; other commercial
organizations have a single evaluation period and then need a paid license.
