# Refactoring a Python Graphics Project into a Mobile App

A classroom-ready computer science lesson where students refactor a CMU Graphics Python project into a mobile app using CodeHS React Native. The activity helps students explore how the same programming concepts translate across languages and platforms while developing problem-solving, debugging, and creative design skills.

**Teacher-facing lesson site:** [markalanjohnston.github.io/cmu-graphics-to-mobile-app](https://markalanjohnston.github.io/cmu-graphics-to-mobile-app)

**Live app demo:** [codehs.com/sandbox/id/mickeyscreen-AtogQW](https://codehs.com/sandbox/id/mickeyscreen-AtogQW)

---

## Project Overview

Students take an existing interactive program built in Python using the [CMU CS Academy](https://academy.cs.cmu.edu/) graphics library and refactor it into a mobile application using [CodeHS React Native](https://codehs.com/).

The goal is not simply to recreate the project in a new language — it is to help students understand how programming concepts transfer between environments. Students write their original CMU Graphics project in the [CMU CS Academy IDE](https://academy.cs.cmu.edu/ide), then use [Claude.ai](https://claude.ai/) to help refactor the code into React Native. The result is tested and run in the [CodeHS Sandbox](https://codehs.com/sandbox).

> This activity was created as part of the **Computing Skills for Today's Middle School and High School Classrooms Workshop**, which encouraged teachers to design classroom activities using tools introduced during the training.

**The project emphasizes concept transfer, not syntax memorization.** Students learn that programming ideas — events, variables, state changes, conditionals — exist across many languages and frameworks.

---

## The Tool Chain

```
CMU CS Academy  →  Claude.ai  →  CodeHS Sandbox
 (write Python)    (refactor)    (run on device)
```

Students write their original project in CMU CS Academy, paste it into Claude.ai to refactor into React Native, then paste the result into the CodeHS sandbox and debug until it runs. The finished app can be opened on a tablet or phone via the Expo Go app using the CodeHS shareable link.

---

## Why This Activity Works

Many introductory programming courses rely on graphics libraries (such as CMU Graphics) to teach interactive programming concepts. Mobile applications rely on the same underlying ideas:

| CMU Graphics Concept | Mobile App Equivalent |
|---|---|
| `onMousePress` | Touch event (`onPress`) |
| Shape position | Component position |
| State variables | React `this.state` |
| `shape.clear()` | `this.setState({ part: false })` |
| Drawing order | Component render order |

By refactoring an existing project, students can focus on understanding the logic rather than inventing an idea from scratch.

---

## Learning Objectives

Students will:

- Recognize how programming concepts translate across languages and platforms
- Practice debugging and iterative development
- Build a basic mobile application interface
- Collaborate effectively with an AI coding assistant
- Communicate technical problems clearly and precisely
- Reflect on how design decisions change across platforms

---

## Classroom Implementation

**Course:** Fundamentals of Computer Science
**Grade Level:** High School (9–10)

Students complete the activity in four phases.

### Phase 1 — Explore the Original Program

Students run and analyze the CMU Graphics project using the starter file (solution redacted). They identify variables, events, state changes, and drawing logic.

### Phase 2 — Plan the Mobile Version

Students sketch how the program should behave as a mobile app: what UI components are needed, what replaces `onMousePress` on a touchscreen, and how layout changes from a square canvas to a phone screen.

### Phase 3 — Refactor with AI

Students paste their Python code into Claude.ai and prompt it to refactor for CodeHS React Native. They paste the output into the CodeHS sandbox, run it, copy each error message back to Claude, and iterate until the app works.

### Phase 4 — Reflect

Students discuss or write about which concepts transferred directly, what the AI got right and wrong, and what decisions required human judgment.

---

## Repository Structure

```
/docs
    index.html                    ← GitHub Pages teacher lesson site
    /assets                       ← Screenshots used by the site

/examples
    cmu-starter.py                ← CMU Graphics starter code (solution redacted)
    react-native-example.jsx      ← Finished React Native app (fully commented)

/lesson
    ai-refactoring-process.md     ← Full AI collaboration log with error walkthrough
```

---

## For Teachers

The [GitHub Pages site](https://markalanjohnston.github.io/cmu-graphics-to-mobile-app) is the primary teacher-facing resource. It includes the concept mapping table, the full AI debugging log, classroom implementation guide, and links to all files — no GitHub experience required to navigate it.

**About the Python starter file:** `examples/cmu-starter.py` contains the full drawing setup but has the `onMousePress` solution replaced with `### Solution code redacted — fill in your logic here ###`. This lets teachers work through the solution before sharing the file with students. The React Native file is complete and unredacted.

**About the AI collaboration log:** `lesson/ai-refactoring-process.md` documents all six rounds of errors encountered during the refactoring, what caused each one, how it was fixed, and what lesson it teaches. It is designed to be shared with students before they start their own refactoring to set realistic expectations.

---

## Technology Used

- [CMU CS Academy](https://academy.cs.cmu.edu/) — original Python project environment
- [Claude.ai](https://claude.ai/) — AI-assisted code refactoring
- [CodeHS](https://codehs.com/) — React Native sandbox for mobile development
- [Expo Go](https://expo.dev/go) — mobile app for running the finished project on a device
- JavaScript / React Native
- GitHub / GitHub Pages — lesson distribution and public documentation

---

## License

This lesson may be reused or modified for educational purposes.
