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
$ git push
```

When Travis-CI pass build, push tags

```
$ git tag ${release_tag}
$ git push --tags
```

After this push, Travis-CI deploy the library to release page.

When you fork this repo, you would setup deploy section in .travis.yml
by [travis](https://github.com/travis-ci/travis.rb) command.

Consult [Deployment - Travis CI Documentation](http://docs.travis-ci.com/user/deployment/)
to find information about deployment methods supported by Travis CI.

