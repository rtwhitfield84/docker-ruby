# Ruby

Docker image to build Ruby using ruby-build. Defaults to 2.3.3 using the $RUBY_VERSION env variable.

Installs bundler and common system dependencies for gems.

Use this a base image for Ruby applications.

## Usage

The image builds Ruby using an ONBUILD command so the actual install of Ruby is deferred until you build another image using this image as the base.

### Use this image from Docker Hub

In your Dockerfile reference the prebuilt image as the base

		FROM lookitsatravis/ruby:2.3.3

### To build the image

		$ git clone https://github.com/lookitsatravis/docker-ruby.git
		$ cd docker-ruby
		$ docker build -t ruby:2.3.3 .

## License

MIT

## Copyright

© 2015-2016 Travis Vignon
