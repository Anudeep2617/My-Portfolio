# Detailed Guide to Different Style Guides for Technical Writers

## 1. What Is a Style Guide?

A style guide defines consistent rules for writing and presenting information. It helps writers maintain consistency in grammar, punctuation, capitalization, terminology, formatting, tone, and document structure.

For example, without a style guide, different writers might use “Log in,” “Login,” and “Sign in” inconsistently. A style guide identifies the preferred term and explains when to use it.

A documentation team may use several guides together:

- A primary language and editorial guide.
- A technical documentation style guide.
- An API documentation standard.
- A product-specific terminology guide.
- Accessibility and inclusive-language guidance.
- Company-specific templates and review rules.

A style guide explains **how information should be communicated**. It does not, by itself, verify whether the technical information is correct.

## 2. Major Style Guides

### 2.1 Microsoft Writing Style Guide

**Main focus:** Software documentation, user-facing content, cloud products, UI text, and developer content.

It emphasizes clear, concise, user-focused language.

**Useful for:**
- Product and user guides.
- Installation guides.
- Troubleshooting content.
- Help documentation.
- UI instructions.

Official guide: <https://learn.microsoft.com/en-us/style-guide/welcome/>

### 2.2 Google Developer Documentation Style Guide

**Main focus:** Developer-focused documentation, code examples, conceptual explanations, procedures, and technical tutorials.

It emphasizes direct language, consistent terminology, and content that is easy to scan.

**Useful for:**
- API documentation.
- SDK documentation.
- Developer guides.
- Integration guides.
- Technical tutorials.

Official guide: <https://developers.google.com/style>

### 2.3 The Chicago Manual of Style (CMOS)

**Main focus:** General editorial conventions, including grammar, punctuation, capitalization, quotations, citations, and publishing practices.

It is a broad editorial reference rather than a software-specific documentation guide.

**Useful for:**
- Editorial questions.
- Long-form technical content.
- White papers and publications where the organization adopts Chicago conventions.

Official website: <https://www.chicagomanualofstyle.org/>

### 2.4 Associated Press (AP) Stylebook

**Main focus:** Journalism, media, and public-facing communications.

It covers editorial conventions such as grammar, numbers, dates, abbreviations, and names.

**Useful for:**
- Corporate communications.
- Announcements.
- Press releases.
- Editorial content.

It is not usually the primary guide for detailed software API references.

Official website: <https://www.apstylebook.com/>

### 2.5 IBM Style Guide

**Main focus:** Technical content, enterprise software documentation, information design, terminology, and task-oriented instructions.

**Useful for:**
- Enterprise product documentation.
- Complex technical procedures.
- Technical support content.
- Structured information.

IBM documentation: <https://www.ibm.com/docs/en/ibm-style>

### 2.6 APA and MLA Styles

The American Psychological Association (APA) and Modern Language Association (MLA) publish style guidance primarily for academic writing, citations, references, and research publications.

**Useful for:**
- Research papers.
- Academic publications.
- Technical content requiring formal citations.

They are less commonly used as the main style guides for day-to-day software product documentation.

- APA Style: <https://apastyle.apa.org/>
- MLA Style Center: <https://style.mla.org/>

### 2.7 Quick Comparison

| Style guide | Main focus | Typical use |
|---|---|---|
| Microsoft Writing Style Guide | Software and user-facing content | Product guides, UI instructions, help content |
| Google Developer Documentation Style Guide | Developer documentation | APIs, tutorials, integration guides |
| Chicago Manual of Style | General editorial conventions | Long-form content and publishing |
| AP Stylebook | Journalism and communications | Press releases and announcements |
| IBM Style Guide | Enterprise technical content | Enterprise product and support documentation |
| APA and MLA | Academic writing and citations | Research and academic publications |

**Important:** Do not combine rules from different guides arbitrarily. Follow the organization's primary guide and use other references only when appropriate.

## 3. Microsoft, Google, and IBM: Practical Comparison

