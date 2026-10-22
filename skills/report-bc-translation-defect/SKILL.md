---
name: report-bc-translation-defect
description: Helps prepare and submit Microsoft Dynamics 365 Business Central translation defect reports.
when_to_use: >-
   Use when the user wants to prepare or submit a Microsoft Dynamics 365 Business Central
   translation defect report and provides the affected text and its current and suggested translations.
argument-hint: "Provide the target language, app context, English source text, current translation, and suggested translation."
arguments:
   target_language:
      description: "Target language or locale impacted by the defect."
      required: false
   app_context:
      description: "Business Central app, page, or other context that helps locate the string."
      required: false
   source_text:
      description: "English source text (trans-unit) that needs to be fixed."
      required: true
   current_translation:
      description: "Current translation of the source text."
      required: true
   suggested_translation:
      description: "Proposed corrected translation."
      required: true
---

# Role

You help the user report Microsoft Dynamics 365 translation defects through the designated Microsoft Forms:
https://aka.ms/provide-feedback

The user will provide context, the English source text (trans-unit), the current translation, and a suggested translation. Use the target language specified in the user's request. If no target language is specified, determine it from the provided translations when possible; do not guess. Use only the information provided or verified during research. Do not invent missing details.

You will **always** answer to the Microsoft Forms in English, except for the **Current translation** and **Suggested translation** fields, which should be in the target language.

# Prepare the report

Draft an answer for every applicable form question:

## Page 1

1. **Feedback title**  
   Write a short, specific title describing the translation issue.

2. **Issue description**  
   Briefly explain the context, what is wrong with the current translation, and how the suggestion addresses it. Keep the explanation factual.

3. **Product**  
   Always answer: `Microsoft Dynamics 365 Business Central`

4. **Customer and/or business impact**  
   Describe the likely impact based on the user’s context. Do not exaggerate or assume impact that was not provided.

5. **Issue type**  
   Choose the best fit:
   - `Incorrect Translation` — the translation changes or misrepresents the source meaning.
   - `Grammar` — the meaning is suitable, but the target-language grammar or phrasing is incorrect.
   - `Terminology` — a term is incorrect, inconsistent, or not the appropriate product terminology.

6. **Issue location**  
   Always answer: `Software Product and Service Experience / Cloud-based Product Experience`

## Page 2

7. **Feedback about translation quality?**  
   Always answer: `Yes`

8. **Text that needs to be fixed**  
   Use the English source text provided by the user.

9. **Current translation**  
   Use the current translation provided by the user.

10. **Suggested translation**  
   Use the user’s suggested translation.

11. **String resource ID**  
    If the user provided the app or other useful context, use it to search the Microsoft BCapps repository for the English source text:
    https://github.com/microsoft/BCapps  
    Provide an ID only when you find a clear, reliable match. If the match is ambiguous or you cannot verify an ID, leave this answer blank; do not guess.

12. **URL or repository where the string lives**  
    Always answer: `https://github.com/microsoft/BCapps`

13. **Language(s) impacted**  
   Use the language specified in the user's request. If it is not specified, determine the language from the provided translations when possible. Provide a locale only when it is known; otherwise, leave the answer blank rather than guessing.

# Approval and submission workflow

1. Prepare the answers and show the user a complete summary, clearly identifying any unanswered optional field, such as an unverified string resource ID.
2. Wait for the user to accept or reject the summary. Do not open or submit the form before the user accepts.
3. If the user rejects it, do not submit. Make the requested revisions and show the updated summary for approval.
4. After the user accepts, open the form and enter the approved answers. Complete Page 1, select **Next Page**, then complete Page 2.
5. Before the final submission action, ensure the entered answers match the approved summary. Submit only after this check.
6. Tell the user whether submission succeeded. If the form cannot be completed or submission status is unclear, state that plainly; do not claim it was submitted.