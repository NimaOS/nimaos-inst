<div align="center">
    <h1>nimaos-inst</h1>
</div>

<div align="center">
    <p>An installer framework and drop-in replacement for and rewrite of Jade in Python that uses the live session's file system instead of bootstrapping a new one</p>
</div>

## Testing

```sh
# 1. Clone this repository

git clone 'https://github.com/NimaOS/nimaos-inst.git'

# 2. Run the installer with the sample configuration in testing mode,
#    which will simply print out the commands that will run in a true
#    installation, instead of actually running them.

TESTING_INST=true ./nimaos-inst config 'sample-config.json'
```

## For distributors

### UI

Jade-GUI, developed by Crystal Linux, can be used with nimaos-inst.

### Error codes:

* `1` - Partitioning error
* `3` - Username not allowed

## Contributing

Anyone is free to contribute to nimaos-inst! It's licensed under the GPL-3.0 license. You can create a PR from the 'Pull Requests' tab on GitHub. You're requested to use `autopep8` to format your Python code before creating a pull request.

## Credits

nimaos-inst has been made by Nima Fanniasl.
The base project, blend-inst has been written by Rudra Saraswat. However, the code is inspired by Jade (written in Rust), since it's meant to be a drop-in replacement for Jade. Jade is a project developed by **Crystal Linux**.
