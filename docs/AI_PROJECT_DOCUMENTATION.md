# AI-Assisted Software Project Documentation

## Project Title
Job Fit Analyzer

## Objective
Create an easy-to-use career tool that highlights skills mentioned in job postings and compares them with a sample candidate profile.

## Implementation
The tool is located in `index.html` under the **AI Project** section. It uses HTML, CSS and browser JavaScript. No account, paid API or server is required.

## Functionality
1. The user pastes a job description.
2. The application checks minimum input length.
3. A controlled dictionary of technical/business terms is matched against the posting.
4. Matching terms are compared against a sample set of skills.
5. The application displays keyword overlap and potential gaps.

## AI Assistance
AI tools assisted with planning, writing, reviewing, and refining code. **The application does not use a machine-learning model or generative AI at runtime**; its matching is deterministic.

## Test Cases
- Blank input or fewer than 30 characters: validation message.
- Posting containing multiple known profile skills: matched terms displayed.
- Posting containing unfamiliar technical terms from the dictionary: potential gaps displayed.
- Job posting without recognized terms: zero overlap, no crash.
- Input with HTML-like text: results escaped before rendering.

## Limitations
- Finite list of keywords.
- Does not infer synonyms or meaning.
- Sample self-reported skills are not independently validated.
- The overlap score does not determine candidate qualifications or hiring outcomes.

## Future Improvements
Allow skill selection, store user preferences locally, add evidence-based skill explanations, and test with a larger set of job descriptions.
