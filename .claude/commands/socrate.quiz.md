---
description: Generate assessment quizzes for knowledge points or lesson plans. Create quizzes with multiple choice (4 options), short answer, and true/false questions, including answer keys. Use Socratic-style questions where appropriate. Follow UbD principles for assessing understanding.
---

## User Input

```text
$ARGUMENTS
```

You **MUST** consider the user input before proceeding (if not empty).

## Role

You are a Socratic assessment designer. Design assessment quizzes to check understanding while using Socratic questions to deepen thinking.

## Core Principles

1. **Follow the learning contract** at all times
2. **Assess understanding, not memorization**
3. **Use Socratic questions to provoke deeper thinking**
4. **Keep answers clear and observable**
5. **Balance question types**

## Prerequisites

- `outlines/[topic]-outline.md` exists
- `lessons/[kp-id]-plan.md` or `lessons/[kp-id]-lesson.md` exists (optional)

## Execution Flow

### Step 1: Determine KP or Lesson Plan

**Input Methods**:

**Method 1 - KP-ID**:
```
/socrate.quiz "KP-1.1.1"
```

**Method 2 - Lesson plan path**:
```
/socrate.quiz "lessons/python-variables-lesson.md"
```

**Method 3 - Topic**:
```
/socrate.quiz "python-basics"
```

### Step 2: Analyze Content

From input, extract:
- Main concepts and terminology
- Learning objectives (EU/SWBAT)
- Common misconceptions
- Key knowledge points

### Step 3: Generate Quiz Questions

#### Multiple Choice (4 Options)

Generate 2-3 questions per KP:
- 1 basic concept question
- 1 application question
- 1 analysis/comparison question (if applicable)

```markdown
### Multiple Choice

1. **Which of the following is a valid Python variable name?**
   - A) `my-variable` ❌
   - B) `my_variable` ✅
   - C) `my variable` ❌
   - D) `1myvariable` ❌

2. **[Application] After executing `x = 5; x = x + 1`, what is the value of x?**
   - A) 5
   - B) 6 ✅
   - C) 5+1
   - D) Error

3. **[Analysis] Why can't Python variable names start with a number?**
   - A) Syntax rule, avoids parsing ambiguity ✅
   - B) Historical artifact
   - C) Performance concern
   - D) No reason
```

#### Short Answer

Generate 1-2 questions per KP:
- Open-ended questions
- Allow different answer paths

```markdown
### Short Answer

1. **Explain why variable names should be descriptive. What makes a variable name good or bad?**

   **Sample Answer**:
   - Good: descriptive like `user_age` vs bad: `x`
   - Consistency, avoiding magic numbers
   - Examples with explanations

2. **Socratic question: How are "variables" in programming languages similar to or different from "variables" in mathematics?**

   **Follow-up prompts**:
   - Math: unknown in equation, fixed after assignment
   - Programming: can be reassigned multiple times, stores changing values
   - Socratic follow-up: "If that's the case, what would you call a counter in a loop?"
```

#### True/False

Generate 2-3 questions per KP:
- Focus on key concepts and common misconceptions

```markdown
### True/False

1. **In Python, variables must be declared before they can be used.**
   - ❌ False: Python variables don't need pre-declaration, just assign to create
   - Key concept: Python is dynamically typed

2. **The variable names `total_score` and `totalScore` refer to the same variable in Python.**
   - ❌ False: Python is case-sensitive, these are different variables
   - Key concept: Case sensitivity

3. **Once a variable is assigned a value, its type is fixed forever.**
   - ❌ False: Python variables can be reassigned to different types
   - Key concept: Dynamic typing
```

### Step 4: Generate Answer Key

```markdown
## Answer Key

### Multiple Choice
1. B - `my_variable` is the only option following Python naming rules
2. B - x is first assigned 5, then x+1=6 is reassigned to x
3. A - Avoids parsing ambiguity, e.g., `123abc` could be parsed as number 123 plus identifier abc

### Short Answer
1. [See sample answer]
2. [Socratic discussion points]

### True/False
1. ❌ False - Python variables don't require pre-declaration
2. ❌ False - Python is case-sensitive
3. ❌ False - Python is dynamically typed
```

## Output Format

Save to `quizzes/[kp-id]-quiz.md`:

```markdown
---
kp_id: "KP-1.1.1"
topic: "Variables and Assignment"
difficulty: "easy"
estimated_time: "15-20min"
generated_date: "YYYY-MM-DD"
---

# Quiz: Variables and Assignment

**Knowledge Point**: KP-1.1.1
**Difficulty**: Easy
**Time**: 15-20 minutes

---

## Multiple Choice

1. [Question]
   - A) [Option]
   - B) [Option]
   - C) [Option]
   - D) [Option]

[... more questions ...]

## Short Answer

1. [Question]
   **Sample Answer**: [Answer outline]

2. [Question]
   **Prompts**: [Socratic follow-up prompts]

## True/False

1. [Statement]
   - ❌ False - [Explanation]
   - or
   - ✅ True - [Explanation]

[... more questions ...]

---

## Answer Key

### Multiple Choice
1. B - [Brief explanation]
2. A - [Brief explanation]
[...]

### Short Answer
1. [Sample answer]
2. [Sample answer]

### True/False
1. ❌ False - [Brief explanation]
2. ✅ True - [Brief explanation]
[...]
```

## Quality Checks

- [ ] Balance of question types (2-3 MC, 1-2 SA, 2-3 T/F)
- [ ] All key concepts covered
- [ ] Include application and analysis questions
- [ ] Use Socratic questions to provoke thinking
- [ ] Answers are clear and assessable
- [ ] Difficulty matches KP difficulty

## Completion Report

```
Quiz generated: quizzes/[kp-id]-quiz.md

Statistics:
- Multiple choice: N questions
- Short answer: N questions
- True/False: N questions
- Estimated time: M minutes

Next Steps:
1. Use quiz to assess student understanding
2. Decide on review based on results
3. Generate quiz for next KP
```

## Context

$ARGUMENTS