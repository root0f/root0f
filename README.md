- 👋 Hi, I’m Ilmir Mavliutov
- 🌱 My tech stack: JavaScript, HTML, CSS, ReactJS, TypeScript
- 📫 How to reach me: Email: mavlutov@bk.ru or mechasop@gmail.com, Telegram: [@D_R_ROBOT](https://t.me/D_R_ROBOT), LinkedIn: [Ilmir Mavlyutov](https://www.linkedin.com/in/ilmir-mavliutov-01265a20a/)
- 🤓 CODEWARS: https://www.codewars.com/users/D_R_ROBOT
- 👀 Hobbies other than coding: 🏋 weightlifting
- name: Generate Snake
on:
  schedule:
    - cron: "0 0 * * *"  # Ежедневно в полночь
  workflow_dispatch:
jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - uses: Platane/snk@master
        id: snake
        with:
          github_token: ${{ secrets.GITHUB_TOKEN }}
      - uses: crazy-max/ghaction-github-pages@v2.1.3
        with:
          target_branch: output
          build_dir: output
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}


<!---
root0f/root0f is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
