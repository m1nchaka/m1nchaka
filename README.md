<div align="center">

#  💫 About Me:
🔭 I’m currently working on Graduation Project using Firebase



# 📊 GitHub Stats:

![](https://github-readme-stats.vercel.app/api?username=m1nchaka&theme=radical&hide_border=false&include_all_commits=false&count_private=false)<br/>

![](https://github-readme-streak-stats.herokuapp.com/?user=m1nchaka&theme=radical&hide_border=false)<br/>

![](https://github-readme-stats.vercel.app/api/top-langs/?username=m1nchaka&theme=radical&hide_border=false&include_all_commits=false&count_private=false&layout=compact)


---


<!-- Proudly created with GPRM ( https://gprm.itsvg.in ) -->



<h3 align="center">Languages and Tools:</h3>
<p align="center"> <a href="https://www.w3schools.com/css/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original-wordmark.svg" alt="css3" width="40" height="40"/> </a> <a href="https://firebase.google.com/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/firebase/firebase-icon.svg" alt="firebase" width="40" height="40"/> </a> <a href="https://www.w3schools.com/html/default.asp" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original-wordmark.svg" alt="html5" width="40" height="40"/> </a> <a href="https://www.w3schools.com/js/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-original.svg" alt="javascript" width="40" height="40"/> </a>  </p>


<h3 align="left">Connect with me on github</h3>
<p align="left">
</p>
</div>

[![](https://visitcount.itsvg.in/api?id=m1nchaka&icon=7&color=6)](https://visitcount.itsvg.in)






```c
#include <stdio.h>
#include <stdbool.h>

bool isLeapYear(int year) {
    if ((year % 4 == 0 && year % 100 != 0) || (year % 400 == 0)) {
        return true;
    }
    return false;
}

int main() {
    int day, month, year;
    bool valid = true;

    printf("Vuvedete dati (den mesec godina): ");
    scanf("%d %d %d", &day, &month, &year);

    bool leap = isLeapYear(year);

    if (month < 1 || month > 12) {
        valid = false;
    } else if (month == 2) {
        if (leap && (day < 1 || day > 29)) {
            valid = false;
        } else if (!leap && (day < 1 || day > 28)) {
            valid = false;
        }
    } else if ((month == 4 || month == 6 || month == 9 || month == 11) && (day < 1 || day > 30)) {
        valid = false;
    } else if (day < 1 || day > 31) {
        valid = false;
    }

    if (valid) {
        printf("Vuvedenite dati  %d-%d-%d e validen.\n", day, month, year);
    } else {
        printf("Vuvedenite dati ne e validen.\n");
    }

    return 0;
}```