# Primitives::files_existence version 1.0

License: MIT
Tags: cfdc, primitive, files, present, absent, existence, enterprise_compatible, enterprise_3_6
Authors: Nick Anderson <nick@cmdln.org>

## Description
This sketch provides facilities ensuring a list of files exists or not. It can also be used strictly for validating the presence of a file which may be useful for host classification.

## Dependencies
CFEngine::sketch_template

## API
### bundle: absent (description: Ensure all given files are absent.)
* parameter _environment_ *runenv* (default: none, description: none)

* parameter _metadata_ *metadata* (default: none, description: none)

* parameter _list_ *list_of_files* (default: none, description: List of files to ensure are absent.)

* parameter _string_ *success_class* (default: none, description: Class to define if all files are absent.)

* parameter _string_ *fail_class* (default: none, description: Class to define if any file is present and can not be deleted.)

### bundle: present (description: Ensure all given files are present.)
* parameter _environment_ *runenv* (default: none, description: none)

* parameter _metadata_ *metadata* (default: none, description: none)

* parameter _list_ *list_of_files* (default: none, description: List of files to ensure are absent.)

* parameter _string_ *success_class* (default: none, description: Class to define if all files are present.)

* parameter _string_ *fail_class* (default: none, description: Class to define if any file is absent and can not be created.)


## SAMPLE USAGE
See `test.cf` or the example parameters provided

