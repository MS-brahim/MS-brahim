## Hi there 👋 You are welcome to my Github



- 🔭 I’m currently working on PRF && PP
- 🌱 I’m currently learning MERN Stack

## Skills
:bowtie: HTML
:smile: CSS
:satisfied: JAVASCRIPT
:laughing: REACT
:blush: Technical Writing
:smiley: Git
:relaxed: NODEJS

<!--
**MS-brahim/MS-brahim** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->

on:
  workflow_dispatch:
  schedule:
    # Runs at 12am UTC
    - cron: "0 0 * * *"

jobs:
  update-readme:
    name: Update this repo's README
    runs-on: ubuntu-latest
    steps:
      - uses: athul/waka-readme@master
        with:
          WAKATIME_API_KEY: ${{ secrets.WAKATIME_API_KEY }}
