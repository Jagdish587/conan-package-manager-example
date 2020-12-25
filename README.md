# conan-package-manager-example


#Format

[requires]

# You may have multiple lines like the one below, if you have many dependencies.

$library/$version@$owner/$branch

[generators]

cmake

# find variants of sqlite db
$ conan search sqlite3* --remote=conan-center

# Steps 
$ mkdir build

$ cd build

$ conan install ..

#Generate dependecy of your project
$ conan info ..-- graph=graph.html
