
New assumption after succesfully building the adjusted chart on my m1 laptop multiple times. Well succesfully insofar as to not have it be labeled "unhealthy" within the Truenas Scale UI as a catalog
but still unable to perform the ffmpeg edit I was attempting.

run `tools/build-release.sh -s` while running the truecharts devcontainer in VS code from the workspaces/apps directory


.devcontainer
        from within the apps directory is important. Have visual studio code build the container using it

        the green "Container" label at the bottom left of visual studio code MUST include some variation of */truecharts/*
            it very specifically cannot just read as Ruby container otherwise the build script will fail

        whoami does not appear to be important, I was root within the container and able to have it build

directory
        had to call the script from /workspaces/apps which essentially is the base directory for the github repo of frap/apps

script
                             **    `tools/build-release.sh -s`       **

                             above is the exact command to build the catalog while within the container

                             -s appears to be standalone that doesn't link to the main gh repo which is exactly what I want for private development, it also says that form the -h command of the build-release.sh

        I called the script from within the terminal of the visual studio code
                it was labeled as qemu-x86

        it took a long time to run the first time, and longish times after that but not as bad.
        i've been unable to get it to build on my windows computer, I don't know why but not important anyway to me











