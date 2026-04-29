# Teacher Guide: HTML/CSS Learning Environment with AI Tutor

## Overview

This workspace transforms GitHub Copilot in VS Code into an educational tutor for teaching HTML and CSS fundamentals to grade 9 students while also teaching AI literacy skills.

## How It Works

### The AI Tutor System

The system uses VS Code's agent customization features to create context-aware tutoring:

1. **Core Behavior** (`.github/copilot-instructions.md`)
   - Defines Copilot's teaching philosophy and personality
   - Implements guardrails against providing complete solutions
   - Teaches both HTML/CSS AND how to work with AI

2. **Lesson-Specific Guidance** (`.github/instructions/lesson-*.instructions.md`)
   - Automatically activates when students work on specific lessons
   - Provides lesson-appropriate teaching strategies
   - Adapts difficulty and scaffolding by lesson number

3. **Validation System** (`.github/instructions/validation.instructions.md`)
   - Activates when students ask to "check my work"
   - Requires students to explain their code
   - Provides feedback on understanding, not just correctness

4. **Challenge System** (`.github/instructions/advanced-challenges.instructions.md`)
   - Activates when students request challenges
   - Provides extension activities appropriate to their level

### Progressive Learning Structure

**Lessons 1-3 (Scaffolded):**
- Partial code with blanks to fill in
- More explicit guidance from Copilot
- Frequent encouragement and smaller steps

**Lessons 4-8 (Independent):**
- TODO comments but less starter code
- Copilot pushes for independent problem-solving
- More "what do you think?" questions

**Projects (Open):**
- Templates to start from, but student-driven
- Copilot guides planning and problem-solving
- Focus on creativity and applying all skills

## Distribution Methods

### Option A: Git Clone (Recommended)

**Setup:**
1. Create a GitHub repository from this workspace
2. Students clone: `git clone [your-repo-url]`
3. Open in VS Code

**Benefits:**
- Teaches industry practice (git workflow)
- You can review commit history to see progression
- Students can push updates and you can pull to review
- Built-in backup of student work

**Student Git Workflow:**
```bash
# After completing a section:
git add .
git commit -m "Complete Lesson 1"
git push

# Teacher can pull to review progress
```

### Option B: Shared Drive Copy

**Setup:**
1. Copy workspace folder to shared drive
2. Students copy to their computers
3. Open in VS Code

**Benefits:**
- Simpler for students unfamiliar with git
- No account setup needed
- Works offline

## Required Setup for Students

### Essential Extensions

1. **GitHub Copilot** - The AI tutor
   - Requires GitHub account with education access
   - Free for students via GitHub Education
   
2. **Live Server** - Instant preview
   - Install from VS Code extensions marketplace
   - Right-click HTML file → "Open with Live Server"

### VS Code Settings

No special settings required! The `.github/copilot-instructions.md` file automatically configures Copilot's behavior.

## Monitoring Student Progress

### Git Commits (if using git)

Review commit history to see:
- How frequently they commit (should be after each section)
- Commit messages (descriptive or vague?)
- Code changes over time
- Whether work appears suddenly (red flag for copying)

```bash
# View student commit history
git log --oneline
git log --all --graph

# See specific changes
git diff [commit1] [commit2]
```

### Code Reviews

Look for:
- **Understanding vs copying:** Can they explain their code?
- **Progression:** Does code quality improve over lessons?
- **Independence:** Do later lessons show more independent work?
- **Experimentation:** Evidence of trying different approaches?

### In-Class Observation

- Ask students to explain their code verbally
- Watch how they interact with Copilot (asking good questions?)
- Observe debugging process (systematic or random?)
- Check if they test their code as they build

## Guardrails & Academic Integrity

### What the Guardrails Do

The system is designed to prevent shortcuts:

1. **Never provides complete solutions**
   - Detects phrases like "do it for me", "complete this"
   - Responds with questions instead of answers
   - Requires attempt before providing help

2. **Explanation-based validation**
   - "Check my work" asks students to explain code first
   - Assesses understanding, not just correctness
   - Makes copying less effective (you can't explain code you don't understand)

