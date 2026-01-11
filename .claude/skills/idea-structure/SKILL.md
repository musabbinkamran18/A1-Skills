---
name: idea-structure
description: Takes unstructured notes or messy ideas and organizes them into a clear, logical structure. Use when the user has scattered thoughts, brainstorming notes, or disorganized content that needs to be structured coherently.
allowed-tools: Read
---

# Idea Structure

Transforms unstructured notes and messy ideas into clear, logical structures with organized sections and headings.

## Instructions

When the user provides unstructured notes or messy ideas:

1. **Analyze the input** to identify:
   - Main themes or topics
   - Key concepts and ideas
   - Relationships between ideas
   - Natural groupings or categories
   - Logical flow or sequence

2. **Organize the content** by:
   - Grouping related ideas together
   - Creating a hierarchical structure (main points → sub-points)
   - Arranging topics in a logical order
   - Identifying appropriate section headings
   - Maintaining all original ideas without adding new ones

3. **Present the results** in this format:

   **Structured Outline:**
   ```
   I. Main Section
      A. Subsection
         1. Point
         2. Point
      B. Subsection

   II. Main Section
       A. Subsection
       B. Subsection
   ```

   **Section Headings with Descriptions:**
   - **Section 1 Title:** Brief description of what this section covers
   - **Section 2 Title:** Brief description of what this section covers
   - **Section 3 Title:** Brief description of what this section covers

   **Reasoning for the Structure:**
   - Explain why this particular organization makes sense
   - Describe the logical flow (e.g., "chronological order", "general to specific", "problem to solution")
   - Highlight how related concepts are grouped
   - Note any patterns or themes that emerged

4. **Follow these rules strictly:**
   - Do NOT add new ideas, examples, or content
   - Do NOT elaborate or expand on the original ideas
   - Do NOT omit any of the user's original ideas
   - Only reorganize and structure what was provided
   - Improve clarity through organization, not through adding content
   - Keep the structure simple and logical

5. **Handle different input types:**
   - If given a file path, use the Read tool to load the content first
   - If given inline text, work with it directly
   - If given bullet points, preserve all points while reorganizing
   - If given paragraphs, extract key ideas and structure them

## Examples

### Example 1: Meeting Notes

**User:** "Structure these notes: need to update website, team mentioned budget concerns, deadline is March, Sarah will handle design, also need to fix the login bug, marketing wants new landing page, server costs are high, John suggested cloud migration"

**Response:**

**Structured Outline:**
```
I. Project Tasks
   A. Website Updates
      1. New landing page (marketing request)
      2. Fix login bug
   B. Team Assignments
      1. Sarah - design responsibilities

II. Budget & Infrastructure
    A. Concerns
       1. Budget concerns raised by team
       2. High server costs
    B. Proposed Solutions
       1. Cloud migration (suggested by John)

III. Timeline
     A. Deadline: March
```

**Section Headings with Descriptions:**
- **Project Tasks:** Website development work including new features and bug fixes, along with team member assignments
- **Budget & Infrastructure:** Financial concerns and technical infrastructure issues, plus proposed solutions
- **Timeline:** Key dates and deadlines for project completion

**Reasoning for the Structure:**
- Organized by **category** (what, resources/costs, when) for clarity
- Grouped related tasks together (website work in one section)
- Separated concerns (tasks vs budget) to make action items clear
- Paired problems with solutions (server costs → cloud migration)
- Timeline isolated at the end as it applies to the overall project
- This structure allows stakeholders to quickly find relevant information by topic

### Example 2: Brainstorming Session

**User:** "Organize this: customer complaints about slow checkout, ideas for loyalty program, mobile app crashes on Android, competitors offering free shipping, could add product recommendations, payment gateway timeouts, holiday sale planning, Instagram ads performing well, cart abandonment rate is 68%, need better product photos"

**Response:**

**Structured Outline:**
```
I. Current Issues
   A. Technical Problems
      1. Slow checkout process
      2. Mobile app crashes on Android
      3. Payment gateway timeouts
   B. Business Metrics
      1. Cart abandonment rate at 68%

II. Competitive Landscape
    A. Competitor advantages
       1. Free shipping offers

III. Improvement Opportunities
     A. Product Enhancements
        1. Add product recommendations
        2. Improve product photos
     B. Customer Retention
        1. Implement loyalty program
     C. Marketing Initiatives
        1. Instagram ads performing well
        2. Plan holiday sale
```

**Section Headings with Descriptions:**
- **Current Issues:** Technical problems affecting user experience and concerning business metrics that need immediate attention
- **Competitive Landscape:** What competitors are doing that may be affecting our performance
- **Improvement Opportunities:** Proposed enhancements across products, customer retention, and marketing efforts

**Reasoning for the Structure:**
- Follows a **problem-to-solution** flow (issues first, then improvements)
- Technical problems grouped together for the development team
- Separated competitive analysis to provide context for decisions
- Improvement opportunities organized by functional area (product, retention, marketing)
- Cart abandonment placed with issues since it's a problem metric, not just data
- This structure supports prioritization: fix critical issues, address competition, then implement improvements

### Example 3: Research Notes

**User:** "Structure the notes in research.txt"

**Response:**
[Use Read tool to load research.txt, then apply the same structuring process]

**Structured Outline:**
[Organized outline based on file contents]

**Section Headings with Descriptions:**
[Headings with descriptions]

**Reasoning for the Structure:**
[Explanation of organizational logic]

## Notes

- **Never add new ideas** - only organize what's provided
- **Preserve all original content** - don't omit anything
- **Clarity through organization** - structure alone should improve understanding
- If the ideas are already well-structured, acknowledge this and provide minor refinements
- Focus on creating a structure that makes information easy to find and understand
- The goal is to reveal the logical relationships between ideas that were already present
- Different organizational patterns may be appropriate: chronological, hierarchical, categorical, problem-solution, cause-effect, etc.
- Choose the structure that best fits the natural relationships in the content
