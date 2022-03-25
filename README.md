- [Group Enargite](#group-enargite)
- [Authers](#authers)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Running the test](#running-the-test)
  - [CODE TEST](#code-test)
  - [Workflow???](#workflow)
- [visualization](#visualization)
- [License](#license)

## Group Enargite

This program is designed for mineral processing to obtain the optimal loop for two products (concentration and tailings). Genetic Algorithms is the core tool that we used to achieve this goal. In addition to this, two helper functions named check validity process and check monetary value are used to screen for potential circuits. Finally, the optimum circuit configuration is plotted by using a graph.

## Authers

Group Members - Kairui Kou, Kefan Wang, Nikhil Kumar, Nourhan Berwaji, Yan Chan, Yuhang Zhang, Siyuan Jiang, Shengnan Li



## Prerequisites

For the development of this project, you should install the following tools before running the code.

- [CMake](https://cmake.org/)
- [Visual Studio Code](https://code.visualstudio.com/)
- [Python](https://www.python.org/)



## Installation

- Clone this repo to your local machine using:

```
https://github.com/ese-msc-2021/acs-gormanium-rush-enargite.git
```

- Complie the program

```
make 
make tests
```

- Run the program

  On Mac

```
./bin/Genetic_Algorithm
```

​		On windows

```
add something...
```



## Running the test

### CODE TEST

There are few test cases that we performed to make sure all the function can work properly, please use the following command to test and run it on your machine

1. CPP files

```sh
make tests
```

2. Python files

```sh
# if __name__ == "__main__":
#     import doctest

#     doctest.testmod(verbose=True)
```

Please just uncomment these lines in visualization.py and run it

### Workflow???



## visualization

Graphviz is a python package that we need to plot the graph. First, let us create a 'conda' environment

```
conda env create -f environment.yml
conda activate plotenv
```



We decided to save the ouput from previous step to a txt file, can be seen as follows：

```
vector=4, 10, 1, 0, 8, 5, 3, 1, 11, 1, 9, 1, 6, 2, 9, 8, 2, 0, 2, 5, 7, optimum=222.612
vector=4, 10, 1, 0, 8, 5, 3, 1, 11, 1, 9, 1, 6, 7, 9, 8, 2, 0, 2, 5, 7, optimum=225.363
vector=4, 10, 1, 0, 8, 5, 3, 1, 11, 1, 9, 1, 6, 5, 9, 8, 2, 0, 2, 5, 7, optimum=249.751
vector=4, 10, 1, 0, 8, 5, 3, 1, 11, 1, 9, 1, 6, 5, 9, 8, 2, 0, 5, 5, 7, optimum=304.901
vector=4, 10, 1, 0, 8, 8, 3, 1, 11, 1, 9, 1, 6, 5, 9, 8, 2, 0, 5, 5, 7, optimum=311.65
vector=4, 10, 1, 0, 8, 5, 3, 1, 11, 1, 9, 1, 6, 1, 9, 8, 2, 0, 5, 5, 7, optimum=318.496
vector=4, 10, 1, 0, 8, 5, 3, 1, 11, 1, 9, 1, 6, 5, 9, 8, 2, 1, 5, 5, 7, optimum=337.044
vector=4, 10, 1, 0, 8, 5, 3, 1, 11, 1, 9, 1, 6, 1, 9, 8, 2, 1, 5, 5, 7, optimum=356.141
vector=4, 10, 1, 0, 8, 8, 3, 1, 11, 1, 9, 1, 6, 1, 9, 8, 2, 1, 5, 5, 7, optimum=357.874
vector=4, 10, 1, 0, 8, 5, 3, 8, 11, 1, 9, 1, 6, 1, 9, 8, 2, 1, 5, 5, 7, optimum=362.984
vector=4, 10, 1, 0, 8, 8, 3, 5, 11, 1, 9, 1, 6, 1, 9, 8, 2, 1, 5, 5, 7, optimum=363.59
vector=4, 10, 1, 0, 8, 8, 3, 8, 11, 1, 9, 1, 6, 1, 9, 8, 2, 1, 5, 5, 7, optimum=364.724
vector=4, 10, 1, 0, 8, 5, 3, 8, 11, 1, 9, 1, 6, 1, 4, 8, 2, 1, 5, 5, 7, optimum=366.532
vector=4, 10, 1, 0, 8, 5, 3, 8, 11, 5, 9, 1, 6, 1, 4, 8, 2, 1, 5, 5, 7, optimum=368.08
vector=4, 10, 1, 0, 8, 5, 3, 5, 11, 8, 9, 1, 6, 1, 4, 8, 2, 1, 5, 5, 7, optimum=371.065
vector=4, 10, 1, 0, 8, 5, 3, 8, 11, 8, 9, 1, 6, 1, 4, 8, 2, 1, 5, 5, 7, optimum=372.015
vector=4, 10, 1, 0, 8, 5, 3, 8, 11, 8, 9, 1, 6, 1, 4, 8, 2, 1, 5, 8, 7, optimum=374.465
vector=4, 10, 1, 0, 8, 8, 3, 8, 11, 8, 9, 1, 6, 1, 4, 8, 2, 1, 5, 8, 7, optimum=375.495
vector=4, 10, 1, 0, 8, 8, 3, 8, 11, 8, 9, 1, 6, 1, 4, 8, 2, 1, 5, 8, 7, optimum=375.495
```

If you are interested at both the images and gif of simple circuits, please enter to view them:

```
python visualization.py
```

Finally,  you can see result in a folder named post_processing_result containing  many written texts and jpgs, you can also see a file named result.gif, in which the gif illustrates how the convergence path towards the optimum circult.



## License

This project is licensed under the MIT License - see the [LICENSE.md](https://github.com/ese-msc-2021/acs-gormanium-rush-enargite/blob/main/LICENSE) file for details

