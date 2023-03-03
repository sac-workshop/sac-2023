# SAC 2023 website source

This is the source code for the website for the Selected Areas in Cryptography (SAC) 2023 conference.  The website is built using the [Jekyll](https://jekyllrb.com/) framework and at the moment is deployed on Github Pages at [https://sac-workshop.github.io/sac-2023/](https://sac-workshop.github.io/sac-2023/).

Most of the website will be auto-generated from data files in the YAML formal, under the `_data` directory.

## Getting started

For the initial launch of the website, you will want to edit the following files:

- `_config.yml`
- `_data/variables.yml`
- `_data/dates.yml`
- `_data/organizers.yml`
- `_data/programcommittee.yml`

As planning progresses, you will need to edit the following files.  (Note that until you have updated the files below, you should hide them from being displayed by editing the relevant variables in `_data/variables.yml`.)

- `_data/sponsors.yml`
- `_data/schedule.yml`
- `_data/speakers.yml`
- `registration.md`
- `summer-school.md`
- `travel.md`

## Deploying

Once you push to the `main` branch on Github, the page will automatically be deployed on Github Pages at [https://sac-workshop.github.io/sac-2023/](https://sac-workshop.github.io/sac-2023/).  Note that it may take a few minutes for the updated site to get built; check the status at [https://github.com/sac-workshop/sac-2023/actions](https://github.com/sac-workshop/sac-2023/actions).

## Building locally

You can build and test the website on your local computer.  You need to have Ruby and [Jekyll](https://jekyllrb.com/) installed.  

Installing Ruby can be tricky (especially on macOS), so here are some instructions to use Docker which might be simpler.  Run the following commands from within the checked out repository:

```bash
docker pull jekyll/jekyll
docker run --rm --volume="$PWD:/srv/jekyll:Z" \
       --publish 4000:4000 --publish 35729:35729 \
       jekyll/jekyll \
       jekyll serve --livereload
```

Then open your web browser and visit [http://0.0.0.0:4000](http://0.0.0.0:4000).  If everything is set up correctly, the local server will automatically update whenever you save a changed file.
