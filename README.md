# microbit-docs

## Editing the docs

To edit micro:bit documentation, please edit the raw markdown files contained in the `./docs` folder. Please note that any text placed inside a block like this:

``` 
[comment]: <> ({"className":"MicroBitAccelerometer"}) 

[comment]: <> ({"end":"MicroBitAccelerometer"})
```

Will be deleted and regenerated when `python doc-gen.py` is executed.

We use mkdocs version 0.15.3 to build this site, please use this version only.

mkdocs can be obtained via the [pip](https://pip.readthedocs.io/en/stable/) command.

### Live editing

It is recommended that docs are edited locally using `mkdocs serve` before submitting a pull request with changes.

## Generating API documentation

Text placed in the following markdown comments:

``` 
[comment]: <> ({"className":"MicroBitAccelerometer"}) 

[comment]: <> ({"end":"MicroBitAccelerometer"})
```

Is automatically generated by the `doc-gen.py` script. Any changes made here will not be retained. Changes to API documentation should be made at the source: either [microbit-dal](https://github.com/lancaster-university/microbit-dal) or [microbit](https://github.com/lancaster-university/microbit).

Only maintainers of this repository are allowed to push updates to the live site.

Old versions of the site are contained in the archive folder: 

`./docs/archive`

and can be accessed using the specific version tag:

https://lancaster-university.github.io/microbit-docs/archive/v2.0.0-rc3/
