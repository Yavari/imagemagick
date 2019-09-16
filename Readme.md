Build

    docker build . -t imagemagick

Run

    docker run --rm -it --volume path:/test imagemagick /bin/sh
    convert 1.png -fill white -fuzz 40% +opaque "#000000" result.png