| Area | Microsoft | Google | IBM |
|---|---|---|---|
| Main focus | Software and user-facing content | Developer documentation | Enterprise technical content |
| Tone | Friendly, direct, conversational | Conversational and practical | Clear, consistent, globally appropriate |
| Headings | Follow the guide's conventions | Generally uses sentence case | Follow IBM's documented conventions |
| Instructions | Clear, action-oriented steps | Task-oriented, direct instructions | Structured, consistent procedures |
| Code and UI formatting | Consistent technical formatting | Explicit code and UI conventions | Consistent markup and presentation |
| Typical use | Product and help documentation | APIs, tutorials, developer guides | Enterprise product documentation |

The official guides provide detailed rules. An organization's own approved rules and product terminology take precedence where specified.

## 4. Important Style-Guide Rules

### 4.1 Voice and Tone

- **Voice** is the consistent personality of the writing.
- **Tone** changes according to the context and audience.

| Situation | Weak writing | Clearer writing |
|---|---|---|
| Procedure | The user should now proceed to click the Save button. | Select **Save**. |
| Explanation | It is to be noted that the application supports SSO. | The application supports SSO. |
| Error message | Oops! Something went terribly wrong! | The connection failed. Check the server URL and try again. |
| Warning | You must be careful when doing this. | **Warning:** This action deletes the configured identity source. |

The goal is to communicate clearly without unnecessary words or exaggerated language.

### 4.2 Active Voice and Passive Voice

**Active voice** makes the person or system performing an action clear.

- Active: The administrator configures the identity source.
- Passive: The identity source is configured by the administrator.

Use active voice when it makes instructions clearer.

Passive voice is not always incorrect:

- Active: The server returns a `401 Unauthorized` response.
- Passive: The request is rejected if the token is invalid.

Choose the sentence that communicates the relevant action or condition most clearly.

### 4.3 Sentence Case and Title Case

**Sentence case:** Capitalize the first word and proper nouns.

Example: `Configure the identity source`

**Title case:** Capitalize major words according to the selected title-case convention.

Example: `Configure the Identity Source`

Google's developer documentation guide uses sentence case for headings and titles.

Example Markdown structure:

```markdown
# Configure the identity source

## Prerequisites

## Configure the connection

## Verify the configuration
```

Heading levels represent information hierarchy; capitalization is a separate style decision.

Do not change the exact capitalization of product names, commands, API parameters, UI labels, or other product-defined identifiers to match a general heading rule.

### 4.4 UI Terminology and Formatting

UI instructions explain how users interact with an application.

Suppose the application contains a button labeled **Create Identity**.

1. Open the **Identity Sources** page.
2. Select **Create Identity**.
3. Enter the required details.
4. Select **Save**.

Common conventions include:

- Use the exact UI label.
- Follow the guide's formatting for buttons, menus, tabs, and fields.
- Use the same term for the same control throughout the documentation.
- Do not invent labels or change the wording shown in the application.
- Verify the UI because labels can change between product versions.

### 4.5 Terminology and Word Choice

Terminology management is especially important when documenting complex enterprise products.

| Preferred term | Avoid inconsistent alternatives |
|---|---|
| Sign in | Log in, Login, Sign-on, unless product terminology requires them |
| Select | Click on, Press, Hit, when the standard calls for Select |
| Identity source | Identity provider, connector, source, when these mean different things |
| API endpoint | API URL, API path, when a more specific term is needed |
| Administrator | Admin, system operator, when they refer to the same defined role |

These are examples, not universal prohibitions. The correct term depends on the product and its established terminology.

A terminology database or word list can record:

- Preferred term.
- Definition.
- Approved abbreviations.
- Terms to avoid.
- Capitalization and plural forms.
- Product-specific meaning.
- First-use requirements.

### 4.6 Punctuation and Numbers

Style guides establish consistent rules for punctuation, lists, numbers, dates, abbreviations, and units.

For example:

- Heading: `Configure the server`
- Complete sentence: `Configure the server before starting the application.`

Headings generally do not need a trailing period under Google's conventions. Complete sentences normally do.

Other decisions to standardize include:

- Whether to use the serial comma.
- How to format dates and times.
- How to write percentages, sizes, and units.
- Whether list items end with periods.
- How to expand abbreviations at first use.
- Whether to use American or British English.

For example, `03/04/2026` can mean March 4 or April 3, depending on the date convention. Writing `4 March 2026` or `March 4, 2026` avoids ambiguity.

