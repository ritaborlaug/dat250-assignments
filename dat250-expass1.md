For this assignment I started by just following the steps provided in the task description.
The first thing I did was therefore to create a new repository for the assignment.
Then the task was to set up gradle as the build system, and here I ran into my first problem. I ran the `gradle init`command in the terminal and chose the settings that was written in the task description, but I kept getting an error message saying that the package name was invalid. I had followed the example package name written in the description, and did therefore not understand how this could be an invalid name. After some searching online I found out that the problem was because of my student id number, as you cannot have a number as the leading character after a period.

After fixing this small issue, I could push the files to GitHub.
When I sat up the gradle build system, the project was automatically opened in IntelliJ. I therefore chose to use IntelliJ as my IDE, even though I normally use VSCode, and started to fix the compilation errors. After having added the `package` declaration and the Javalin dependency, I still got an error message saying _Cannot access script base class 'org.gradle.kotlin.dsl.KotlinBuildScript'. Check your module classpath for missing or conflicting dependencies._ Both the **build.gradle.kts** and the **settings.gradle.kts** file gave the same error message, even though I could not seem to find anything that was wrong with the files. I also tried ChatGPT, and tried all the suggestions that got listed up. I checked that the dependencies were compatible, that I used the correct versions of the plugins and I tried to clear caches, all without result. After **a lot** of googling, I finally found a chat forum where several different people had come across the same problem. They all used IntelliJ as IDE, and they wrote that the problem was somehow related to IntelliJ. I therefore changed IDE to VSCode, and then everything worked perfectly fine.

After getting rid of the errors, I added some tests for the App-class and pushed it to GitHub. 

I have no prior experience with containerization, but I followed the example provided for the Dockerfile, which worked well. I created an account on DockerHub and made a new repository that I pushed the image to.
The URL of the image is https://hub.docker.com/layers/ritaborlaug/dat250/latest/images/sha256-88f23bf6c840764871a11183baef9594e1491078e569cd3a4357838075a2a4d4?context=repo
https://hub.docker.com/repository/docker/ritaborlaug/dat250/general 


To check that the software velopment environment is working, I have tried to run the application several times, write tests for the App-class and check that I have used the right versions for the dependencies.