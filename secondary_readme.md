Mostly so I don't forget what caused all the delays this time like I forgot the first time.

In order to take an edited helm chart from the apps/stable/* location I absolutely have to use the .devcontainer docker container in some way.

I've found the easiest (although still painful) is with visual studio code, however I can't get it to wrok on an M1 mac so must be ran on a windows/linux machine


once done use possibly two scripts

I'm certain you have to at least run .github/scripts/build-catalog.sh in order to create the numerical versions and builds within the catalog/stable/* directory

but I also ran the ./tools/build-release.sh multiple times before eventually running the catalog one. unsure of importance for the build-release but might as well document this to save time in the future when I forget again




