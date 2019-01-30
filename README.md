# edx_course_templater

Ok, so here's the plan:

* Make a survey using an HTML form.
* Have people fill it out to describe the kind of course they want to make.
* Use javascript to get the detail from it and construct the desired course.
    * Slap the boilerplate course in there too while we're at it.
    * And pre-set the gating workaround.
* Tar up the final file so they can download it. (Turns out no need to gzip.)
* Do this all client-side so we don't need to run a secure server.
* Run this out of GitHub Pages, maybe get a custom URL to point at it.

Currently using [TarballJS](https://github.com/ankitrohatgi/tarballjs), a snapshot of which is included in this repo.

Originally I was going to use a JSON file to keep track of the boilerplate course, but honestly it's overkill. Using `find path/to/folder -type f > course_structure.txt` makes a flat file that will work just fine.
