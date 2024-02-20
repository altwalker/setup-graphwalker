# setup-graphwalker

Set up your GitHub Actions workflow with a specific version of [GraphWalker](https://graphwalker.github.io/) CLI.

This action provides the following functionality for GitHub Actions users:

* Installing a version of Python or PyPy
* Installing a version of Java
* Installing a version of GraphWalker CLI and (by default) adding it to the `PATH`

## Usage

```yml
steps:
  - name: Setup GraphWalker
    uses: altwalker/setup-graphwalker@v1
    with:
      graphwalker-version: '4.3.1'
  - name: Run GraphWalker
    run: |
      gw --version
```

The `graphwalker-version` input is optional. If the `graphwalker-version` option does't exist the last released version of GraphWalker will be installed.

If you want to install the most up to date version of GraphWaker from the `master` brach set `graphwalker-version` to `latest`.

See [action.yml](action.yml) for more details.

### Community

For help, discussion about best practices, sharing ideas, projects, or any other conversation that benefits from being searchable:

* [Discuss AltWalker on GitHub](https://github.com/orgs/altwalker/discussions)
* [Google Group](https://groups.google.com/g/altwalker)

For casual chit-chat with us or with other members of the community: 

* [Gitter Chat Room](https://groups.google.com/g/altwalker)

## License

This project is licensed under the [MIT License](LICENSE).
