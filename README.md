# bme-githooks
This is a helper repository for [Bash Magic Enviro](https://github.com/jmnavarrol/bash-magic-enviro) to showcase its [client-side git hooks](https://git-scm.com/book/en/v2/Customizing-Git-Git-Hooks) support.

A common problem with client-side git hooks is how sharing them within a development team as by default they are *"hidden"* under the non-git-tracked *.git/hooks/* directory. Some solutions include documenting a process, adding a manually triggered script, etc.

Fortunately, starting version **2.9**, git offers a means to configure an alternate directory for these hooks by means of its **core.hooksPath** property.

[BME's **githooks** module](https://github.com/jmnavarrol/bash-magic-enviro#githooks) uses this property to set the hooks path to the [*'githooks/'* directory on the repository](./githooks/).  [This way](./.bme_project), upon first clone of this repository, client-side git hooks will be automatically enabled.

A very minimal pre-commit hook [has been added to this repository](./githooks/pre-commit) to showcase this feature.

----

### License<a name="license"></a>
This repository is made available under the terms of the **[GPLv3](https://www.gnu.org/licenses/gpl-3.0.html)**.

See the [license file](./LICENSE) that accompanies this distribution for the full text of the license.
