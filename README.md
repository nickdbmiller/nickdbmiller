
[![HTML5 badge](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Glossary/HTML5)
[![CSS3 badge](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![JavaScript badge](https://img.shields.io/badge/JavaScript-323330?style=for-the-badge&logo=javascript&logoColor=F7DF1E)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
## Thanks for stopping by! [![visitor count badge](https://visitor-badge.glitch.me/badge?page_id=nickdbmiller.nickdbmiller)](https://visitor-badge.glitch.me/#docs)

## Hi, my name is Nick!
> I am a builder of systems who seeks to truly understand all that I do, and all that I create. Leveraging my background in Environmental Science and systems level thinking I am able to see the sum of complex interactions, and how my work fits into that complexity. I pursue information with tenacity when dealing with tough challenges to acquire deep knowledge on the obstacle. This is why I have creative ways of seeing answers to problems; I see them from every angle. I bring true motivation and a clear moral compass to everything that I do and every organization I am a part of.

[![Nick Miller's GitHub stats](https://github-readme-stats.vercel.app/api?username=nickdbmiller&show_icons=true&theme=chartreuse-dark)](https://github.com/anuraghazra/github-readme-stats)

[![Nick Miller's most used programming languages](https://github-readme-stats.vercel.app/api/top-langs/?username=nickdbmiller&layout=compact&theme=chartreuse-dark)](https://github.com/anuraghazra/github-readme-stats)

## Here's some code I wrote recently!
### [Web of Rogues Game](https://nickdbmiller.github.io/Web-of-Rogues-Game/)
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