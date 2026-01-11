---
name: text-formatter
description: Transforms vague, unclear, or poorly written text into clear, well-structured, and professional language. Use when the user needs to improve text quality, refine writing, or make content more readable and professional.
allowed-tools: Read
---

# Text Formatter

Transforms vague, unclear, or poorly written text into clear, well-structured, and professional language while preserving the original meaning.

## Instructions

When the user provides text to format or improve:

1. **Analyze the input text** to identify issues:
   - Unclear or confusing sentences
   - Poor word choice or redundancy
   - Weak sentence structure or flow
   - Tone inconsistencies
   - Grammatical errors
   - Readability problems

2. **Transform the text** by:
   - Rewriting unclear sentences for clarity
   - Improving word choice and eliminating redundancy
   - Enhancing sentence flow and structure
   - Adjusting tone to be professional and appropriate
   - Fixing grammatical and punctuation errors
   - Preserving the original meaning and intent

3. **Present the results** in this format:

   **Original Text:**
   [Show the original text]

   **Improved Text:**
   [Show the rewritten version]

   **What Was Improved:**
   - List specific improvements made (e.g., "Replaced passive voice with active voice", "Simplified complex sentences", "Eliminated redundant phrases")

   **Suggestions for Further Enhancement:**
   - Provide 2-4 actionable suggestions to make the text even better
   - Focus on clarity, tone, impact, or structure
   - Be specific and practical

4. **Handle different input types:**
   - If given a file path, use the Read tool to load the content first
   - If given inline text, work with it directly
   - If given multiple paragraphs, maintain logical organization
   - If context is needed (e.g., audience, purpose), ask the user first

5. **Maintain professionalism:**
   - Keep the tone appropriate for professional communication
   - Preserve technical accuracy in specialized content
   - Respect the user's voice while improving clarity
   - Don't oversimplify if complexity is necessary

## Examples

### Example 1: Email Improvement

**User:** "Format this: hey john, i wanted to reach out about the thing we talked about last week. i think we should maybe do it differently because the current way isnt really working that great and people are getting confused."

**Response:**

**Original Text:**
"hey john, i wanted to reach out about the thing we talked about last week. i think we should maybe do it differently because the current way isnt really working that great and people are getting confused."

**Improved Text:**
"Hi John, I'm following up on our discussion from last week regarding the project workflow. I recommend we revise our current approach, as it's causing confusion among team members and isn't delivering the expected results."

**What Was Improved:**
- Capitalized proper nouns and sentence beginnings
- Replaced vague "the thing" with specific "the project workflow"
- Changed uncertain "maybe do it differently" to confident "I recommend we revise"
- Clarified "current way isn't working" with specific outcomes
- Improved overall professionalism and clarity

**Suggestions for Further Enhancement:**
1. Add a specific proposal for the new approach after stating the problem
2. Include a call-to-action (e.g., "Could we schedule a brief meeting to discuss alternatives?")
3. Quantify the confusion if possible (e.g., "Three team members have raised concerns")
4. Consider adding a timeline or urgency indicator if applicable

### Example 2: Documentation Improvement

**User:** "The system does stuff when you click the button and then things happen in the background which processes data."

**Response:**

**Original Text:**
"The system does stuff when you click the button and then things happen in the background which processes data."

**Improved Text:**
"When you click the Submit button, the system initiates a background process that validates and transforms the input data."

**What Was Improved:**
- Replaced vague "does stuff" with specific "initiates a background process"
- Changed "things happen" to concrete actions ("validates and transforms")
- Identified the specific button ("Submit button")
- Improved sentence structure for clarity
- Used more precise technical vocabulary

**Suggestions for Further Enhancement:**
1. Specify what happens after the data is processed (e.g., "and stores it in the database")
2. Add information about user feedback (e.g., "displays a confirmation message")
3. Mention approximate processing time if relevant
4. Consider adding error handling information

### Example 3: File-based Formatting

**User:** "Format the text in draft.txt"

**Response:**
[Use Read tool to load draft.txt, then apply the same formatting process]

## Notes

- Always preserve the original meaning and intent
- Be respectful of the user's voice and style preferences
- For highly technical content, maintain accuracy while improving clarity
- If the text is already well-written, acknowledge this and provide minor refinements
- Focus on practical improvements that genuinely enhance communication
