# 💭 Reflection: Game Glitch Investigator

Answer each question in 3 to 5 sentences. Be specific and honest about what actually happened while you worked. This is about your process, not trying to sound perfect.

## 1. What was broken when you started?

- What did the game look like the first time you ran it?
- List at least two concrete bugs you noticed at the start  
  (for example: "the hints were backwards").

**Bug Reproduction Log**

Document at least 3 bugs you found. Add rows as needed.

| Input | Expected Behavior | Actual Behavior | Console Output / Error |
|-------|-------------------|-----------------|------------------------|
| 4|expected the codeto say higher since the secret was 23 | outputed lower, and continued to do so until I hit negative numbers| |
|pressed the new game button | allow me to guess again and play again|i was not allowed to play again and every attempt I made didn't lead into anything | |
|everytime I switched difficulties, the guessing range being told to me wasnt changing, but the range for the number was, it kept saying guess 1-100 when in reality the values were 1-20 | tell me 1-20 for normal mode| told me 1-100| |

---

## 2. How did you use AI as a teammate?

- Which AI tools did you use on this project (for example: ChatGPT, Gemini, Copilot)?
- Give one example of an AI suggestion that was correct (including what the AI suggested and how you verified the result).
- Give one example of an AI suggestion that was incorrect or misleading (including what the AI suggested and how you verified the result).

Ai was able to scan and recognize the source of my errors quickly, suggesting to invert logic for the higher and lower text. After trying ingame it was proven to not work since I needed the logic of the numbers itself to change aswell.

Ai was then able to scan for the logic of the guess in comparison to the actual number and change it. It suggested to redo the logic entirely and when executed it worked out well.
---

## 3. Debugging and testing your fixes

- How did you decide whether a bug was really fixed?
- Describe at least one test you ran (manual or using pytest)  
  and what it showed you about your code.
- Did AI help you design or understand any tests? How?

I tested ingame myself, then I used pytest to check the bugs.
1 test I did was trying to replicate the original bug the got me to an error, like the higher lower messages leading me to go over 100 or under 1. It showed me that my code could have game breaking errors arise from simple logic mistakes. Ai also helped design my test for the guessing logic by producing said test after I prompted it.

## 4. What did you learn about Streamlit and state?

- How would you explain Streamlit "reruns" and session state to a friend who has never used Streamlit?
Streamlit "reruns" are when the code resets back to the beginning after an action, but session states allow your code to remember the state in which your code is at so it doesn't have to rerun all the code over again.
---

## 5. Looking ahead: your developer habits

- What is one habit or strategy from this project that you want to reuse in future labs or projects?
  - This could be a testing habit, a prompting strategy, or a way you used Git.
- What is one thing you would do differently next time you work with AI on a coding task?
- In one or two sentences, describe how this project changed the way you think about AI generated code.
I want to  prompt Ai thoroughly and use an identity when prompting it.
1 thing I'd do differently is split up my requests for bug fixing to be seperate prompts so the AI can't confuse itself and mess up any of them.
This project made me realize that AI generated code isn't always reliable and required human intervention to be fully confirmed as both effective and trustworthy. Ai may also not understand logically what you are asking for unless you are specific in your prompts.