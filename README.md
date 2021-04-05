# Devops-Handbook
Personal notes on the book

## First Way: Principles of Flow

The First Way elaborates on principles for movement from left to right of the value chain, and how to make it go faster and smoother.

1. Make all work visible to everyone (e.g. usage of Kanboard)
2. Limit Work-In-Progress (WIP). Stop Starting, Start Finishing!
3. ***Reduce Batch Sizes. Do work in smaller batch sizes, instead of a big-bang approach***
4. Reduce number of work handoffs. Context may get lost in transition. We can do this by automating most stuff.
5. Identify and elevate constraints. Some common constraints are:
    - ***Environment Creation: Creating Production or Testing environment should be automated***
    - ***Code Deployment: Deploying code should be automated and self-service***
    - ***Test setup and Run: Running test cases should be automated***
    - Overly Tight Architecture: How easy is it to commit changes without breaking stuff?
6. Eliminate Hardship and Waste in the Valuestream
    - Partially Done Work: See (2.) Limiting WIP
    - Extra Processes: Unecessary reviews, approvals, or documentation that do not add value
    - Extra Features: Unnecessary features that do not add value (Gold-Plating software)
    - Task Switching: see (2.) Limiting WIP
    - Waiting: see (4.) Reducing Handoffs. Reducing waiting time in the value chain
    - Motion: see (4.) Reducing Handoffs. Make movement in the value chain seamless
    - Defects: Incorrect or missing information slows down the value chain
    - Non-Standard/Manual work: Automated the boring stuff
    - Heroics: Unreasonable workloads, or one-man carry

## Second Way: Principles of Feedback

The Second Way elaborates on principles for movement from right to left of the value chain, giving feeback to the systems prior.

How to work safetly in Complex Systems
1. Complex work is managed so that problems in the design and operations are revealed
    - See problems as they occur through feedback and feedforward strategies
    - This includes PM, QA, Development, Infosec and Operations
    - Automate build and test processes so facilitate faster feedback/feedforward
    - ***Create pervasive telemetry all over***
3. These problems are swarmed and solved, resulting in construction of new knowledge
    - ***Don't fix when you have the time, gather all resources to swarm the problem immediately***
    - This prevent the problem from progressing downstream, which snowballs the technical debt
    - Prevents starting of new work to solve the issue from independent parties
    - Prevents recurrance in the future
    - Create an Andon Cord, which triggers the swarm immediately
5. The new knowledge is exploited globally across the organization
    - Adding more inspections and approvals actually increases the chance of failure
    - ***When more layers of approvals are added, the decisions are made further away from the work, thus diminishing the value***
    - Inefficient controls include adding too much documentation
7. Leaders create other leaders who continually grow these capabilities


There are two types of customers
1. The external paying customer (of the product)
2. ***The internal consuming customer (downstream of your work). This is the more important customer***


