#  Autonomous Delivery Agent

# Course: Artificial Intelligence

# Author: Yash Samadhan Jadhav



# Overview

This project is about a delivery agent that can navigate through a grid. The grid has obstacles and the agent needs to find the path. It uses algorithms like **Uniform Cost Search (UCS)** **A*** and **Simulated Annealing (SA)** to find the path.

The agent can change its path if something new gets in its way. This makes it good at handling surprises.



# Environment Model

* The environment is a grid made up of squares.

* Each square has a cost to move into (it costs least 1).

* A cost of `0` means you can't move into that square (its blocked).

* You can move up down left or right.

* If something blocks your path the agent can replan its route.



#⚙️ Algorithms Used

* **Uniform Cost Search (UCS)** finds the path that costs the least.

* **A*** uses a guess to find the best path.

* **Simulated Annealing (SA)** helps the agent replan if something gets in its way.



# Installation & Setup

* You need Python version **3.8 or higher** (it was tested on 3.12).

* You don't need to install anything

```bash

git clone https://github.com/yourusername/CSA2001-Autonomous-Delivery-Agent.git

cd CSA2001-Autonomous-Delivery-Agent

python agent.py

```



# How to Run

run:

```bash

python agent.py

```

### Output Includes:

* How much the path costs

* How long the path is

* How steps it took to find the path

* How long it took to run



# Available Maps

* `small_map.txt`

* `medium_map.txt`

* `large_map.txt`

* `dynamic_map.txt`



# Dynamic Obstacle Handling

* The agent first plans its path using **A***.

* If something gets in its way it replans using ** Annealing**.

* This shows how the agent can adapt.



# Testing & Reproducibility

* The project has checks to make sure the path is correct and avoids obstacles.

* The random seed is set to `42`:

```python

random.seed(42)

```

* This means you get the results every time.



# Analysis

* A comparison of how well **UCS** **A*** and **SA** work.

* It looks at:

* How long it takes to run

* How steps it takes to find the path

* How good the path is

📄 There's a report in: `report.pdf`



# Demo

You can see screenshots in:

```

demo_screenshots/

```

It shows:

* The agent planning its path

* Something getting in its way

* The agent replanning



# Grid File Format

```

rows cols start_r start_c goal_c

grid values row by row

```

For example:

```

5 5 0 0 4 4

1 1 1 0 1

1 0 1 1 1

1 1 1 0 1

0 1 1 1 1

1 1 0 1 1

```



# Key Features

* The agent uses algorithms to find its path.

* It can replan if something gets in its way.

* It's efficient and easy to understand.

* The project setup is consistent and reliable.





This project shows how AI can be used in real-world delivery systems. It highlights how agents can adapt and make decisions.



# References

* "Artificial Intelligence: A Modern Approach" by Stuart Russell

* Online resources, on **UCS** **A***. *Simulated Annealing**

* Python documentation



⭐ *If you found this project useful give it a star!*
