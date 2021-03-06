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

## Third Way: Principles of Continual Learning and Experimentation

The First Way was from left to right, and the Second Way was from right to left. The Third Way goes all around, and speaks more about culture, more specifically one of learning and experimentation. ***This leads to creation of individual knowledge, which must eventually transits to global knowledge***

Values:
- High trust
- Life-long learners
- Risk taking

1. Organizational culture of safety and trust 
    - Dont hoard information, rather, share it freely. Nothing to gain and everything to lose when you hoard
    - Trim down on rules and processes and turf guarding
2.Institutionalize improvement of daily work
    - Invest time in paying techincal debt, and refactoring
    - Engage in `kaizen blitzes`, which are periods of time to allow the engineers to fix any problems they want (Different from working on what they want)
3. Transform local discoveries to global discoveries
    - Convert tacit knowledge into explicit codified knowledge
    - Shared source code bases, libraries and tools help enable this
4. Inject Resilience patterns into daily work
    - Deliberately induce stress to the workflow to see how thing organically adapt to improve
5.  Leaders to reinforce a learning culture
    - ***Leaders are not great for making right decision, but rather, by creating conditions in which the team can discover greatness***
    - A mutual relationship is required because Leaders are not close enough to the work, and workers dont have the context
    - Establish a True North strategic goals, which in turn will create shorter term goals to meet them

## Getting Started

1. Selecting which value streams to start with
     - Select important projects to transform. Dont try to transform all at once
     - Demonstate early and small wins to gain confidence
     - ***Stop throwing bodies, but improve the way you work***
     - Greenfield vs Brownfield services: New projects vs Exisiting projects
     - Brownfield projects are usually harder due to the number of technical debts
     - ***Try to add in the DevOps cycle while its still Greenfield, and not wait till its Brownfield***
     - Systems of Record vs Systems of Engagment: Storage systems (Backend) or Interactive systems (Frontend)
     - Start with Early Adopters, Win the Silent Majority, Idenity Holdouts (Resistance)
3. Undestanding work done
    - Once the value stream has been identified, identify the teams involved
        - Product owner
        - Developers
        - QA
        - Operations
        - Infosec
        - Release Managers
        - Executives
    - Create a value stream map to make visible all the work required
        - Identify places where work must wait
        - Identify places where significant rework is generated or received
    - Create a dedicated Transformation Team
        - This team is operational outsides of the rest of the organization
        - Select generalist people to this team
        - Select respectful people to this team
        - Create a separate physical space for this team
    - Keep the improvement planning horizon short
        - Dont set long and far reaching improvement goals, but short and achievable in the near term ones
    - ***Keep 20% of DevOps time for clearing technical debt***
    - Increase visibility of work
    - Use tools to reinforce desired behavior
5. Designing organization and architecture with Conways Law in mind
    - Conways Law: The organization of a software and the organization of the software teams will be congruent
    - A team of 4 separate groups will build a software with 4 separate functionalities
    - ***To keep Conway's Law in mind, we should structure the output first, before structuring the team***
6. Organizational Archetypes
    - Functional Oriented: Group According to expertise
        - Functional groups tend to have longer lead times due to the coordination between of different groups
        - Working in such silos prevents the person from seeing the bigger picture
        - Quality of work from handoffs also suffers
        - Functional Oriented Organizations optimize for Costs
    - Matrix Oriented: Functional + Market Oriented. Can get Complex.
    - Market Oriented: Flat structure. Each cross functional team addresses a feature or service
        - Cross functional independent teams that service their own demands
        - Embed the functional engineers into each service team
        - Market Oriented Organizations optimize for speed
8. Testing, Operations and Security is the job of everyone, not only a single department
    - Rotation of job scopes to gain exposure ensures everyone knows how to perform other duties
10. Protecting and enabling our teams
    - When a department overspecializes, it creates a silo
    - Any handoffs between them becomes long and of poor quality
    - To prevent this, we encourage all engineers to be generalist, through regular role rotations
    - I-shaped, T-shaped and E-shaped engineers
11. Don't Fund Projects, Fund Services and Products
    - Services and Products can be used in multiple projects, whereas a project has an EOL
12. ***Created Loosely-Coupled Architectures***
    - Enable small teams to be independently productive and decoupled
    - Services must be independent as well (Microservices)
13. Keep Team Sizes Small
    - Two pizza team rule (5-10 people)
    - Ensures that the team is clear about the system they are working on
    - Limits the growth rate of the system, which allows developers to control it
    - Decentralized power across the teams
    - Allows team members to step up to leadership roles
14. Integrate Ops into Devs
    - This ensures that the Devs are kept in check to produce code that can be operationalized
    - Create self-service Ops tools so that the Dev can use them
    - This also allows products created by Dev to be streamlined for Ops, increasing speed of delivery
    - By created such shared services and common tools, Developers can quickly jump between teams without relearning much
    - Gives Ops visibility of Devs workflow, vice-versa. This allows both parties to adapt their work to any changes

## Technical Details of the First Way

Implementations from Dev to Ops

1. Creating a foundational pipeline
    - Ensure that production-like environments are used at every stage of the value stream
        - This ensures that each step would be streamlined into Ops
        - This creation must be automated and version controlled
    - Creating a single source of truth for the repositories
        - e.g. git for version control
        - Code, Configuration, Documentation, Artifacts, Scripts, Schemas etc
    - Make infrastructure easy to rebuild
        - Don't fix or repair, simply rebuild
        - Environments and infrastructure must be easy to spin up or down
    - ***Redefine work that is "DONE", to only when the code can be productionized, not ran locally***
2. Enable Fast and Reliable Automated Testing
    - 
   

