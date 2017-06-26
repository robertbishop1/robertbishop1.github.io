## Robert Bishop's Portfolio
<center>![alt text](https://lh3.googleusercontent.com/s2IoZOvHkMc8HxbeMxb_GchfD7ICVz73jAkfXuF9L-ApBhUK_zMYRoTwuhgCgFi5ADkqZMQgsGUm5FTR_BTcRQZP_tK6fmr3fB985FnmmtbZtXiFRxzV7k3r3MGRWivYfPC-pWCsktxZrh6GJXjaul8-7-M2hU8sGcG9kH1iwsM5EkArnQxQbINqf36P3M5rM1SDX4baFVHMnN2PNGoJY6lqcAF2ElTPAPjSN4oqCK2mNviNYUS9YChjG4IGpnxjLRdq3Ol0AlFZJaIa19bVlGx9rudENcZ0q0Wh8jUVRkeuLJos41lTvD3tNnETRAdAhcXEqi9IwKK8u2Eag8TAdccpThFMIf5S1n84uZlfL4Z9uVrPUr1tt-IBo7RWdI6cnC3tTx1et9ipIKVAKLzLJ74bLYkIrtrzdYSqw6J_j2o27TavnCCYWAu7msw_fRfl9dnoWtunp81w7TycCqvrEAW2m35tWqOdGv-7DIBQSkdZA8mo6ab3jduKxHmhd-U3uXtUC1Of9qluINT9WRYYKhikISgiYtrGSBsmgZi5VVFDKXaSUTp2XyQ8XHyushrcV0r12YgIM2RrallMR3rvvQn3XxSIGpdm5C4PGeCVBKAWpCz7Y-WTqtFOmjU0kadeynd-4zFiCl7-OgJIOfijSzkYTdlbIo1bIOPPCGBLp60 "Me")</center>

## Here are some of my recent projects.

### This project is a simple calculator for movie theater profits.
```c++
// This application calculates gross and net box office profit for a theater.
#include <iostream>
#include <string>
#include <iomanip>
using std::cout;
using std::endl;
using std::cin;
using std::showpoint;
using std::fixed;
using std::setprecision;
using std::string;
using std::right;
using std::setw;

int main()  {
    // Stores the movie title
    string movieName;
    cout << "What is the movie name:" <<endl;
    getline(cin, movieName);

    // Stores values of adult tickets
    int adultTicket = 12;
    int totalAdultSales;
    cout << "How many Adult tickets sold:" << endl;
    cin >> totalAdultSales;

    // Stores value of child tickets
    int childTicket = 9;
    int totalChildSales;
    cout << "How many Child tickets sold:" << endl;
    cin >> totalChildSales;

    // Prints movie title with quotes
    string addPar = "\"" + movieName + "\"";
    cout << "Movie Name:" << setw(30) << right << addPar <<endl;

    // Prints adult ticket sales
    cout << "Adult Tickets Sold:" << setw(12) << setprecision(2)
         << fixed << totalAdultSales << endl;

    // Prints child ticket sales
    cout << "Child Tickets Sold:" << setw(12) << totalChildSales << endl;

    // Prints and calculates gross profit
    double grossCal = (adultTicket * totalAdultSales)
                      + (childTicket * totalChildSales);
    cout << "Gross Box Office Profit:" << setw(8) << showpoint
         << "$ " << grossCal << endl;

    // Prints and calculates net profit
    double netCal = grossCal *0.22;
    cout << "Net Box Office Profit:" << setw(10)
         << showpoint << "$ " << netCal<< endl;

    // Prints amount paid to Dist
    cout << "Amount Paid to Distributor:" << setw(5) << showpoint << "$ "
         << grossCal - netCal << endl << endl;

    // Pauses screen for viewing
    char pause = cin.get();
    cout << "Press enter to continue: ";
    cin.get(pause);
    return 0;
}

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/robertbishop1/robertbishop1.github.io/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
