# DRM Activator documentation

This project is the documentation source for Sphinx online documentation (https://drm-activator-documentation.readthedocs.io/en/latest/) of the DRM Activator IP.

When there is a push on this git repository, a build is automatically done on https://readthedocs.org/projects/drm-activator-documentation/builds/. If the build is "passed", a new version of "latest" version of documentation is automatically available online: https://drm-activator-documentation.readthedocs.io/en/latest/.

To be sure to be notified by any change on Algodone repository, apply email notifications when there is activity on the root documentation done on Algodone git: https://externalgit.plda.com/profile/notifications and set to "watch" for Algodone. It's allow to know when a documentation is necessary


## How to update documentation

The root documentation is coming from Algodone git repository: https://externalgit.plda.com/Algodone/IP-Activator. Documentation is present on: https://externalgit.plda.com/Algodone/IP-Activator/blob/BRANCH/docs/DOCUMENTATION.md and https://externalgit.plda.com/Algodone/IP-Activator/blob/BRANCH/docs/RELEASE_NOTES.md .

When there is update of the DRM Activator repository (https://externalgit.plda.com/Algodone/IP-Activator), we need to apply this modification on this current repository:
   - Use comparison between 2 commits: https://externalgit.plda.com/Algodone/IP-Activator/compare
   - Get the 2 hash commits: https://externalgit.plda.com/Algodone/IP-Activator/activity
   - Apply difference on https://github.com/xlz-jeydoux/DRM-Activator-documentation/tree/master/docs corresponding rst file(s) and images.


## How to write documentation in restructured text (.rst) format

To know how to witre documentation on restructured text (.rst) format, also, DRM integration documentation is a good reference project to see the differents aspects of the rst syntax: https://github.com/xlz-jeydoux/DRM-integration-documentation/blob/master/docs/index.rst.

Online rst preview and syntax verification: http://rst.ninjs.org/# 


rst syntax: http://openalea.gforge.inria.fr/doc/openalea/doc/_build/html/source/sphinx/rest_syntax.html

## Documentation version management

When you create a tag on this git repository to release a new documentation version, this new version must be activated on  https://readthedocs.org/projects/drm-activator-documentation/versions:
   - Check: https://readthedocs.org/projects/drm-activator-documentation/versions/ that the new tag version exist.
   - You can now set the version "active":
      - click on "edit"
      - click on "Active"
Now the version is available online with link: https://readthedocs.org/dashboard/drm-activator-documentation/version/vX.Y.Z/





