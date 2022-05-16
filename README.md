
## Hello, I'm [AbhishekTungala!](https://google.com) <img src="https://raw.githubusercontent.com/MartinHeinz/MartinHeinz/master/wave.gif" width="30px"> 
[![Typing SVG](https://readme-typing-svg.herokuapp.com?size=25&color=1A9AF7&lines=I'm+Full+Stack+Web+Developer;and+Competitive+Coder)](https://git.io/typing-svg)
    



## just a Introduction:

Hi, I'm Abhishek Tungala, A Student and Learner 🚀 from Hyderabad,Telangana, India, currently 💻 doing my undergraduate BTECH (1st year) from Lovely professional university and I am passionate about technology and want to learn & explore new technologies ,Beside's Computer Science, I love photography, Travelling.




### Talking about Personal Stuffs:

- 👋 Hi, I’m AbhishekTungala
- 👀 I’m currently partcipating in as much Hackathons as I can...
- 👀 I’m interested in Data Science, Full Stack Web Development
- 🌱 I’m currently learning Mern 🤟 ...
- 💬 Ask me about anything, I am happy to help


---

[![Abhishek github activity graph](https://activity-graph.herokuapp.com/graph?username=AbhishekTungala&theme=react-dark)](https://github.com/AbhishekTungala)


### 📊 Some Fun Stats:
| ![image](https://github-readme-stats.vercel.app/api?username=AbhishekTungala&&show_icons=true&title_colour=ffffff&icon_color=bb2acf&text_color=daf7dc&bg_color=151515) | ![My Stats](https://github-readme-stats.vercel.app/api/top-langs/?username=AbhishekTungala&theme=midnight-purple) | 
| --- | --- |
😍 Total Views on Profile:<br><br>
![Visitor Count](https://profile-counter.glitch.me/AbhishekTungala/count.svg) |



### 🍁 My Skill stack :

|               |           |
|       ---     |    ---    |
| `Web-Dev`     | ![HTML5](https://img.shields.io/badge/-HTML5-CC2400?style=for-the-badge&logo=html5&logoColor=white) ![CSS3](https://img.shields.io/badge/-CSS3-E24800?style=for-the-badge&logo=css3) ![JavaScript](https://img.shields.io/badge/-JavaScript-FE7601?style=for-the-badge&logo=javascript) |
| `Languages`   | ![C++](https://img.shields.io/badge/-C++-034D9A?style=for-the-badge&logo=c%2B%2B) ![C](https://img.shields.io/badge/-C-034D9A?style=for-the-badge&logo=c%2B%2B) ![Python](https://img.shields.io/badge/-Python-1F65AC?style=for-the-badge&logo=Python&logoColor=white) |
| `Tools`       | ![VS Code](https://img.shields.io/badge/Visual_Studio_Code-5D1A60?style=for-the-badge&logo=visual%20studio%20code&logoColor=white) ![Git](https://img.shields.io/badge/Git-682181?style=for-the-badge&logo=git&logoColor=white) |

___  

### 🤝 Connect with me:

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/abhishek-tungala-bb46a2220)
[![Twitter](https://img.shields.io/badge/Twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white)](https://twitter.com/abhishektungala)
[![Instagram](https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white)](https://www.instagram.com/_.abhi._.1212._/)
[![GMail](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:abhishektungala1212@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/AbhishekTungala)




<h2>🏆 Github Profile Trophy</h2>
<a href="https://github.com/ryo-ma/github-profile-trophy">
  <img height="180" src="https://github-profile-trophy.vercel.app/?username=AbhishekTungala&column=8&theme=algolia&no-frame=true"/>
</a>



![](https://raw.githubusercontent.com/halfrost/halfrost/master/icons/header_.png)



### 🐍 Watch Snake eating my contribution:
![snake svg](https://github.com/spyder15/spyder15/blob/output/github-contribution-grid-snake.svg)

# GitHub Action for generating a contribution graph with a snake eating your contributions.

name: Generate Snake

# Controls when the action will run. This action runs every 6 hours.

on:
  schedule:
      # every 6 hours
    - cron: "0 */6 * * *"

# This command allows us to run the Action automatically from the Actions tab.
  workflow_dispatch:

# The sequence of runs in this workflow:
jobs:
  # This workflow contains a single job called "build"
  build:
    # The type of runner that the job will run on
    runs-on: ubuntu-latest

    # Steps represent a sequence of tasks that will be executed as part of the job
    steps:

    # Checks repo under $GITHUB_WORKSHOP, so your job can access it
      - uses: actions/checkout@v2

    # Generates the snake  
      - uses: Platane/snk@master
        id: snake-gif
        with:
          github_user_name: AbhishekTungala
          # these next 2 lines generate the files on a branch called "output". This keeps the main branch from cluttering up.
          gif_out_path: dist/github-contribution-grid-snake.gif
          svg_out_path: dist/github-contribution-grid-snake.svg

     # show the status of the build. Makes it easier for debugging (if there's any issues).
      - run: git status

      # Push the changes
      - name: Push changes
        uses: ad-m/github-push-action@master
        with:
          github_token: ${{ secrets.GITHUB_TOKEN }}
          branch: master
          force: true

      - uses: crazy-max/ghaction-github-pages@v2.1.3
        with:
          # the output branch we mentioned above
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}

