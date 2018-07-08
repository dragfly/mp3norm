# mp3norm
A simple mp3 normalization Docker Image

# Motivation
I needed a simple and quick tool to normalize mp3 files, so I created this bare bones image to process all files in a directory using mp3gain (thanks to [Martin Wimpress](https://launchpad.net/~flexiondotorg/+archive/ubuntu/audio) for his PPA)

# Usage
To normalize files in the current folder just use $PWD (macOS or Linux) or %CD% (Windows)

Usage:

Linux
```
docker run --rm -v $PWD:/files dragfly/mp3normalizer
```

Windows
```
docker run --rm -v %CD%:/files dragfly/mp3normalizer
```