### 4.7 Formatting Code, Commands, and Filenames

Technical documentation must distinguish normal prose from literal technical values.

| Content | Example |
|---|---|
| Filename | `application.properties` |
| API parameter | `identityId` |
| HTTP method | `GET` |
| HTTP status code | `403` |
| Command | `systemctl status httpd` |
| Placeholder | `<identity-id>` |
| Code sample | Fenced code block |

Example:

To retrieve an identity, send a `GET` request to the identity endpoint and provide the required authentication token.

```http
GET /identities/{identityId}
Authorization: Bearer <access-token>
```

The code formatting distinguishes technical identifiers and commands from explanatory prose.

The request above is illustrative. Actual endpoint paths, parameters, and authentication requirements must come from the product's API specification.

### 4.8 Lists, Tables, and Procedures

Use the format that helps the reader find information quickly.

- **Numbered lists:** Ordered steps.
- **Bulleted lists:** Unordered items.
- **Tables:** Structured comparisons or parameter details.
- **Warnings and notes:** Important information that should stand out.

Example procedure:

**Restart the service**

1. Open a terminal.
2. Check the service status:

   ```bash
   sudo systemctl status httpd
   ```

3. Restart the service:

   ```bash
   sudo systemctl restart httpd
   ```

4. Verify that the service is running.

Use a prerequisites section when users must complete setup before starting a procedure. Do not hide essential prerequisites in the middle of a long sequence.

## 5. Specialized Standards for Technical Writers

A general writing style guide is only one part of a documentation workflow. Other standards address specific content types and technical requirements.

### 5.1 DITA

**DITA** stands for **Darwin Information Typing Architecture**.

It is a standard for structuring, organizing, reusing, and publishing technical content. It supports topic-based authoring, such as:

- Concepts.
- Tasks.
- Reference topics.

DITA is primarily a content architecture and authoring standard, not a grammar guide.

Official resources: <https://www.oasis-open.org/committees/dita/>

### 5.2 Company-Specific Style Guides

Organizations often extend a general guide with:

- Product terminology.
- Heading templates.
- Release-note conventions.
- Screenshot requirements.
- Versioning rules.
- Approval workflows.
- Accessibility requirements.
- Document-specific templates.

These rules are often the most important ones to follow on the job.

### 5.3 API Documentation Conventions and OpenAPI

API documentation conventions cover:

- Endpoint descriptions.
- HTTP methods.
- Parameters and schemas.
- Request and response bodies.
- Authentication and authorization.
- Error responses.
- Examples.
- Consistent technical terminology.

**OpenAPI** is a machine-readable API description specification, not a general writing style guide. It can be used alongside editorial standards such as Microsoft or Google.

Official specification: <https://spec.openapis.org/oas/latest.html>

### 5.4 Accessibility Standards

Accessibility guidance helps people with disabilities use digital content. Relevant practices include:

- Meaningful link text.
- Appropriate heading structure.
- Alternative text for informative images.
- Accessible tables.
- Clear language and instructions.

**WCAG** stands for **Web Content Accessibility Guidelines**. WCAG is a web accessibility standard, not a grammar style guide.

Official resources: <https://www.w3.org/WAI/standards-guidelines/wcag/>

## 6. Which Style Guide Should You Use for Each Document?

| Document type | Recommended starting point | Additional rules |
|---|---|---|
| User guide | Microsoft or Google | Product terminology and UI conventions |
| Installation guide | Microsoft or Google | Commands, configuration, and prerequisites |
| API reference | Google or Microsoft | OpenAPI specification and API templates |
| Developer integration guide | Google | Code samples, authentication, and errors |
| Release notes | Company-specific guide, supported by Microsoft or Google | Versioning, issue IDs, feature changes, known issues |
| Troubleshooting guide | Microsoft or Google | Standardized error, cause, and resolution formats |
| Knowledge base article | Microsoft or Google | Support templates and search-friendly headings |
| Security documentation | Company-specific guide plus a general technical style guide | Accurate security terminology and approved warning formats |

There is no universal rule that one guide must be used for every document. The company may mandate IBM Style, Microsoft, Google, or an internal guide.

