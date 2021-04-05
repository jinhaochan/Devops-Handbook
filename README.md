# Devops-Handbook
Personal notes on the book

## First Way: Principles of Flow

This First Way elaborates on principles for movement from left to right of the value chain, and how to make it go faster and smoother.

1. Make all work visible to everyone (e.g. usage of Kanboard)
2. Limit Work-In-Progress (WIP). Stop Starting, Start Finishing!
3. Reduce Batch Sizes. Do work in smaller batch sizes, instead of a big-bang approach
4. Reduce number of work handoffs. Context may get lost in transition. We can do this by automating most stuff.
5. Identify and elevate constraints. Some common constraints are:
    - Environment Creation: Creating Production or Testing environment should be automated
    - Code Deployment: Deploying code should be automated and self-service
    - Test setup and Run: Running test cases should be automated
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
