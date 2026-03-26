# Codebase-to-Course Skill

English | [中文](./README_zh.md) | [📺 Interactive Demo](./demo.html)

## Overview

The **codebase-to-course** skill transforms any codebase into a beautiful, interactive single-page HTML course that teaches how the code works to non-technical people (especially "vibe coders" who build with AI).

**[🎮 Try the Interactive Demo](./demo.html)** to see examples of code translations, quizzes, and interactive elements in action!

## What It Does

Converts a repository into a self-contained HTML file featuring:
- 📚 **Scroll-based modules** with smooth navigation
- 🎨 **Animated visualizations** showing data flow and architecture
- ✅ **Interactive quizzes** testing practical application
- 📝 **Code↔English translations** - side-by-side plain language explanations
- 💡 **Glossary tooltips** for every technical term
- 🎯 **Group chat animations** showing component interactions
- 📊 **Flow diagrams** illustrating system architecture

## How to Use

When interacting with DeerFlow, you can trigger this skill by saying:

- "Turn this into a course"
- "Make a course from this project"
- "Create an interactive tutorial from this codebase"
- "Explain this codebase interactively"
- "Turn [GitHub URL] into a course"
- "Make a course from ./my-project"

## Examples

### Convert the current repository:
```
Turn the DeerFlow repository into an interactive course
```

### Convert a GitHub repository:
```
Make a course from https://github.com/bytedance/deer-flow
```

### Convert a local project:
```
Turn ./my-app into a course
```

## What Gets Generated

The skill creates a single `course.html` file with:

1. **5-8 modules** structured as a learning journey
2. **Module 1**: What the app does and how it works
3. **Modules 2-6**: Components, data flows, APIs, patterns, debugging
4. **Final module**: Big picture architecture

Each module includes:
- 3-6 screens (sub-sections)
- Code with English translations
- Interactive elements (quizzes, animations)
- "Aha!" callout boxes
- Practical metaphors

## Design Philosophy

The course is designed for **"vibe coders"** - people who:
- Build software using AI coding tools
- Need to understand code without writing from scratch
- Want to steer AI better, debug faster, and make smarter decisions
- May lack traditional CS education

Every concept is explained in plain language, assuming zero technical background.

## File Structure

```
skills/public/codebase-to-course/
├── SKILL.md                           # Main skill implementation guide
├── README.md                          # This file
└── references/
    ├── design-system.md              # CSS tokens, colors, typography
    └── interactive-elements.md       # Interactive element patterns
```

## Technical Details

- **Output**: Single self-contained HTML file
- **Dependencies**: Only Google Fonts CDN
- **Size**: Typically 200-500KB
- **Works offline**: Yes (after initial font load)
- **Mobile friendly**: Fully responsive
- **Browser support**: Modern browsers (Chrome, Firefox, Safari, Edge)

## Implementation

The skill follows a 4-phase process:

1. **Codebase Analysis** - Deep dive into repository structure
2. **Curriculum Design** - Plan 5-8 module learning arc
3. **Build the Course** - Generate HTML with all interactive elements
4. **Review and Open** - Present to user for feedback

## Credit

This skill was created by [zarazhangrui](https://github.com/zarazhangrui) and is now integrated into DeerFlow.

Original repository: https://github.com/zarazhangrui/codebase-to-course

## License

Follows the same license as the DeerFlow project (MIT).
