# docker-python-ta-lib

[travis-badge]: https://img.shields.io/travis/9fevrier/docker-python-ta-lib/master.svg?label=TravisCI
[travis-badge-url]: https://travis-ci.org/9fevrier/docker-python-ta-lib

A Dockerfile to build an image including Python TA-Lib wrapper and dependencies.

[![TravisCI Build Status][travis-badge]][travis-badge-url]

## Table of Contents

* [Synopsis](#synopsis)
* [Usage](#usage)
* [Installation](#installation)
* [Build](#build)
* [Tests](#tests)
* [Compatibility](#compatibility)
* [Issues](#issues)
* [Contributing](#contributing)
* [Credits](#credits)
* [History](#history)
* [License](#license)

## <a name="synopsis"> Synopsis

A Dockerfile to build an image including Python TA-Lib wrapper and dependencies.

## <a name="usage"> Usage

```bash
docker run -it 9fevrier/python-ta-lib
```

## <a name="installation"> Installation

```bash
docker pull 9fevrier/python-ta-lib
```

## <a name="build"> Build

```bash
docker build -t 9fevrier/python-ta-lib .
```

## <a name="tests"> Tests

This command does not return error:

```bash
docker run --name python-ta-lib -t 9fevrier/travis-python-ta-lib python3 -c 'import talib'
```


## <a name="compatibility"> Compatibility

* [Docker CE](https://docs.docker.com/release-notes/docker-ce/) >= 18.03.1-ce

## <a name="issues"> Issues

Feel free to [submit issues](https://github.com/9fevrier/docker-python-ta-lib/issues) and enhancement requests.

## <a name="contributing"> Contributing

Please refer to project's style guidelines and guidelines for submitting patches and additions. In general, we follow the "fork-and-pull" Git workflow.

 1. **Fork** the repo on GitHub
 2. **Clone** the project to your own machine
 3. **Commit** changes to your own branch
 4. **Push** your work back up to your fork
 5. Submit a **Pull request** so that we can review your changes

**NOTE**: Be sure to merge the latest from "upstream" before making a pull request!

## <a name="credits"> Credits

### Thanks to the developers...

* [TA-Lib](https://sourceforge.net/projects/ta-lib/files/ta-lib/)
* [John Benediktsson](https://github.com/mrjbq7) for his great development of a [Python wrapper](https://github.com/mrjbq7/ta-lib). [TA-Lib](https://sourceforge.net/projects/ta-lib/files/ta-lib/).
* [Domenico Silletti](https://github.com/dsilletti) for his [comment](https://github.com/mrjbq7/ta-lib/issues/157#issuecomment-367329661) to fix bug about small numbers.

## <a name="history"> History

Please refer to [the changelog file](CHANGELOG.md).

## <a name="license"> License

>
> [The MIT License](https://opensource.org/licenses/MIT)
>
> Copyright (c) 2018 [SAS 9 Février](https://9fevrier.com/)
>
> Permission is hereby granted, free of charge, to any person obtaining a copy
> of this software and associated documentation files (the "Software"), to deal
> in the Software without restriction, including without limitation the rights
> to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
> copies of the Software, and to permit persons to whom the Software is
> furnished to do so, subject to the following conditions:
>
> The above copyright notice and this permission notice shall be included in all
> copies or substantial portions of the Software.
>
> THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
> IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
> FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
>AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
> LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
> OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
> SOFTWARE.
>
