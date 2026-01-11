---
name: clarity-checker
description: Reviews written content to determine whether it is clear, well-structured, and ready to be shared. Evaluates clarity, completeness, and audience understanding, identifies confusion points, and provides actionable improvement suggestions with a final readiness verdict.
allowed-tools: Read
---

# Clarity Checker

Reviews written content to evaluate its clarity, structure, and readiness for sharing, providing a comprehensive assessment with specific improvement recommendations.

## Instructions

When the user provides text to review for clarity:

1. **Analyze the content** across these dimensions:
   - **Clarity:** Are sentences clear and easy to understand? Any ambiguous or confusing parts?
   - **Structure:** Is the content well-organized with logical flow?
   - **Completeness:** Does it cover all necessary points? Any gaps or missing context?
   - **Audience appropriateness:** Is the tone and complexity level suitable for the intended audience?
   - **Precision:** Are terms well-defined? Any vague language or jargon issues?
   - **Coherence:** Do ideas connect logically? Smooth transitions between points?

2. **Identify specific issues** that may cause confusion:
   - Unclear statements or ambiguous phrasing
   - Missing definitions or unexplained concepts
   - Logical gaps or jumps in reasoning
   - Inconsistent terminology or tone
   - Overly complex sentences or unnecessary jargon
   - Missing context or background information
   - Weak or missing transitions
   - Structural problems (poor organization, unclear headings)

3. **Provide actionable suggestions** for each identified issue:
   - Be specific about what to change and why
   - Prioritize suggestions by impact (high/medium/low)
   - Offer concrete examples where helpful
   - Focus on improvements that enhance understanding

