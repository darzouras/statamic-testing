# Statamic POC and Experiments

This repository is the outcome of my attempt to build a website using [Statamic](https://statamic.com). This README is a collection of notes for quick reference in future Statamic projects.

## Getting Started
Getting the environment set up so far has been the trickiest part of this:

Important links:
- [Statamic installation docs](https://docs.statamic.com/installing)
- Mac only, my preferred method of serving: [Laravel Valet](https://laravel.com/docs/5.7/valet)
- Definitely need if using Laravel Valet: [Composer](https://getcomposer.org/)

Note: I was unable to get the Statamic demo working with PHP 7.3 installed due to a bug (I forgot the name). PHP 7.1 seems to be running smoothly, so when going through the Laravel Valet install process I install PHP 7.1 specifically with `brew install php@7.1`

*Apparently an update to support PHP7.3 came out a day after I attempted my first download- PHP versioning should be much less of a big deal now.*

## Quick Reference

- `php please make:theme NAME-OF-THEME` creates a basic new theme. npm install inside that theme folder to use `gulp` capabilities to compile scss files. Statamic recommends keeping theme names all lowercase.
- The **layout** wraps around the **template**. If a template is not defined it will use `default.html`.
- The folders and files in the `site/content/pages` folder creates the page structure of the site.
