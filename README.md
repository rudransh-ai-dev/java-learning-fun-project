# 🌲 Green Graph (GitHub Contribution Automator)

**Green Graph** is a clever, customizable Node.js script that lets you paint your GitHub contribution graph by automating commits. With this tool, you can make it look like you've been working tirelessly in the past (or the future).

The tool randomly selects dates within a given timeframe (like the entire year of 2025) and creates a series of timestamped backdated commits, completely filling up those green squares on your GitHub profile. 🚀

---

## 🛠️ Built With
- **Node.js** (v20+)
- **simple-git** - For easy execution of asynchronous git commands
- **moment** - To easily handle subtract/add dates from the present
- **random** - To randomly distribute commits across the grid

---

## 🚀 Getting Started

To get your own contribution graph fully populated:

### 1. Prerequisites
Make sure you have [Node.js](https://nodejs.org/) installed on your machine.
Ensure you've cloned this repository into a folder that has a `.git` tracking connection to your GitHub repository.

### 2. Install Dependencies
Install the required npm modules to run the project.
```bash
npm install
```

### 3. Customize Your Script (Optional)
By default, the script generates **300 commits randomly scattered across the year 2025**.

If you wish to change this behavior:
- Open `index.js`
- Scroll to the bottom where `makeCommits(300)` is called
- Change the `300` to whatever number of total commits you want
- Modify the `moment` timeframe logic to target a different year or timeframe

### 4. Run the Script
When you're ready to create the history, execute the script:
```bash
npm start
```
*Alternatively run `node index.js`*

Sit back and watch the magic happen! The script will loop and generate the fake commits locally and automatically `push` them to your GitHub profile branch.

---

## 🎨 Creative Ideas & Next Steps
- **Paint Shapes:** Instead of passing random inputs, map an X (weeks) & Y (days) grid loop to draw specific letters, words, or pixel art!
- **Commit Density:** Instead of one random commit in a day, map multiple to increase the "darkness" of the green square.

---

## ⚠️ Disclaimer
While this is a super fun way to demonstrate automation using JavaScript and Git internals to trick GitHub's UI graph, remember that relying *solely* on fake commits to impress recruiters might not work—they typically check the code contents too! Use it for fun, art, or just a cool flex.

---
### 👤 Built by Rudransh
🔗 [GitHub Profile](https://github.com/rudransh-ai-dev)
