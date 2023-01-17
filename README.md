# watchep.org Website

This is the repository for the WATCHEP public website using GitHub pages.

WATCHEP is the Western Advanced Training for Computational High-Energy Physics.

## Using Jekyll for building web pages

We are using [Jekyll](https://jekyllrb.com) to build the site. The easiest way to run Jekyll is to use the Docker container:

> docker run --rm -it 
      --volume="$PWD:/srv/jekyll" -p 4000:4000 
      jekyll/builder:stable bash
      
Then from that Docker container shell:
> bash-5.1# jekyll serve --watch

This will cause Jekyll to rebuild the site automatically when you change input files. 
You can view your changes locally at [http://0.0.0.0:4000](http://0.0.0.0:4000).