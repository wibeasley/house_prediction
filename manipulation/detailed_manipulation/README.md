`./manipulation/detailed_manipulation/` Directory
=========

When there are many tests/tasks involved in the data manipulation procedure, files that actually do the data manipulation process can be moved into this sub-directory to keep the folder organized. Then these file will be sourced inside some organizing/combining R files in the `./manipulation/` folder based on their purposes. The concept is that by modularizing each manipulation process for each task, it's easier and quicker to find out where bugs are and debug. It is also more visually friendly, especially for people who get in touch with the folder for the first time. 

=========
Here is an example
./manipulation/
    global.r                    # where you define packages/functions/data.versions
    baseline.r
    test.results.r
    status.r
    adverse.events.r
    detailed_manipulation/
        test_a.r
        test_b.r
        test_c.r
        test_d.r
        test_f.r
        baseline_screening_test.r
        demongraphics.r
        .
        .
        .