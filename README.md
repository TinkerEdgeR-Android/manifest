# manifest

Please refer to the following URL to install Docker.

    https://docs.docker.com/engine/install/ubuntu/

Please refer to the following URL to install Repo. 

    https://source.android.com/setup/develop#installing-repo

Please refer to the following URL to understand how to download the AOSP code.

    https://source.android.com/setup/build/downloading

Then, you can issue the following command to donwload the source for Tinker Edge R Android.

    $ repo init -u https://github.com/TinkerEdgeR-Android/manifest.git -b p-rk3399pro
    $ repo sync

Go to to the directory where you have downloaded the souce and execute the script as the following. This will take a while to install the necessary packages on the host, build the Docker image, and start the container:

    $ ./docker-builder/docker-builder-run.sh

Once it is done. You are in the shell of this newly started Docker container and you can execute the following script to build the Tinker Edge R Android image.

    $ ./build.sh

And the image will be stored as the following in the directory where you have downloaded the souce

    ./IMAGE/Tinker_Edge_R-Android9-eng-username-YYYMMDD.HHMM/IMAGES/update.img