4. **Present the results** in this format:

   **Content Summary:**
   [1-2 sentences describing what the content is about and its purpose]

   **Clarity Assessment:**

   ✓ **Strengths:**
   - List what works well (2-4 points)
   - Acknowledge clear sections, good structure, effective explanations

   ⚠ **Issues Identified:**
   - **[Issue Category]:** Specific problem description
     - Impact: [High/Medium/Low]
     - Location: [Where in the text this occurs]
     - Why it matters: [How this affects reader understanding]

   **Actionable Recommendations:**
   1. **[Priority: High/Medium/Low]** - [Specific suggestion]
      - Current: [What it says now or what's missing]
      - Recommended: [What to do instead]
      - Benefit: [How this improves clarity]

   **Readiness Verdict:**

   Status: [Ready to Share / Needs Minor Revisions / Needs Significant Revisions / Not Ready]

   **Reasoning:** [2-3 sentences explaining the verdict based on the analysis]

   **Next Steps:** [Prioritized list of 2-3 most important actions to take before sharing]

5. **Handle different input types:**
   - If given a file path, use the Read tool to load the content first
   - If given inline text, work with it directly
   - If context is needed (e.g., intended audience, purpose, platform), ask the user first
   - Adjust assessment criteria based on content type (email, documentation, blog post, etc.)

6. **Calibrate feedback appropriately:**
   - Be constructive and specific, not just critical
   - Balance praise for strengths with actionable critique
   - Consider the content's purpose when assessing readiness
   - If the content is already excellent, acknowledge this clearly
   - Focus on meaningful improvements, not nitpicking

## Examples

### Example 1: Technical Documentation Review

**User:** "Check if this is ready to share: The API endpoint processes requests. You need to send data and it returns results. Make sure to include authentication."

**Response:**

**Content Summary:**
Brief technical documentation describing an API endpoint's functionality and basic usage requirements.

**Clarity Assessment:**

✓ **Strengths:**
- Mentions key components (endpoint, requests, authentication)
- Concise and attempts to cover the basics
- Identifies authentication as a requirement

⚠ **Issues Identified:**

- **Vague Language:** Multiple instances of unclear descriptions
  - Impact: High
  - Location: Throughout the entire text
  - Why it matters: Readers won't know which endpoint, what data format, or how to implement authentication

- **Missing Critical Details:** No specifics about implementation
  - Impact: High
  - Location: Entire document
  - Why it matters: Developers cannot implement the API without concrete examples and specifications

- **Poor Structure:** No organization or formatting
  - Impact: Medium
  - Location: Single paragraph format
  - Why it matters: Technical docs need clear sections for quick reference

- **Incomplete Information:** No error handling, response format, or examples
  - Impact: High
  - Location: Missing sections
  - Why it matters: Developers need to know what to expect in different scenarios

**Actionable Recommendations:**

1. **[Priority: High]** - Specify the exact endpoint and HTTP method
   - Current: "The API endpoint processes requests"
   - Recommended: "POST /api/v1/process - Processes data transformation requests"
   - Benefit: Developers know exactly what to call and how

2. **[Priority: High]** - Define the request/response data structure
   - Current: "send data and it returns results"
   - Recommended: Add a JSON example showing request payload structure and expected response format
   - Benefit: Eliminates ambiguity about data formats and field requirements

3. **[Priority: High]** - Explain authentication implementation
   - Current: "Make sure to include authentication"
   - Recommended: "Include a Bearer token in the Authorization header: `Authorization: Bearer YOUR_API_KEY`"
   - Benefit: Developers can implement authentication correctly on first try

4. **[Priority: Medium]** - Add structure with clear sections
   - Current: Single paragraph
   - Recommended: Use sections like "Endpoint", "Authentication", "Request Format", "Response Format", "Error Codes", "Example"
   - Benefit: Information is scannable and easier to reference

5. **[Priority: Medium]** - Include a complete working example
   - Current: No example provided
   - Recommended: Add a curl or code example showing a complete request and response
   - Benefit: Developers can test immediately and understand the full context

**Readiness Verdict:**

Status: **Not Ready**

**Reasoning:** While the content identifies the right topics, it lacks the specificity and detail needed for technical documentation. Developers would be unable to implement the API without guessing at critical details like endpoint URLs, data formats, and authentication methods. The vague language and missing examples make this unsuitable for sharing in its current form.

**Next Steps:**
1. Add specific endpoint URL, HTTP method, and complete request/response examples with actual JSON structures
2. Provide concrete authentication instructions with example headers or tokens
3. Organize content into clear sections (Overview, Authentication, Request, Response, Examples, Errors)

### Example 2: Business Email Review

**User:** "Is this ready to send to my team? Subject: Project Update. Hi everyone, we made progress on the thing we discussed. There are some issues but we're working on them. Let me know if you have questions. Thanks"

**Response:**

**Content Summary:**
A brief project update email to team members mentioning progress and ongoing issues.

**Clarity Assessment:**

✓ **Strengths:**
- Polite and professional tone
- Invites questions and feedback
- Acknowledges both progress and challenges

⚠ **Issues Identified:**

- **Vague References:** "the thing we discussed" and "some issues"
  - Impact: High
  - Location: Main body, sentences 1-2
  - Why it matters: Team members may not remember what specific project or issues you're referring to, leading to confusion or follow-up questions

- **Lack of Specificity:** No concrete details about progress or next steps
  - Impact: Medium
  - Location: Throughout
  - Why it matters: Team needs actionable information to understand status and plan their work

- **Missing Information:** No timeline, action items, or context
  - Impact: Medium
  - Location: Entire message
  - Why it matters: Recipients can't determine urgency or what's expected of them

**Actionable Recommendations:**

1. **[Priority: High]** - Specify what project you're discussing
   - Current: "the thing we discussed"
   - Recommended: "the customer portal redesign we discussed in Monday's meeting"
   - Benefit: Eliminates ambiguity and provides immediate context

2. **[Priority: High]** - Detail specific progress made
   - Current: "we made progress"
   - Recommended: "We completed the wireframes and received approval from the design team"
   - Benefit: Team understands concrete accomplishments

3. **[Priority: Medium]** - Identify specific issues and their status
   - Current: "There are some issues but we're working on them"
   - Recommended: "We encountered integration challenges with the payment gateway, but the dev team is implementing a workaround expected to complete by Friday"
   - Benefit: Transparency about problems and clear timeline for resolution

4. **[Priority: Medium]** - Add next steps or action items
   - Current: No action items mentioned
   - Recommended: Add a section: "Next Steps: Sarah will finalize the mockups by Wednesday, and we'll schedule a review session for Thursday afternoon"
   - Benefit: Team knows what's happening and when

5. **[Priority: Low]** - Make the subject line more specific
   - Current: "Project Update"
   - Recommended: "Customer Portal Redesign - Week of Jan 3 Update"
   - Benefit: Easier to find in email history and sets context before opening

**Readiness Verdict:**

Status: **Needs Significant Revisions**

**Reasoning:** While the tone is appropriate and professional, the email lacks essential details that would make it useful to recipients. The vague references and missing specifics mean team members will likely need to send follow-up questions rather than having the information they need. With revisions to add concrete details, this could become an effective update.

**Next Steps:**
1. Replace vague references with specific project names and details about what was accomplished
2. Clearly identify the issues encountered and the plan/timeline for resolving them
3. Add a "Next Steps" section with action items and owners

### Example 3: File-based Review

**User:** "Check if proposal.txt is ready to share with the client"

**Response:**
[Use Read tool to load proposal.txt, then apply the same clarity assessment process]

**Content Summary:**
[Summary based on file contents]

**Clarity Assessment:**
[Full assessment following the format above]

## Notes

- **Be thorough but constructive** - The goal is to help, not discourage
- **Context matters** - A casual email has different standards than formal documentation
- **Prioritize ruthlessly** - Not all issues are equally important
- **Be specific** - "Add more detail" is less helpful than "Specify which database and version"
- **Consider the audience** - What's clear to experts may confuse beginners
- **Readiness is relative** - Assess based on the content's purpose and intended recipient
- **Balance is key** - Acknowledge what works well while addressing issues
- **If content is excellent** - Say so clearly and provide only minor polish suggestions
- **Focus on clarity over style** - Unless style affects understanding, prioritize substance
