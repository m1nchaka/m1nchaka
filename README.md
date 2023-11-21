<div align="center">

#  💫 About Me:
🔭 I code just for fun



<!-- # Stats: -->

<!--![](https://github-readme-stats.vercel.app/api?username=m1nchaka&theme=radical&hide_border=false&include_all_commits=false&count_private=false)<br/> -->

<!--![](https://github-readme-streak-stats.herokuapp.com/?user=m1nchaka&theme=radical&hide_border=false)<br/> -->







<!-- Proudly created with GPRM ( https://gprm.itsvg.in ) -->



<h2 align="center">Languages and Tools:</h2>
<p align="center"> <a href="https://www.w3schools.com/html/default.asp" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original-wordmark.svg" alt="html5" width="40" height="40"/> </a><a href="https://www.w3schools.com/css/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original-wordmark.svg" alt="css3" width="40" height="40"/> </a> <a href="https://firebase.google.com/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/firebase/firebase-icon.svg" alt="firebase" width="40" height="40"/> </a> <a <a href="https://www.w3schools.com/js/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-original.svg" alt="javascript" width="40" height="40"/> </a> <a href="https://www.w3schools.com/c/c_intro.php" target="_blank" rel="noreferrer"> <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/1/18/C_Programming_Language.svg/926px-C_Programming_Language.svg.png" alt="css3" width="40" height="40"/> </a> </p>
<h5 align="center">Click on the icons to learn more about it</h5>


---

![](https://github-readme-stats.vercel.app/api/top-langs/?username=m1nchaka&theme=radical&hide_border=false&include_all_commits=false&count_private=false&layout=compact)

<h3 align="left">Connect with me on github</h>
<p align="left">
</p>
</div>

<!-- [![](https://visitcount.itsvg.in/api?id=m1nchaka&icon=7&color=6)](https://visitcount.itsvg.in) -->




#include <stdio.h>
#include <stdlib.h>
#include <time.h>

// Function to display task condition and author's name
void displayTaskInfo() {
    printf("Task: Process a one-dimensional array A(20) with values in the interval (-99 to +99)\n");
    printf("Author: Your Name\n\n");
}

// Function to fill the array with random values in the given interval
void fillArray(int A[], int size) {
    srand(time(NULL)); // Seed for random number generation

    for (int i = 0; i < size; i++) {
        A[i] = rand() % 199 - 99; // Generates random number in the range [-99, 99]
    }
}

// Function to display the contents of the array
void displayArray(int A[], int size) {
    printf("Array Contents:\n");

    for (int i = 0; i < size; i++) {
        printf("%d ", A[i]);
    }

    printf("\n");
}

int main() {
    // Declare and initialize the array
    int A[20];

    // Display task information
    displayTaskInfo();

    // Fill the array with random values in the specified interval
    fillArray(A, 20);

    // Display the contents of the array
    displayArray(A, 20);

    return 0;
}

