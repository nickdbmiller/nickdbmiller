[![Lime green geometric design. Get in touch to learn more!](./assets/images/Github.png)](mailto:nickbarrettmiller@gmail.com)

# Currently open to work. Click a badge to get in touch!
[![Gmail contact badge](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:nickbarrettmiller@gmail.com)
[![LinkedIn badge](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/ndbmiller/)

## Welcome!
> As a web developer I am driven to simplify intricate problems. My background in systems level thinking enables me to see the sum of complex interactions. Solving tough challenges inspires me to pursue information with tenacity and confidence, and intuit creative ways to overcome obstacles.

## Some stats about me:
[![Nick Miller's GitHub stats](https://github-readme-stats.vercel.app/api?username=nickdbmiller&show_icons=true&theme=chartreuse-dark)](https://github.com/anuraghazra/github-readme-stats) [![Nick Miller's most used programming languages](https://github-readme-stats.vercel.app/api/top-langs/?username=nickdbmiller&layout=compact&theme=chartreuse-dark)](https://github.com/anuraghazra/github-readme-stats)

## My skills include (but are not limited to):
##### Click any badge to learn more about my stack!

### Front End:
[![JavaScript badge](https://img.shields.io/badge/JavaScript-323330?style=for-the-badge&logo=javascript&logoColor=F7DF1E)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![React badge](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)](https://reactjs.org/)
[![HTML5 badge](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Glossary/HTML5)
[![CSS3 badge](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![Tailwind CSS badge](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)](https://tailwindcss.com/)

### Back End:
[![Ruby badge](https://img.shields.io/badge/Ruby-CC342D?style=for-the-badge&logo=ruby&logoColor=white)](https://www.ruby-lang.org/en/)
[![Ruby on Rails badge](https://img.shields.io/badge/Ruby_on_Rails-CC0000?style=for-the-badge&logo=ruby-on-rails&logoColor=white)](https://rubyonrails.org/)
[![PostgreSQL badge](https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white)](https://www.postgresql.org/)
[![Node JS badge](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)](https://nodejs.org/en/about/)
[![Express badge](https://img.shields.io/badge/Express.js-000000?style=for-the-badge&logo=express&logoColor=white)](https://expressjs.com/)
[![MongoDB badge](https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white)](https://www.mongodb.com/)

### Tools:
[![Git badge](https://img.shields.io/badge/GIT-E44C30?style=for-the-badge&logo=git&logoColor=white)](https://git-scm.com/)
[![Github badge](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/nickdbmiller)
[![Figma badge](https://img.shields.io/badge/Figma-F24E1E?style=for-the-badge&logo=figma&logoColor=white)](https://www.figma.com/)

### Deployment:
[![Netlify badge](https://img.shields.io/badge/Netlify-00C7B7?style=for-the-badge&logo=netlify&logoColor=white)](https://www.netlify.com/)
[![Heroku badge](https://img.shields.io/badge/Heroku-430098?style=for-the-badge&logo=heroku&logoColor=white)](https://www.heroku.com/about)

### OS's I use:
[![Linux badge](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)](https://en.wikipedia.org/wiki/Linux)
[![Windows badge](	https://img.shields.io/badge/Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white)](https://en.wikipedia.org/wiki/Microsoft_Windows)
[![Mac OS badge](https://img.shields.io/badge/mac%20os-000000?style=for-the-badge&logo=apple&logoColor=white)](https://en.wikipedia.org/wiki/MacOS)

## Here's some code I wrote recently!
### [Web of Rogues](https://web-of-rogues.netlify.app/)

>These two functions are how objects are randomly rendered in Web of Rogues each time the dungeon is generated. First a list of floor tiles is generated...

```
let currentPlayerPos = null;
let currentStairPos = null;
let floorTiles = [];

function listFloorTiles () {
    for (let r = 1; r <= (dungeonHeight*dungeonWidth); r++) {
        let thisTile = document.getElementById(`-${r}`);
        if (thisTile.className == `floor`) {
            floorTiles.push(`-${r}`);
        };
    };
    return floorTiles;
};
```

>...Then the stairs are put on a random floor tile (using a RNG function declared elsewhere in the script). The tile will always be different than the floor tile the PC is put on to prevent overwriting.

```
function renderStairs () {
    let position = `${floorTiles[RNG(0, (floorTiles.length-1))]}`;
    let tile = document.getElementById(`${position}`);
    currentStairPos = position;
    if (currentPlayerPos == currentStairPos) {
        while (currentPlayerPos == currentStairPos) {
            position = `${floorTiles[RNG(0, (floorTiles.length-1))]}`;
            tile = document.getElementById(`${position}`);
            currentStairPos = position;
        }
        tile.innerText = `>`;
    } else {
        tile.innerText = `>`;
    };
};
```

## Thanks for stopping by! [![visitor count badge](https://visitor-badge.glitch.me/badge?page_id=nickdbmiller.nickdbmiller)](https://visitor-badge.glitch.me/#docs)

## Reach out to me about projects, problems, and coding!
[![Gmail contact badge](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:nickbarrettmiller@gmail.com)
[![LinkedIn badge](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/ndbmiller/)

- ###### [Badges by Alexandre Sanlim.](https://github.com/alexandresanlim/Badges4-README.md-Profile)

- ###### [Visitor count badge project on glitch.](https://visitor-badge.glitch.me/)

- ###### [Banner created with Figma.](https://www.figma.com/)
