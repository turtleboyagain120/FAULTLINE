# Contributing to FAULTLINE

Thank you for your interest in contributing to FAULTLINE! This document explains how to contribute code, report bugs, suggest features, and improve the project.

---

## Table of Contents

1. [Code of Conduct](#code-of-conduct)
2. [Getting Started](#getting-started)
3. [Types of Contributions](#types-of-contributions)
4. [Reporting Bugs](#reporting-bugs)
5. [Suggesting Features](#suggesting-features)
6. [Submitting Code](#submitting-code)
7. [Development Setup](#development-setup)
8. [Coding Standards](#coding-standards)
9. [Pull Request Process](#pull-request-process)
10. [Community](#community)

---

## Code of Conduct

### Our Pledge

We are committed to providing a welcoming and inclusive environment for all contributors. We expect everyone to:

- **Be respectful** — Treat others with courtesy and respect
- **Be inclusive** — Welcome people of all backgrounds and skill levels
- **Be collaborative** — Work together toward shared goals
- **Be professional** — Keep discussions constructive and focused

### Unacceptable Behavior

The following will not be tolerated:
- Harassment, discrimination, or hate speech
- Offensive comments or personal attacks
- Trolling or deliberately disruptive behavior
- Sexual harassment or inappropriate content
- Threats or intimidation
- Spam or self-promotion

### Reporting Issues

If you witness or experience misconduct:
1. Report privately to the maintainer
2. Include specific details and context
3. Do not publicly shame or attack individuals
4. Allow for investigation and resolution

---

## Getting Started

### Prerequisites

**Required:**
- Git (download from [git-scm.com](https://git-scm.com/))
- A text editor or IDE (VS Code, Sublime, etc.)
- Modern web browser (Chrome, Firefox, Safari, Edge)
- Basic JavaScript knowledge (for code contributions)

**Optional:**
- GitHub account for collaboration
- Node.js (for development tools)
- Python 3.9+ (for local testing)

### Your First Contribution

**New to open source?** Start here:

1. **Read the README** — Understand the project
2. **Review existing issues** — See what needs work
3. **Look for "good first issue" tag** — Tasks perfect for beginners
4. **Fork the repository** — Create your own copy
5. **Clone locally** — Download to your computer
6. **Make a small change** — Start with something simple
7. **Submit a pull request** — Share your improvement

---

## Types of Contributions

### 1. Bug Reports
Help us find and fix problems:
- Game crashes or freezes
- Controls not responding
- Visual glitches or rendering issues
- Performance problems
- Browser compatibility issues

### 2. Feature Requests
Suggest improvements and new content:
- New gameplay mechanics
- Additional levels or difficulty modes
- UI/UX improvements
- New weapons or abilities
- Customization options

### 3. Code Contributions
Improve the codebase:
- Bug fixes (with tests)
- Performance optimizations
- Code refactoring
- Accessibility improvements
- Browser compatibility fixes

### 4. Documentation
Improve guides and references:
- Typo fixes
- Clarification of unclear sections
- Tutorial improvements
- API documentation
- Example code

### 5. Art & Assets
Enhance visuals and audio:
- Sprite improvements
- New level themes
- Sound effects or music
- UI graphics
- Animation tweaks

### 6. Testing
Improve quality assurance:
- Test cases and edge cases
- Cross-browser testing
- Performance testing
- Accessibility testing
- Device compatibility testing

### 7. Modding & Customization
Create and share mods:
- Level packs
- Custom game modes
- Asset mods
- Balance tweaks
- Quality-of-life improvements

---

## Reporting Bugs

### Before You Report

1. **Check existing issues** — Your bug may already be reported
2. **Try troubleshooting** — See [FAULTLINE Wiki - Troubleshooting](./FAULTLINE_Wiki.md#troubleshooting)
3. **Test on multiple browsers** — Confirm it's not browser-specific
4. **Verify your setup** — Ensure you followed installation correctly

### Creating a Bug Report

Use the GitHub Issues tab and include:

**Title** (clear and specific)
```
[Bug] Gamepad input stops responding after 5 minutes
```

**Description** (provide context)
```
The gamepad input becomes completely unresponsive after approximately 5 minutes of gameplay.
```

**Steps to Reproduce** (exactly how to trigger the bug)
```
1. Connect Xbox controller to computer
2. Open FAULTLINE in Chrome
3. Start a level
4. Play for 5+ minutes, using jump and dash actions
5. Attempt to move character → no response
```

**Expected Behavior** (what should happen)
```
Gamepad should remain responsive throughout gameplay.
Input lag should be imperceptible (under 100ms).
```

**Actual Behavior** (what actually happens)
```
Input stops registering entirely.
Must refresh page to regain control.
```

**Environment** (your setup)
```
Browser: Chrome 120.0.6099.129
OS: Windows 11 (Build 23630)
Gamepad: Xbox Series X Controller (wired USB)
Hardware: Ryzen 5 5600X, RTX 3070, 16GB RAM
Connection: Wired Ethernet
```

**Screenshots/Video** (if applicable)
- Attach screenshot showing the issue
- GIF or video demonstrating the problem
- Error messages from console (F12 → Console)

**Additional Context**
```
This happens consistently in both Level 1 and Level 2.
Works fine with keyboard controls.
Other games recognize the gamepad fine.
```

### Bug Report Template

```markdown
**Describe the bug**
A clear description of what's wrong.

**Steps to reproduce**
1. Step one
2. Step two
3. ...

**Expected behavior**
What should happen.

**Actual behavior**
What actually happens.

**Environment**
- Browser: [Chrome/Firefox/Safari/Edge] version
- OS: [Windows/macOS/Linux] version
- Hardware: [CPU/RAM/GPU if relevant]

**Screenshots**
[Attach if visual issue]

**Console errors**
[Paste from F12 → Console if applicable]

**Additional context**
Any other relevant information.
```

### Priority Levels

We use these labels to prioritize:

| Level | Impact | Example |
|---|---|---|
| 🔴 **Critical** | Game unplayable | Crashes on launch, all inputs broken |
| 🟠 **High** | Major feature broken | Gamepad doesn't work, audio missing |
| 🟡 **Medium** | Feature partially broken | One browser affected, one level broken |
| 🟢 **Low** | Minor issue | Typo, visual glitch in rare case |

---

## Suggesting Features

### Before You Suggest

1. **Check existing issues** — Your idea may already be discussed
2. **Read the roadmap** — See what's already planned
3. **Consider scope** — Is it realistic for a browser game?
4. **Think about users** — Does it benefit players?

### Feature Request Template

Use the GitHub Issues tab:

**Title** (clear and compelling)
```
[Feature] Difficulty levels for customizable challenge
```

**Description** (explain your idea)
```
Add Easy/Normal/Hard difficulty modes so players can customize the challenge level. This would improve retention for both casual and hardcore players.
```

**Problem** (why is this needed?)
```
Currently, all players experience the same difficulty. New players find it hard, while experienced players find it too easy. This limits the appeal.
```

**Solution** (how should it work?)
```
Easy Mode:
- Enemies have 50% health
- Player has 50% more health
- Slower enemy projectiles
- Longer invulnerability after hit

Normal Mode:
- Current game as-is

Hard Mode:
- Enemies have 2x health
- Player has 50% less health
- Faster enemy fire rate
- Shorter invulnerability
```

**Alternative Solutions** (other approaches)
```
- Sliders for individual difficulty parameters
- Custom difficulty editor
- Leaderboards with difficulty multipliers
```

**Additional Context**
```
Similar to: Mirror's Edge difficulty levels
Community interest: High (mentioned in 3 issues, multiple Discord posts)
Estimated effort: Medium
Priority: Nice-to-have
```

### Feature Request Template

```markdown
**Is your feature request related to a problem?**
Describe the problem. E.g., "I'm frustrated when..."

**Describe the solution you'd like**
Clear description of what you want.

**Describe alternatives you've considered**
Other approaches or solutions.

**Additional context**
Examples from other games, mockups, etc.
```

---

## Submitting Code

### Before You Code

1. **Check the roadmap** — Avoid conflicting work
2. **Discuss major changes** — Open an issue first
3. **Read coding standards** — Below in this document
4. **Review existing code** — Understand the style
5. **Test locally first** — Ensure it works

### Development Workflow

#### Step 1: Fork the Repository
```bash
# Click "Fork" on GitHub
# Creates your personal copy
```

#### Step 2: Clone Your Fork
```bash
git clone https://github.com/YOUR-USERNAME/FAULTLINE.git
cd FAULTLINE
```

#### Step 3: Create a Feature Branch
```bash
# Always create a new branch for each feature/fix
git checkout -b feature/add-difficulty-levels
# or
git checkout -b fix/gamepad-input-lag
```

**Branch naming convention:**
- `feature/description` — New features
- `fix/description` — Bug fixes
- `docs/description` — Documentation
- `refactor/description` — Code refactoring
- `test/description` — Tests or test improvements

#### Step 4: Make Your Changes
```bash
# Edit files
# Test frequently (F5 in browser)
# Commit regularly with clear messages
git add .
git commit -m "Fix: Gamepad input handling delay"
```

**Commit message guidelines:**
- Start with type: `Fix:`, `Feature:`, `Docs:`, `Refactor:`
- Keep it under 50 characters
- Use imperative mood ("Fix" not "Fixed" or "Fixes")
- Reference issues: `Fix: Input lag (fixes #123)`

#### Step 5: Keep Your Branch Updated
```bash
# Before submitting, sync with main
git fetch upstream
git rebase upstream/main
```

#### Step 6: Push to Your Fork
```bash
git push origin feature/add-difficulty-levels
```

#### Step 7: Submit a Pull Request
- Go to [FAULTLINE repository](https://github.com/turtleboyagain120/FAULTLINE)
- Click "New Pull Request"
- Select your branch
- Fill in the PR template (below)
- Click "Create Pull Request"

---

## Development Setup

### Local Setup

#### 1. Install Prerequisites
```bash
# Install Git from https://git-scm.com/
git --version

# Install Node.js (optional, for tools)
node --version
npm --version
```

#### 2. Clone Repository
```bash
git clone https://github.com/turtleboyagain120/FAULTLINE.git
cd FAULTLINE
```

#### 3. Start Development
```bash
# No build step required!
# Just open index.html in your browser

# Windows:
start index.html

# macOS:
open index.html

# Linux:
firefox index.html
```

#### 4. Test Your Changes
```bash
# Open browser developer tools (F12)
# Check Console tab for errors
# Test on multiple browsers
# Test on multiple screen sizes
```

### Project Structure

```
FAULTLINE/
├── index.html              # Game entry point
├── styles/
│   └── main.css           # Styling
├── scripts/
│   ├── game.js            # Main game loop
│   ├── player.js          # Player mechanics
│   ├── enemy.js           # Enemy AI
│   ├── physics.js         # Collision/movement
│   ├── render.js          # Canvas rendering
│   └── input.js           # Gamepad/keyboard
├── assets/
│   ├── sprites/           # Character graphics
│   ├── environments/      # Level graphics
│   └── audio/            # Sound effects
├── levels/                # Level definitions
├── tests/                 # Test files (if any)
└── docs/                  # Documentation
```

### Debugging Tips

**Browser Console (F12)**
- Check for errors (red messages)
- Use `console.log()` to debug
- Monitor performance (Ctrl+Shift+P → "Show Performance")

**Chrome DevTools**
- Sources tab: Set breakpoints and step through code
- Elements tab: Inspect HTML/CSS
- Network tab: Monitor asset loading
- Performance tab: Profile frame rate

**Firefox Developer Tools**
- Inspector: HTML/CSS inspection
- Debugger: JavaScript debugging
- Console: Error messages and logging
- Network: Asset loading

---

## Coding Standards

### JavaScript Standards

**Use strict mode**
```javascript
"use strict";
// Code here...
```

**Variable naming**
```javascript
// Use camelCase for variables and functions
const playerHealth = 100;
const movePlayer = (x, y) => { };

// Use PascalCase for classes/constructors
class GameEngine { }
class Enemy { }

// Use UPPER_SNAKE_CASE for constants
const MAX_HEALTH = 100;
const GRAVITY = 9.8;
```

**Comments**
```javascript
// Use single-line comments for brief explanations
const speed = 5; // pixels per frame

// Use multi-line comments for complex logic
/*
 * Calculate if player collides with enemy.
 * Check both hitboxes and return true if overlapping.
 * Must account for both moving and stationary enemies.
 */
```

**Function style**
```javascript
// Prefer arrow functions
const calculateDamage = (attack, defense) => {
  return Math.max(1, attack - defense);
};

// Or function declarations for complex logic
function updatePlayerPosition(deltaTime) {
  // Complex logic here
}
```

**Avoid anti-patterns**
```javascript
// ❌ DON'T use eval()
eval("code here"); // NEVER

// ❌ DON'T use var
var x = 5; // Use const or let instead

// ❌ DON'T use == (loose comparison)
if (x == 5) { } // Use === instead

// ❌ DON'T modify global scope
window.myVariable = 5; // Avoid this

// ✅ DO use const by default
const x = 5;

// ✅ DO use let when you need to reassign
let score = 0;
score += 10;

// ✅ DO use strict comparison
if (x === 5) { }

// ✅ DO use local variables
const myVariable = 5;
```

### CSS Standards

**Use semantic selectors**
```css
/* ✅ DO: Specific, semantic selectors */
.game-canvas { }
.player-health-bar { }
.enemy-sprite { }

/* ❌ DON'T: Generic or overly broad selectors */
.container { }
div { }
* { }
```

**Naming convention**
```css
/* Use kebab-case for CSS classes */
.player-sprite { }
.enemy-health-bar { }
.level-background { }
```

**Organization**
```css
/* Group related styles */
/* Layout */
.game-container {
  display: flex;
  width: 100%;
}

/* Colors */
.player-sprite {
  background-color: #ff0000;
}

/* Animation */
@keyframes move {
  from { transform: translateX(0); }
  to { transform: translateX(100px); }
}
```

### HTML Standards

**Use semantic HTML**
```html
<!-- ✅ DO: Semantic HTML -->
<header>
  <nav>Menu</nav>
</header>
<main>
  <canvas id="gameCanvas"></canvas>
</main>
<footer>
  <p>Credits</p>
</footer>

<!-- ❌ DON'T: Generic divs -->
<div>
  <div>Menu</div>
  <div>Canvas</div>
  <div>Credits</div>
</div>
```

**Use meaningful IDs and classes**
```html
<!-- ✅ DO: Descriptive names -->
<canvas id="gameCanvas"></canvas>
<div class="hud-score"></div>
<button class="start-button"></button>

<!-- ❌ DON'T: Generic names -->
<canvas id="canvas1"></canvas>
<div class="container"></div>
<button class="btn"></button>
```

---

## Pull Request Process

### Creating a Pull Request

**Title** (clear and specific)
```
Add difficulty levels for customizable challenge
```

**Description** (explain your changes)
```
## Changes
- Added Easy/Normal/Hard difficulty modes
- Updated enemy health scaling
- Added difficulty selector to main menu

## Why?
Players requested ability to adjust difficulty. New players find the game too hard, experienced players find it too easy.

## Testing
- Tested all 3 difficulty levels on Chrome and Firefox
- Verified enemies scale correctly
- Checked save/load of difficulty preference
- Performance impact: <1% increase

## Screenshots
[Include screenshots of new UI/features]
```

**Checklist** (before submitting)
```markdown
- [ ] Code follows style guidelines
- [ ] New code includes comments explaining complex logic
- [ ] No console errors or warnings
- [ ] Tested on Chrome, Firefox, and Safari
- [ ] Game performance not degraded
- [ ] Commit messages are clear
- [ ] No unrelated changes included
- [ ] Updated documentation if needed
```

### Pull Request Template

```markdown
## Description
Brief explanation of what this PR does.

## Type of Change
- [ ] Bug fix (fixes an issue without breaking changes)
- [ ] New feature (adds functionality without breaking changes)
- [ ] Breaking change (fix or feature that causes existing functionality to change)
- [ ] Documentation update

## Changes
- Change 1
- Change 2
- Change 3

## Testing
How you tested this change:
- [ ] Tested on Chrome
- [ ] Tested on Firefox
- [ ] Tested on Safari
- [ ] Tested on mobile browser
- [ ] Performance impact: Minimal / None / [explain]

## Screenshots (if applicable)
[Attach images/GIFs]

## Related Issues
Fixes #[issue number]
Related to #[issue number]

## Checklist
- [ ] Code follows style guidelines
- [ ] No new warnings in console
- [ ] Added comments for complex logic
- [ ] Updated relevant documentation
- [ ] No unrelated changes included
```

### Review Process

**What happens after you submit:**

1. **Automated checks** (5-10 minutes)
   - Verify no breaking errors
   - Check code doesn't have obvious issues
   - Test builds successfully

2. **Maintainer review** (1-7 days)
   - Read code and understand changes
   - Test locally
   - Check for bugs or improvements
   - Provide feedback

3. **Feedback & revision** (as needed)
   - You may need to make changes
   - Push updates to same branch
   - PR automatically updates
   - Process repeats if needed

4. **Approval & merge** (when ready)
   - Maintainer approves changes
   - PR is merged to main branch
   - Your code is now part of FAULTLINE!

**During review, be open to:**
- Questions about your approach
- Suggestions for improvement
- Requests for additional tests
- Requests for documentation
- Style or refactoring feedback

---

## Community

### Discussion Forums

- **GitHub Issues** — Bug reports and features
- **GitHub Discussions** — General questions and ideas
- **Discord** (if available) — Real-time chat
- **Reddit** — r/gamedev community

### Getting Help

**Stuck on something?**
1. Check the [FAULTLINE Wiki](./FAULTLINE_Wiki.md)
2. Search existing GitHub Issues
3. Ask on GitHub Discussions
4. Email the maintainer if urgent

### Crediting Contributors

All contributors will be credited:
- In the game credits (if applicable)
- In the GitHub contributor list
- In release notes for major contributions
- On the project website

### Recognition Levels

| Contribution | Recognition |
|---|---|
| Small fixes/typos | GitHub contributor list |
| Bug fixes | Release notes + credits |
| Features | Release notes + credits + special mention |
| Major work | Listed as maintainer/lead |

---

## FAQ

### Q: I found a bug, but I'm not sure how to fix it. Can I still contribute?

**A:** Yes! Report it using the bug report template. Others can help fix it, or it alerts the maintainer.

### Q: Can I work on a feature before opening an issue?

**A:** It's better to open an issue first. Major features might already be planned, and you could be duplicating work. Quick discussion saves time.

### Q: What if my pull request gets rejected?

**A:** That's okay! Rejection usually means:
- The timing isn't right
- The approach needs adjustment
- The scope is too large
- There's a conflict with other work

Ask for feedback and learn. You can revise and resubmit.

### Q: How long does review take?

**A:** Usually 1-7 days depending on:
- Complexity of changes
- Maintainer availability
- Whether you need revision

### Q: Can I make changes after submitting a PR?

**A:** Yes! Push to your branch and the PR updates automatically. You don't need to create a new PR.

### Q: Do I get paid for contributions?

**A:** FAULTLINE is a volunteer project. Contributors do it for portfolio building, learning, and community. Recognition is provided but there's no payment.

### Q: What if I disagree with feedback?

**A:** Open a discussion! Explain your reasoning. Maintainers will listen and collaborate. If you still disagree, it's okay — there's no obligation to proceed.

---

## Contact

**Maintainer:** turtleboyagain120  
**GitHub:** [@turtleboyagain120](https://github.com/turtleboyagain120)  
**Repository:** [FAULTLINE](https://github.com/turtleboyagain120/FAULTLINE)

---

## License

By contributing to FAULTLINE, you agree that your contributions will be licensed under the same Apache 2.0 license.

---

**Thank you for contributing to FAULTLINE! 🎮**

Whether it's code, art, bug reports, or ideas — your involvement makes this project better.

Happy contributing! 🚀
