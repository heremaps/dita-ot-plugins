# DITA Open Toolkit Plug-ins

This repository serves to organize a set of DITA OT plug-ins developed internally at [HERE](https://company.here.com/here/)
into a single project, where each plugin is a separate git submodule.
This makes it easier to work with the plug-in projects as a unit.

* `com.here.validate.svrl` - a structure, style and content checker plug-in for DITA documents.
* `com.here.validate.svrl.overrides` -  a demonstration plug-in module showing how to add, remove or extend the ruleset of the base [DITA Validator](https://github.com/heremaps/com.here.validate.svrl)
* `com.here.validate.svrl.text-rules` - a text-rules plug-in is an extension of the base [DITA Validator](https://github.com/heremaps/com.here.validate.svrl) which adds simple rule-based spelling and grammar validation for the text elements within DITA documents.


If you clone or fork this repository, you must then initialize the
contained submodules in order to get the source for each plug-in, using the `git submodule init` and `git submodule update` commands in the `dita-ot-plugins` directory, e.g.:

```bash
# "cd" to the path you wish to clone this repository into
cd ~/PATH_TO_CLONE_INTO
cd clone https://github.com/heremaps/dita-ot-plugins.git
cd dita-ot-plugins
git submodule init
git submodule update
git submodule foreach git checkout master
```

After running these commands, you should have an up-to-date repo for each plug-in, checked out to the `master` branch.

If any plug-in is updated, you can update your local repo using the command:

```bash
git submodule foreach git pull
```

## Licensing
All plug-ins are released under the `MIT License`.  
Please inspect each plug-in directory for the appropriate `LICENSE` file.

## Other Sources of Plug-ins

* The DITA Open Toolkit is available at [http://www.dita-ot.org](http://www.dita-ot.org).
* The DITA Community Open Toolkit Plug-ins are available at [https://github.com/dita-community/dita-community-ot-plugins](https://github.com/dita-community/dita-community-ot-plugins)
* DITA for Publishers ([http://dita4publishers.sourceforge.net](http://dita4publishers.sourceforge.net)) provides a number of plug-ins, including EPUB, HTML5, and enhanced HTML output. It also provides a general map-driven framework that can be used by other plug-ins.
* The [DITA Users Yahoo Group](https://groups.yahoo.com/neo/groups/dita-users/info) has a files area that includes community-contributed plug-ins.

## Other Links

Please visit our GitHub page at [https://github.com/heremaps](https://github.com/heremaps)