A release-note template might require sections such as *Feature Enhancements*, *Resolved Issues*, and *Known Issues*. Those section names are product-specific conventions, not requirements imposed by a general style guide.

## 7. How to Create a Company-Specific Style Guide

A practical style guide can use the following structure.

1. **Purpose and scope:** Which products, audiences, and documents does the guide cover?
2. **Language and grammar:** Voice, tone, active voice, sentence length, and spelling.
3. **Capitalization:** Headings, product names, UI labels, acronyms, and technical terms.
4. **Formatting:** Bold, italics, code font, links, tables, images, and warnings.
5. **Terminology:** Preferred terms, definitions, approved abbreviations, and alternatives to avoid.
6. **Document structure:** Templates for user guides, installation guides, API references, and release notes.
7. **Technical accuracy:** Rules for validating commands, API parameters, examples, configuration settings, and error codes.
8. **Accessibility and localization:** Descriptive links, image alt text, clear language, and consistent units.
9. **Review and maintenance:** Ownership, version control, review responsibilities, and update frequency.

### Example: Terminology Decision

Suppose different writers use `Identity IQ`, `IdentityIQ`, and `Identity IQ product`.

The style guide should specify the official product name, where it must be used, and whether an abbreviation is allowed after first use.

This prevents inconsistent naming across user guides, release notes, and API documentation.

## 8. How to Apply a Style Guide During Documentation Review

### Step 1: Identify the Governing Guide

Check the company guide, product terminology, document template, and required technical standards.

### Step 2: Review Structure and Readability

Check headings, prerequisites, task sequence, sentence clarity, tables, and warnings.

### Step 3: Check Consistency

Validate terminology, capitalization, punctuation, formatting, and cross-references.

### Step 4: Verify Technical Accuracy

Confirm product behavior, UI labels, commands, API parameters, responses, and examples with authoritative technical sources or the relevant subject-matter expert (SME).

### Step 5: Record and Resolve Deviations

Use a review checklist, tracked changes, or Git pull-request comments. Update the guide when a recurring rule is missing.

A style guide can improve consistency, but it cannot verify whether a feature actually works. Technical validation remains a separate responsibility.

## 9. Learning Plan for Technical Writers

Follow this order to build practical skills:

1. **Microsoft Writing Style Guide:** Learn voice, tone, capitalization, UI instructions, and numbers.
2. **Google Developer Documentation Style Guide:** Learn headings, code formatting, lists, links, and developer content.
3. **Company-specific style-guide design:** Build terminology rules and document templates.
4. **OpenAPI documentation conventions:** Understand how editorial rules work alongside YAML and API schemas.
5. **Documentation review practice:** Review a sample API guide and release note against a checklist.

## 10. Interview Question: Which Style Guides Have You Used?

Explain the guides you have actually used. Do not claim professional experience with a guide simply because you have studied it.

Sample answer:

> I understand the purpose of technical writing style guides and how they help maintain consistency across product documentation. Microsoft and Google provide useful guidance for voice, tone, terminology, headings, UI instructions, and technical formatting. I also understand that company-specific guidelines take precedence for product terminology, templates, and release-note conventions. For API documentation, I apply these editorial principles alongside the API specification and validate technical details with engineering teams. My focus is on clear, consistent, accurate, and user-oriented documentation.

## 11. Recommended Starting Point

Start with the Microsoft Writing Style Guide, then study the Google Developer Documentation Style Guide. Practise applying both to an installation guide, an API reference, and a release note.

Practical application will provide more value than trying to memorize multiple style guides.

## Glossary

| Term | Definition |
|---|---|
| API | Application Programming Interface |
| APA | American Psychological Association |
| AP | Associated Press |
| CMOS | Chicago Manual of Style |
| DITA | Darwin Information Typing Architecture |
| HTTP | Hypertext Transfer Protocol |
| MLA | Modern Language Association |
| OAS | OpenAPI Specification |
| SDK | Software Development Kit |
| SME | Subject-Matter Expert |
| SSO | Single Sign-On |
| UI | User Interface |
| WCAG | Web Content Accessibility Guidelines |
| YAML | YAML Ain't Markup Language |
