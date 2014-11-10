Libraries required to build PandoraAgent for Windows
====================================================

A collection of libraries required to build PandoraAgent for Windows.
When git tag has pushed travis-ci deploy the libraries to release page

when you want to build ${version} for ${required_library}

```
$ cd ${required_library}
$ git checkout ${version}
$ cd ..
$ git commit ${required_library}
$ git push origin master
```

When Travis-CI pass build, push tags

```
$ git tag ${release_tag}
$ git push --tags origin master
```

After this push, Travis deploy the library to release page.

