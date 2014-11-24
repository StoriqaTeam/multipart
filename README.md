Multipart + Hyper [![Build Status](https://travis-ci.org/cybergeek94/multipart.svg?branch=master)](https://travis-ci.org/cybergeek94/multipart)
=========

An extension to [Hyper][1] that adds support for HTTP multipart (`Content-Type: multipart/form-data`) requests.

See `src/bin/multipart_server.rs` for server-side example (used in testing).

####[Documentation][2]


#####Warning
Using this library with `RUST_LOG=debug` will **flood** your logs due to excess `debug!()` usage during development. This will be fixed in a future update. I suggest you apply more specific log filtering, such as `RUST_LOG=<your crate>=debug`.

#####TODO:  
- [ ] Remove excess debug statements
- [ ] Fill out README and provide examples
- [ ] Improve documentation
- [ ] Add support for multiple files per field (nested boundaries)
- [ ] Expand test coverage
- [ ] Integrate with future HTTP compression extension(s)

[1]: https://github.com/hyperium/hyper
[2]: http://rust-ci.org/cybergeek94/multipart/doc/multipart/
