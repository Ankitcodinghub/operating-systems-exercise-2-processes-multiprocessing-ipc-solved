# operating-systems-exercise-2-processes-multiprocessing-ipc-solved
**TO GET THIS SOLUTION VISIT:** [Operating Systems Exercise 2-Processes, Multiprocessing , IPC Solved](https://www.ankitcodinghub.com/product/operating-systems-exercise-2-processes-multiprocessing-ipc-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;99218&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;0&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;0&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;0\/5 - (0 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;Operating Systems Exercise 2-Processes, Multiprocessing , IPC Solved&quot;,&quot;width&quot;:&quot;0&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 0px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            <span class="kksr-muted">Rate this product</span>
    </div>
    </div>
<div class="page" title="Page 1">
<div class="layoutArea">
<div class="column">
Exercise 2 Processes, Multiprocessing &amp; IPC

<ul>
<li>Part 1
In this question we will implement a C application that checks the response time of Internet URLs. The application should receive a file containing a list of URLs and the number of workers we want to use. After a successful run the application prints a numeric average of the successful URL queries, number of sites reached and the number of unknowns (for URLs it failed to test).

You will implement it in both methods, PIPE and Memory mapping. Add a flag “-f” in case you run it with pipe and without this flag the program run using memory mapping.
</li>
</ul>
1. In addition to the manual pages from exercise 1, read the manual page for the following System Calls:

</div>
</div>
<div class="layoutArea">
<div class="column">
<ol>
<li>FORK(2)</li>
<li>PIPE(2)</li>
<li>SIGNAL(7)</li>
<li>MMAP(2)</li>
<li>semaphore.h(0p)</li>
</ol>
</div>
<div class="column">
i.e. execute: man 2 fork also read PIPE(7)

</div>
</div>
<div class="layoutArea">
<div class="column">
<ol start="2">
<li>Install the libcurl development package on your VM:
sudo apt-get install libcurl3-dev
</li>
<li>Create a new eclipse project for exercise 2, and change the following:</li>
</ol>
a. Project-&gt;Properties-&gt;C/C++ Build-&gt;Settings-&gt;Tool Settings-&gt;Cross GCC Linker-&gt;Libraries-

&gt;Add…-&gt;”curl” (do the same with “rt” and “pthread“ instead of “curl”) 4. Complete the application ex2.c (missing parts are marked with //TODO)

</div>
</div>
</div>
<div class="page" title="Page 2">
<div class="layoutArea">
<div class="column">
Examples (numbers might vary between runs)

$ ./ex2

usage:

./ex2 NUMBER_OF_PROCESSES FILENAME

$ ./ex2 1 top10.txt

0.0146 Average response time from 8 sites, 2 Unknown

$ ./ex2 2 top10.txt -f

0.1002 Average response time from 9 sites, 1 Unknown

$ ./ex2 10 top10.txt

Illegal url detected, exiting now

Guidelines

<ul>
<li>● &nbsp;Use the manual.</li>
<li>● &nbsp;Make sure to always close the files you open.</li>
</ul>
○ Same goes for pipes.

<ul>
<li>● &nbsp;A parent must wait for all his/her child processes.</li>
<li>● &nbsp;Always check syscalls return value for errors. ALWAYS.</li>
<li>● &nbsp;You are not allowed to use any additional external libraries, if you are not sure if you are allowed to
use something, ask in the forusudo m.
</li>
</ul>
○ You may use any function that was already used in the provided skeleton.

<ul>
<li>● &nbsp;You may assume that the function input is valid.</li>
<li>● &nbsp;Feel free to change the internals of given functions, but not their signatures.</li>
<li>● &nbsp;Notice that when compiling using gcc on the terminal, you should still use the “-lcurl” flag.</li>
<li>● &nbsp;Do not change the program output, i.e. the print statements.</li>
<li>● &nbsp;The check_url function returns a URL_ERROR if a URL address doesn’t start with ‘http’. If your
program receives a URL_ERROR, all processes (parent and children) must exit immediately and

the following message should be printed: “Illegal url detected, exiting now”.
</li>
<li>● &nbsp;Hint: a struct is just a bunch of bits, you can write() and read() structs.
Using Docker for Smoke Testing
</li>
</ul>
<ul>
<li>The VM is installed with Docker software (more on that later in the semester).</li>
<li>When being graded, your solution will be tested in a container identical to the one that will
be built using the supplied Dockerfile.
</li>
<li>There are two smoke tests (sanity checks) to this exercise. You can explore the
‘EX2/check_submission/do_not_change’ folder for more details
</li>
</ul>
o The first test checks your program against 10 international URLs using memory

mapping

o The second test checks your program against 8 Israeli URLs using pipe

• Usage:

o You’re given EX2 folder, containing:

▪ A ‘check_submission’ folder, which contains a python script to execute (check_submission.py).

</div>
</div>
</div>
<div class="page" title="Page 3">
<div class="layoutArea">
<div class="column">
▪ A skeleton file ‘ex2.c’

▪ Two text files: ‘top10.txt’, ‘top128.txt’

o Do not move ANY of the files inside check_submission, or you won’t be able to use

our tests.

o You should edit ‘ex2.c’ with your solution.

o Each time you want to test your final submission file (zip file):

<ul>
<li>▪ &nbsp;Open a terminal and go the EX2/check_submission.</li>
<li>▪ &nbsp;copy your submission file (ex2-YOUR_ID.zip) to your machine (anywhere
you want)
</li>
<li>▪ &nbsp;Execute ‘python check_submission.py &lt;full path to your submission file&gt;’
If everything is fine, you will get:
</li>
<li>▪ &nbsp;Average response times may vary. Under some conditions one or two URLs may not respond; it is fine, but make sure that at least one of your runs is without unknown sites</li>
</ul>
</div>
</div>
</div>
