# The Field Guide to Security Training in the Newsroom v 1.0.0

The Field Guide to Security Training in the Newsroom is a round up of resources and lesson plans designed to improve and expand newsroom digital privacy training. 

This curriculum is hosted by [OpenNews](https://opennews.org/), a team that helps developers, designers, and data analysts convene and collaborate on open journalism projects. The first draft was composed during a two-day convening in Chicago in June 2017. The curriculum launched publicly in the Spring of 2018.

This is a living resource and we welcome your [contributions](docs/contributing.md) and [feedback](https://github.com/OpenNewsLabs/field-guide-security-training-newsroom/issues).

Our goal is not to replicate good work that other organizations have already done, so if you know about great training resources for security trainers, we'd love to add those to our [resource roundup](https://the-field-guide-to-security-training-in-the-newsroom.readthedocs.io/en/latest/Chapter03-01-Resources.html).

## More ways to contribute

* **Tell us about your experience:** Have you used *The Field Guide to Security Training in the Newsroom* to lead a workshop in your newsroom? [We'd love to hear about it](mailto:fieldguide@opennews.org). We're also looking for newsrooms that want to work closely with us to lead trainings and edit the guide in the process. Email us if this sounds like you.

* **New lessons, and lesson ideas.** As new tools are developed and new threats emerge, we plan to add lesson plans to cover them. [Let us know](mailto:fieldguide@opennews.org) what topics you're most interested in seeing covered, or share an agenda from a workshop you've used with your peers. If you want to get started on a lesson plan right away, your first step should be to create an issue for it! Once that's done, you'll find Markdown and HTML templates in the project's `templates` directory. 

* **Resource links and glossary items.** Chapter 3 includes a glossary and links to existing security resources, to complement and extend the topics covered in our lesson plans. If your favourite links are missing, we'd love to add them!
If you're comfortable with GitHub, we welcome [Pull Requests](https://github.com/OpenNewsLabs/field-guide-security-training-newsroom/pulls) and [new Issues](https://github.com/OpenNewsLabs/field-guide-security-training-newsroom/issues/new), or you can also [drop us an email anytime](mailto:fieldguide@opennews.org).

* **Translation and localization.** The initial version of the guide was written with North American English-speaking newsrooms in mind, but digital security is important for journalists working in all communities and languages. If you can provide translations of the existing guide resources, or if you'd like to add lesson plans covering topics more relevant to your community, please [contact us](mailto:fieldguide@opennews.org). 

* **Pick up an existing need:** Our [GitHub Issues list](https://github.com/OpenNewsLabs/field-guide-security-training-newsroom/issues) captures specific tasks that need to be addressed. If you're looking for a way to contribute, grab a ticket!

## Building the Guide

The field guide is published on ReadTheDocs using Sphinx, a Python-based documentation system. If you have changes to share and want to preview them before sending us a pull request, here's how to build the guide locally. (Note that these instructions assume a Unix-like environment. If you're using OS X or Linux, you should be good to go. Windows 10 users should consider enabling the Windows Subsystem for Linux - users of earlier Windows versions should look into [Cygwin](https://www.cygwin.com/).) 

1. If they're not already available, install Python 2, pip, and virtualenv. For more information, see the [Python Beginners Guide](https://wiki.python.org/moin/BeginnersGuide/Download).
2. From the command line, create and activate a new virtualenv:
```bash
virtualenv field-guide
cd field-guide
source bin/activate
```
4. Fork the project on Github and clone your fork on your local computer, within the virtualenv directory:
```bash 
git clone <your fork here> 
cd field-guide-security-training-newsroom
```
3. From the command line, use pip to install the necessary modules:
```bash
pip install -r requirements.txt 
```
4. From the the project's `docs` subdirectory,
run the command `make html`. This will build the guide in the `docs/_build/html` project subdirectory.

(The `make` utility is installed by default on most unix-like environments. If you see errors like `make: command not found`, you should install the base development tools for your environment, which will include `make`.)

6. Open the file `docs/_build/html/index.html` in your browser to view the local copy of the guide.

7. Run `make html` again after any changes to update your local copy.

