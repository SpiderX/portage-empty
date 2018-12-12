# portage-empty

[golang-vcs-snapshot](https://devmanual.gentoo.org/eclass-reference/golang-vcs-snapshot.eclass/index.html) provides a convenience src_unpack() which unpacks the
first tarball mentioned in SRC_URI to its appropriate location in
${WORKDIR}/${P}, treating ${WORKDIR}/${P} as a go workspace.

This repository is used to force golang-vcs-shapshot unpacking an empty
repository without doing any harm to others package' sources.

This repository is intended to be used in live golang ebuilds and 
should be specified in the first line of
```sh
EGO_VENDOR=( "github.com/SpiderX/portage-empty {commit}"
....
.... )
```
