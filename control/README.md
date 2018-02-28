Control file validation:
------------------------

Run command

    xmllint --noout --relaxng /usr/share/YaST2/control/control.rng *.xml

or simply

    make check


### Notes

The xmllint tool is not reliable much when the validation fails, it can
report incorrect problems in the file and does not provide enough details.

If you need to know *why* the validation failed then use the `jing` tool.

    jing /usr/share/YaST2/control/control.rng *.xml

or

    make check-jing

