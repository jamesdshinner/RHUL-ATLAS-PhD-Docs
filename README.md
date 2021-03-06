# RHUL-ATLAS-PhD-Docs
A repository to hold documentation of software tutorials for new PhD students in the RHUL ATLAS group.

## Dependencies

This project is built with the Python package `mkdocs`, which can be installed using the following command:

```
pip install mkdocs
```

## Adding Tutorials

To add tutorials to the repository, start by forking the repository. 

You can then add a markdown file containing your tutorial to the `docs/` directory. 

To make it accessible from the navigation menu, you need to add a line in `mkdocs.yml`, as follows:

```
nav:
	...
	...
	- <Tutorial name>: <Tutorial markdown file>
```

With these two steps complete, submit a pull request to get your changes approved and integrated into the main repository.

If you want to test your changes locally, you can run `mkdocs serve` from the folder containing the `mkdocs.yml` file to deploy a version of the project site to http://127.0.0.1:8000/

## Github Pages Integration

The project site is hosted live using Github pages at https://rhulpp.github.io/RHUL-ATLAS-PhD-Docs

To update the live version, checkout the master branch of the main repo, and then run the command `mkdocs gh-deploy`