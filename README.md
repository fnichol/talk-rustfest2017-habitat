# Taking Rust To Production: Lessons Learned From The Habitat Project

## RustFest 2017 Talk by Fletcher Nichol

|                         |                              |
|-------------------------|------------------------------|
| Event                   | [RustFest 2017](http://2017.rustfest.eu/) |
| Presentation Recording  | https://youtu.be/zAXbPnfTJg4 |
| Online Slides           | https://fnichol.github.io/talk-rustfest2017-habitat/ |
| PDF Slides              | https://speakerdeck.com/fnichol/rustfest-2017-taking-rust-to-production-lessons-learned-from-the-habitat-project |

## Abstract

The Rust language is more than ready for production–it excels at it! The [Habitat](https://www.habitat.sh/) project team has been using Rust for a year in public and an extra year in stealth. With over 40,000 lines of Rust code so far, we maintain multiple CLI applications, a cross-platform process supervisor, a gossip subsystem, and a micro service-oriented distributed build system.

In this talk we will cover some of the challenges that Rust is uniquely qualified to address including static compilation, inlining dependencies, using clap for CLI parsing, pragmatically using native C libraries, maintaining a common codebase for Linux, Mac, and Windows, and on-boarding new Rustaceans. Have no fear: there has never been a better time to use Rust for your next service, application, or tool!

## Development

### Running Local Presentation

```sh
# Install dependencies
npm install

# Start local server
npm start
```

### Exporting PDF Slides

```sh
# Determine your workstation's IP address
ip_addr=10.0.0.15

# Export using Docker
docker run --rm --net=host -v $(pwd):/slides astefanutti/decktape http://${ip_addr}:8000 slides.pdf
```
