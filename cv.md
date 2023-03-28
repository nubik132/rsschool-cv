# Vladislav Hilchuk
### Contact Inforamtion
* **PHONE**: +375298249428
* **E-MAIL**: mister.nubik@list.ru
* **DISCORD**: nubik132#7407
* **TELEGRAM**: https://t.me/nubik132

### About Myself:

As a purposeful individual with a passion for learning, I take on every opportunity as a chance to expand my skillset and knowledge. I am motivated by a desire to succeed and will work tirelessly to achieve my goals. If I commit to a task, I am dedicated to seeing it through to the very end. Whether it's learning a new skill or completing a project, I always strive to do my best and produce high-quality work.

### Skills and Proficiency:

* HTML5, CSS
* JS, C++, Java (Basic)
* C#, Python
* Git (Basic)
* Visual Studio, Visual Studio Code
* Adobe Photoshop

### Code example:

kata (4 kyu) from [Codewars](https://www.codewars.com/kata/human-readable-duration-format)

Your task in order to complete this Kata is to write a function which formats a duration, given as a number of seconds, in a human-friendly way.

The function must accept a non-negative integer. If it is zero, it just returns "now". Otherwise, the duration is expressed as a combination of years, days, hours, minutes and seconds.

<!-- CodeWars -->
```
function formatDuration(seconds) {
    if (seconds == 0) {
        return "now";
    }

    const minute = 60;
    const hour = 60 * 60;
    const day = 60 * 60 * 24;
    const year = 60 * 60 * 24 * 365;
    const dates = [year, day, hour, minute];
    const strDates = ["year", "day", "hour", "minute", "second"];

    let factDates = [0, 0, 0, 0, 0];


    for (const key in dates) {
        factDates[key] = Math.trunc(seconds / dates[key]);
        seconds = seconds % dates[key];
    }

    factDates[4] = seconds;

    let notNullAnswers = [];

    for (let i = 0; i < factDates.length; i++) {
        if (factDates[i] !== 0) {
            let strAnswer = '';
            strAnswer = (`${factDates[i]} ${strDates[i]}`);

            if (factDates[i] > 1) strAnswer += 's';

            notNullAnswers.push(strAnswer);
        };
    }

    if (notNullAnswers.length > 1){
        return notNullAnswers.slice(0, notNullAnswers.length - 1).join(", ")
         + " and " + notNullAnswers[notNullAnswers.length - 1];
    }
    return notNullAnswers[0];
}
```
### Courses

* Python course on [Courcera](https://coursera.org/share/84c3673efd5f56ef0676cbbd9a638ed1)
* JavaScript Manual on learnjavascript.ru (in progress)
* RS Schools Course «JavaScript/Front-end. Stage 0» (in progress)
English: B1/B2 (according to [EFSET](https://www.efset.org/quick-check/take-test/#set15-190/result)).