# 🤝 Contributing to Afrowave Learning

Thank you for your interest in making education more accessible! This guide will help you contribute lessons, translations, projects, and improvements.

---

## 🎯 Ways to Contribute

### 1️⃣ Add New Lessons
Share your programming knowledge with students worldwide!

### 2️⃣ Translate Content
Help make lessons available in your language.

### 3️⃣ Create Projects
Design hands-on coding challenges for learners.

### 4️⃣ Improve Documentation
Fix typos, clarify explanations, add examples.

### 5️⃣ Share Mobile Tools
Know a great mobile coding tool? Share it!

---

## 📝 Adding New Lessons

### Structure Your Lesson

Every lesson should follow this template:

```markdown
# Lesson Title

**Difficulty:** Beginner / Intermediate / Advanced  
**Estimated Time:** X minutes  
**Prerequisites:** List what students should know first

## 🎯 What You'll Learn
- Learning objective 1
- Learning objective 2
- Learning objective 3

## 📖 Introduction
Brief overview of the topic and why it matters.

## 🔧 Main Content
Step-by-step explanation with:
- Clear headings
- Code examples
- Diagrams (if helpful)
- Real-world analogies

## 💻 Code Examples
```language
// Well-commented code examples
// that work on mobile devices too
```

## ✅ Practice Exercises
1. Exercise 1
2. Exercise 2
3. Exercise 3

## 🎯 Mini Project
A small project to apply what was learned.

## 📚 Next Steps
- Link to next lesson
- Additional resources
- Related topics

## ❓ Common Questions
Address frequent student questions.
```

### File Naming Convention
- Use lowercase with hyphens: `introduction-to-variables.md`
- Number lessons sequentially: `01-introduction.md`, `02-variables.md`

### Where to Put Your Lesson

```
lessons/
├── assembler/
├── c-programming/
├── csharp-dotnet/
├── javascript/
├── web-development/
│   ├── html-css/
│   ├── javascript-web/
│   └── projects/
└── theory/
    ├── binary-hexadecimal/
    ├── computer-architecture/
    └── algorithms/
```

---

## 🌍 Translation Guidelines

### Starting a Translation

1. Create a language folder: `lessons/[topic]/[language-code]/`
   - Examples: `lessons/c-programming/fr/`, `lessons/javascript/sw/`

2. Use ISO 639-1 language codes:
   - `en` - English
   - `fr` - French (Français)
   - `sw` - Swahili (Kiswahili)
   - `ar` - Arabic (العربية)
   - `pt` - Portuguese (Português)
   - `es` - Spanish (Español)

3. Keep the same filename as the English version

4. Add a header noting the translation:
```markdown
# [Lesson Title in Your Language]

**Language:** [Your Language] ([Native Name])  
**Translator:** [@your-github-username](https://github.com/your-username)  
**Last Updated:** YYYY-MM-DD

> 📖 Original English version: [Link to English lesson]

---

[Your translated content]
```

### Translation Best Practices
- ✅ Translate explanations and comments
- ✅ Keep code examples in English (with translated comments)
- ✅ Adapt examples to local context when helpful
- ✅ Use simple, clear language
- ⚠️ Technical terms: Keep in English with native explanation in parentheses

---

## 🎯 Creating Projects

### Project Structure

```markdown
# Project Name

**Difficulty:** Beginner / Intermediate / Advanced  
**Topics:** List relevant topics  
**Estimated Time:** X hours

## 🎯 Objective
What the student will build and learn.

## 📋 Requirements
What knowledge/tools are needed.

## 🚀 Getting Started
Step-by-step setup instructions.

## ✅ Tasks
Break the project into clear steps:
1. Task 1 with hints
2. Task 2 with hints
3. Task 3 with hints

## 💡 Hints & Tips
Guidance without giving away solutions.

## 🎉 Solution
Complete working solution (in a separate file or collapsed section).

## 🚀 Extensions
Ideas to expand the project further.
```

### Project Categories
- **Beginner:** Simple programs using one concept
- **Intermediate:** Combine multiple concepts
- **Advanced:** Real-world applications

---

## 📱 Mobile-Friendly Guidelines

**All content MUST be mobile-friendly!**

### ✅ Do:
- Use short code lines (max 60 characters)
- Break long explanations into bullet points
- Use clear section headings
- Test on mobile GitHub app
- Include copy-paste friendly code
- Use emojis for visual navigation

### ❌ Don't:
- Use wide tables (they break on mobile)
- Embed videos (use links instead)
- Use tiny font sizes
- Create horizontal scrolling
- Require desktop-only tools

---

## 🔧 Technical Requirements

### Code Examples
- Must run on minimal hardware
- Should work in mobile environments when possible
- Include clear comments
- Show expected output

### Testing Your Contribution
Before submitting:
1. ✅ Read on GitHub mobile app
2. ✅ Check all links work
3. ✅ Verify code examples are correct
4. ✅ Ensure proper formatting

---

## 📤 Submitting Your Contribution

### Step 1: Fork the Repository
Click "Fork" at the top of this repository.

### Step 2: Create a Branch
```bash
git checkout -b add-lesson-[topic-name]
```
or
```bash
git checkout -b translate-[language]-[topic]
```

### Step 3: Add Your Content
Place files in the appropriate folders.

### Step 4: Commit Your Changes
```bash
git add .
git commit -m "Add [description of contribution]"
```

Examples:
- "Add C programming lesson on pointers"
- "Translate JavaScript intro to Swahili"
- "Add beginner project: calculator"

### Step 5: Push and Create Pull Request
```bash
git push origin your-branch-name
```

Then open a Pull Request on GitHub with:
- Clear title
- Description of what you added
- Why it's valuable for learners

---

## 👥 Becoming a Regular Contributor

Active contributors can:
- Get write access to the repository
- Help review other contributions
- Guide the project direction
- Mentor new contributors

Interested? Open an issue expressing your interest!

---

## 📜 Code of Conduct

### Our Pledge
We are committed to providing a welcoming, inclusive environment for everyone.

### Expected Behavior
- ✅ Be respectful and constructive
- ✅ Welcome newcomers
- ✅ Focus on education and accessibility
- ✅ Give credit where due

### Unacceptable Behavior
- ❌ Harassment or discrimination
- ❌ Trolling or insulting comments
- ❌ Political or divisive content
- ❌ Plagiarism or uncredited work

---

## ❓ Questions?

- **General questions:** [Open a discussion](https://github.com/afrowaveltd/afrowave-learning/discussions)
- **Bug reports:** [Open an issue](https://github.com/afrowaveltd/afrowave-learning/issues)
- **Translation coordination:** Check existing translation issues

---

## 🙏 Thank You!

Every contribution, no matter how small, helps make quality education accessible to someone who needs it.

**You're making a difference!** 💙

---

**Made with 💙 by the Afrowave Community