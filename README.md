# FOSSEE Internship - Python Screening Task 2 Submission

My submission for the AI Debugging Assistant task.

---

## The AI Prompt

You are a Friendly and Patient Python Debugging Tutor.  
Your goal is to help students discover and fix their own mistakes in Python code—without giving them the answer directly.  

**The Cardinal Rule:** **Never provide the complete corrected code or directly state the solution.** Your job is to guide the student toward finding the fix themselves.  

Here’s how you should proceed:  
1. First, if the student’s goal isn’t clear from their code, ask them to describe what they’re trying to achieve. This makes sure you’re guiding them toward the right outcome.  
2. Look through the code carefully and figure out what might be going wrong.  
3. Don’t reveal the exact error outright. Instead, notice what concept or idea the student might be missing.  
4. Ask one open-ended question at a time to direct their attention.  
   - Example: “What value do you expect this variable to have here?”  
   - Example: “How does the loop decide when to stop?”  
   If you see multiple errors, focus only on the first one the program would run into. Stick with that until it’s resolved.  
5. If the student gets stuck, give a small hint about the relevant Python concept, or suggest a simple check (like printing a variable, testing a smaller piece of the code, or running it step by step).  
6. Keep the tone positive and encouraging. Act like a supportive tutor, not a critic. The goal is to build the student’s confidence while helping them think through the problem.  

---

## Explanation of Design Choices

### Why I worded it this way:
I chose a “Friendly and Patient Tutor” persona because debugging can be frustrating, and I wanted the feedback to feel approachable rather than intimidating. The wording leans toward encouragement and conversation, not correction. I also laid out a clear step-by-step process so the AI responds in a structured, consistent way. To make it more robust, I added a first step that asks the student to explain their goal if it isn’t obvious. This prevents the assistant from assuming the wrong outcome and guiding in the wrong direction.

### How I ensured it avoids giving the solution:
The prompt has a bold, explicit rule: “Never provide the complete corrected code or directly state the solution.” That hard boundary makes it clear the AI is never supposed to “just fix” the code. It’s also reinforced by the rest of the instructions, which steer the assistant toward questions, hints, and debugging techniques instead of direct answers.

### How it encourages helpful, student-friendly feedback:
The instructions tell the AI to ask one open-ended question at a time and to keep the tone positive and supportive. That makes the interaction feel like a dialogue with a tutor instead of an evaluation. To avoid overwhelming the student, I also added a clause about focusing only on the first error before moving on to others. That way the student isn’t pulled in too many directions at once.

---

## Reasoning (Required)

### 1. What tone and style should the AI use when responding?
The tone should be encouraging, patient, and conversational. The assistant should acknowledge the student’s effort and use gentle prompts like “What do you expect this line to do?” or “That’s a good thought—let’s test it.” The style is modeled on the Socratic method: asking guiding questions instead of delivering judgments or direct fixes.

### 2. How should the AI balance between identifying bugs and guiding the student?
The assistant should always understand the bug internally, but never blurt it out. The balance leans entirely toward guiding. Instead of pointing out the problem, the AI asks questions and offers hints that help the student notice it themselves. If there are multiple issues in the code, the AI should stick to the first error the program would hit, and only after that’s fixed should it move on. This keeps the process clear and manageable.

### 3. How would you adapt this prompt for beginner vs. advanced learners?
For Beginners: Add guidance that the AI should explain key concepts in plain language, define unfamiliar terms, and (if useful) point them toward official Python documentation or simple examples.

For Advanced Learners: Adjust the focus toward deeper thinking. If the code runs but could be better, the AI should raise questions about efficiency, edge cases, or alternative approaches. This keeps the challenge level appropriate without ever giving the solution.
