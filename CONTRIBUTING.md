# Bugs

Before create a new bug, please, first search if the bug already exists to avoid duplication.

Then, remember to add:
- a short but clear title, 
- a good description, including details and steps to reproduce (if applicable),
- your distro name,
- your distro version.

This will speed up the mitigation process.

# Contributing

Contributions are welcomed and appreciated! To start contributing:

1. Fork the repository on GitHub.com
2. Clone your fork
    - `$ git clone git@github.com:your-user-name/scudcloud.git`
    - `$ cd scudcloud`
3. Create a feature branch using the issue number (if exists):
    - `$ git checkout -b 123-named-feature-branch`
4. Backup local scudcloud
    - `$ sudo mv /opt/scudcloud /opt/scudcloud.bak`
    - `$ sudo mv /usr/bin/scudcloud /usr/bin/scudcloud.bak`
5. Install local scudcloud
    - `$ sudo ln -s scudcloud-1.0/lib/*.py /opt/scudcloud/lib`
    - `$ sudo ln -s scudcloud-1.0/resources/* /opt/scudcloud/resources`
    - `$ sudo ln -s scudcloud-1.0/scudcloud $INSTALL`
6. Make your changes
    - `$ git commit -am "implement feature"`
7. Submit a pull request on GitHub.com
    - `$ git push origin named-feature-branch`
8. Edit your pull request description in GitHub.com to include the issue number


In case you need to inspect HTML/CSS/Javascript, start ScudCloud enabling the web console:

    scudcloud --debug=True
    
Then right click in any element, and select `Inspect`. Then at the top, select `Console`.

## ScudCloud.js

Some JavaScript functions are injected in Slack, to enable integration with ScudCloud. Then file is minimized, to allow a better performance.

If you change anything in the JS source files and want to minimize again, minimize with http://jscompress.com/.
