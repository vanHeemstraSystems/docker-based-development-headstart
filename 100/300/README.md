# 300 - Acceptable trade-offs for most projects

There are some minor drawbacks with container-based development, although they are highly acceptable trade-offs given the benefits for most projects:

1. Although it’s fairly easy to set it up, adopting container based development still requires some initial additional investment.
However, the investment has more than proportional returns, as the complexity and collaborators of the project grow.

2. After the initial setup, it requires collaborators to learn and understand the very basics of containers that they run on the local machine but are isolated environments.
The extra time to learn and understand containers in many casse is even less than to manually set up the development environment though.

3. It takes some additional disk space. As each container is an isolated environment, each of them takes additional space.
We could delete old containers and images from the local machine when not using them though.

4. It takes additional time to start the container every time you start the computer.
