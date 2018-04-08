# The Field Guide to Security Training in the Newsroom

The Field Guide to Security Training in the Newsroom is a round up of resources and lesson plans designed to improve and expand newsroom digital privacy training. 

This curriculum is hosted by [OpenNews](https://opennews.org/), a team that helps developers, designers, and data analysts convene and collaborate on open journalism projects. The first draft was composed during a two-day convening in Chicago in June 2017. The curriculum launched publicly in the Spring of 2018.

This is a living resource and we welcome your [contributions](docs/contributing.md) and [feedback](https://github.com/OpenNewsLabs/field-guide-security-training-newsroom/issues).

Our goal is not to replicate good work that other organizations have already done, so if you know about great training resources for security trainers, we'd love to add those to our [resource roundup](https://the-field-guide-to-security-training-in-the-newsroom.readthedocs.io/en/latest/Chapter03-01-Resources.html).

## More ways to contribute

* **Real-life feedback.** If you use these lesson plans or other materials in your training sessions, we'd love to hear about it! We're particularly interested in the results of workshops and sessions using the pathways suggested in Chapter 1.

* **New lessons, and lesson ideas.** As new tools are developed and new threats emerge, we plan to add lesson plans to cover them. [Let us know](mailto:fieldguide@opennews.org) what topics you're most interested in seeing covered, or share an agenda from a workshop you've used with your peers.

* **Resource links and glossary items.** Chapter 3 includes a glossary and links to existing security resources, to complement and extend the topics covered in our lesson plans. If your favourite links are missing, we'd love to add them!
If you're comfortable with GitHub, we welcome [Pull Requests](https://github.com/OpenNewsLabs/field-guide-security-training-newsroom/pulls) and [new Issues](https://github.com/OpenNewsLabs/field-guide-security-training-newsroom/issues/new), or you can also [drop us an email anytime](mailto:fieldguide@opennews.org).

* **Translation and localization.** The initial version of the guide was written with North American English-speaking newsrooms in mind, but digital security is important for journalists working in all communities and languages. If you can provide translations of the existing guide resources, or if you'd like to add lesson plans covering topics more relevant to your community, please contact us. 

* **Pick up an existing need:** Our [GitHub Issues list](https://github.com/OpenNewsLabs/field-guide-security-training-newsroom/issues) captures specific tasks that need to be addressed. If you're looking for a way to contribute, grab a ticket!
* **Tell us about your experience:** Have you used *The Field Guide to Security Training in the Newsroom* to lead a workshop in your newsroom? [We'd love to hear about it](mailto:fieldguide@opennews.org). We're also looking for newsrooms that want to work closely with us to lead trainings and edit the guide in the process. Email us if this sounds like you.

## Building the Guide

The field guide is published on ReadTheDocs using Sphinx, a Python-based documentation system. If you have changes to share and want to preview them before sending us a pull request, here's how to build the guide locally. (Note that these instructions assume a Unix-like environment. If you're using OS X or Linux, you should be good to go. Windows 10 users should consider enabling the Windows Subsystem for Linux - users of earlier Windows versions should look into [Cygwin](https://www.cygwin.com/).) 

1. If they're not already available, install Python 2 and pip. For more information, see the [Python Beginners Guide](https://wiki.python.org/moin/BeginnersGuide/Download).
2. From the command line, use pip to install the necessary modules:
```bash
pip install recommonmark
pip install sphinx sphinx-autobuild sphinx_rtd_theme
```
(If you encounter permission errors, you may need to run the commands with a `sudo` at the beginning, eg. `sudo pip install recommonmark`.)
