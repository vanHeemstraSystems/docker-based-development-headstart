# 200 - Easy setup and huge benefits

With just two easy docker commands (build and run), not only could we create an image and start a container with a specific operating system, but also automatically install all the dependencies the project needs. This has the following benefits:

1. We could have the exact same development runtime as the production, regardless which operating system or distribution of the local machine that the developers are running the docker container from. This prevents potential problems from unexpected behaviors due to different operating systems.

2. Installations of all project dependencies like C++ shared libraries, Java and Python runtime and packages, and any executables are all automatically managed. Project setup becomes really easy for developers and eliminates human mistakes. This means for Python projects, we no longer need any additional virtualenv or Conda setup that complicates development with activations and switching.

3. With the project running on its own isolated container, potential conflicts between different projects and the operating system are both prevented.

4. Container-based development would also eliminate another common problem that developers face with the system path and environment variables. Both would be configured as part of the image, consistent and isolated from other projects and the local operating system.

5. It fixes one of the worst developer’s nightmares, that some changes accidentally broke the development environment. With a container, we could just delete the broken container and create a new one from the image, perfectly working and exactly the same as it was before being broken.

6. Lastly, all major cloud providers (AWS, Azure, GCP) and compute management systems (Kubernetes) support deploying applications with docker images. This means many projects already have a docker image and it is really easy to create a container from the image and connect to it for local development.

Developing locally through a container has many benefits that save the team tons of work around project environment setup and maintenance. It pays back even more when developers sometimes have to work on multiple projects.