3. **Graduated hints**
   - Level 1: Conceptual (general principle)
   - Level 2: Directional (where to look)
   - Level 3: Specific (what's wrong)
   - Level 4: Example in different context
   - Only reaches level 4 after genuine attempts

### What the Guardrails DON'T Do

**Cannot reliably detect:**
- Code copied from external sources
- Work done by someone else
- Solutions shared between students

**Why explanation-based validation helps:**
- Students who copy can't explain the code
- Becomes obvious in verbal discussions
- Focuses learning on understanding, not completion

### Red Flags to Watch For

- Student can't explain their code when asked
- Code style dramatically changes between lessons
- Advanced techniques not yet covered
- Sudden completion after struggling
- Defensive when asked to explain

### If You Suspect Copying

1. **Don't accuse** - Maintain supportive environment
2. **Ask to explain** - Walk through code together
3. **Ask "what if" questions** - Test understanding
4. **Rebuild together** - Guide them to build understanding
5. **Frame positively** - "Let's make sure you understand this so you can use it later"

## Classroom Facilitation Tips

### Getting Started (First Class)

1. **Setup Day:**
   - Install VS Code and extensions
   - Clone/copy workspace
   - Walk through STUDENT_GUIDE.md together
   - Demo asking Copilot for help
   - Show Live Server

2. **First Lesson Together:**
   - Do Lesson 1 as a class
   - Show how to ask Copilot questions
   - Demonstrate the difference between good and vague questions
   - Model the "try, then ask" approach

### Pacing

**Recommended Schedule** (assuming ~3 hours per week):
- Week 1: Lessons 1-2 + Copilot intro
- Week 2: Lessons 3-4
- Week 3: Lessons 5-6
- Week 4: Lessons 7-8
- Week 5+: Projects

**Flexible pacing:**
- Fast learners: Move to projects early, work on challenges
- Students who need more time: Spend extra time on early lessons, it's okay!
- The lessons are foundational—better to understand deeply than rush

### Discussion Prompts

**For AI Literacy:**
- "What did Copilot suggest? Why do you think it suggested that?"
- "Did Copilot's answer work? What did you learn from testing it?"
- "How did you ask the question? Could you ask it differently?"
- "When should you trust AI vs verify yourself?"

**For Web Development:**
- "Why did you choose that tag/property?"
- "What other ways could you solve this problem?"
- "How would you explain this code to someone else?"
- "What surprised you about how this works?"

### Handling Common Issues

**Student says "Copilot won't help me":**
- Check: Are they asking specific questions?
- Check: Are they asking for complete solutions?
- Teach: How to ask better questions

**"My CSS isn't working":**
- Teach debugging: Check link, check syntax, check selectors
- Use DevTools together
- Guide systematic problem-solving

**"I'm stuck and don't know what to do":**
- Break it down: What's one small thing to try?
- Review README: What does it suggest?
- Ask Copilot: But demonstrate good question-asking

**"This is too easy/hard":**
- Too easy: Challenges! Move to projects early
- Too hard: More time on current lesson, pair programming

## Customizing for Your Class

### Adjusting Difficulty

**Make easier:**
- Add more scaffolding to later lessons
- Extend the scaffolded lessons (1-5 instead of 1-3)
- Add more example code in READMEs
- Provide more explicit hints

**Make harder:**
- Reduce scaffolding in early lessons
- Add more complex challenges
- Introduce advanced topics earlier
- Require independent research

### Adding Content

You can add:
- Additional lessons (create new folder + instruction file)
- More project templates
- Code standards guide
- Assessment rubrics

**To add a new lesson:**
1. Create `lessons/09-your-topic/` folder
2. Add README.md, exercise.html, style.css
3. Create `.github/instructions/lesson-09-your-topic.instructions.md`
4. Use `applyTo: "lessons/09-*/**"` to auto-activate

### Modifying Copilot Behavior

Edit `.github/copilot-instructions.md` to adjust:
- Teaching style (more/less direct)
- Encouragement level
- Guardrail strictness
- AI literacy emphasis

## Assessment Strategies

### Formative Assessment (During)

- **Code reviews:** Check commits regularly
- **Check-ins:** Ask students to explain sections
- **Observation:** Watch problem-solving process
- **Self-assessment:** Students explain what they learned

### Summative Assessment (End)

**Option 1: Project-Based**
- Assign final project with rubric
- Assess HTML structure, CSS styling, code quality
- Require explanation/presentation

**Option 2: Portfolio**
- Students select best 3 projects
- Write reflection on learning
- Present to class

**Option 3: Practical Exam**
- Build specific page from requirements
- Time-limited, but Copilot available
- Must explain code choices

### Rubric Considerations

Assess:
- **Code Quality:** Structure, organization, naming
- **Understanding:** Can explain code decisions
- **Functionality:** Does it work as intended?
- **Design:** Visual appeal, usability
- **Best Practices:** Semantic HTML, accessibility
- **Problem-Solving:** Debugging, independence

## Troubleshooting

### Copilot Not Responding Appropriately

- Check: Is `.github/copilot-instructions.md` present?
- Check: Are lesson instruction files in correct location?
- Try: Reloading VS Code window
- Check: Copilot enabled for workspace?

### Students Getting Complete Solutions

- Remind: The goal is learning, not finishing
- Teach: How to ask for hints, not answers
- Adjust: Make questions more specific in copilot-instructions.md
- Consider: More emphasis on explanation-based validation

### Live Server Not Working

- Check: Extension installed?
- Check: HTML file saved?
- Try: Right-click HTML file → "Open with Live Server"
- Alternative: Open HTML file directly in browser (less convenient)

## Resources for Teachers

- [GitHub Education](https://education.github.com/) - Free Copilot for students
- [MDN Web Docs](https://developer.mozilla.org/) - Reference for concepts
- [VS Code Copilot Docs](https://code.visualstudio.com/docs/copilot/overview) - Official documentation

## Support & Feedback

If you modify or improve this system:
- Document what worked/didn't work
- Share adaptations with other teachers
- Contribute improvements back to the repository

## Philosophy

Remember: **The goal is to develop capable, thoughtful developers who understand their code, not to produce perfect exercises quickly.**

This system teaches:
1. HTML & CSS fundamentals
2. How to learn with AI assistance
3. Problem-solving and debugging
4. Professional development practices (git, DevTools)
5. Critical thinking about code

Success is measured by understanding and growth, not perfect code or quick completion.

---

**Questions?** Ask in the repository issues or discussions. Good luck teaching!
