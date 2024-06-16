FROM ubuntu:22.04

WORKDIR /mydir

RUN apt-get update && apt-get install -y curl python3
RUN curl -L https://github.com/yt-dlp/yt-dlp/releases/latest/download/yt-dlp -o /usr/local/bin/yt-dlp
RUN chmod a+x /usr/local/bin/yt-dlp

# CMD ["/usr/local/bin/yt-dlp"]
# Replacing CMD with ENTRYPOINT
ENTRYPOINT ["/usr/local/bin/yt-dlp"]

# define a default argument
CMD ["https://www.youtube.com/watch?v=Aa55RKWZxxI"]


# make sure you have ubuntu image
# docker pull ubuntu:22.04

# build the image
# docker build -t yt-dlp .

# run the container overriding the default argument
# docker run -v "$(pwd):/mydir" yt-dlp <YOUTUBE_URL>