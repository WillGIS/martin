# Martin

[![Build Status](https://travis-ci.org/urbica/martin.svg?branch=master)](https://travis-ci.org/urbica/martin)

PostGIS [Mapbox Vector Tiles](https://github.com/mapbox/vector-tile-spec) server.

**Warning: this is experimental**

## Installation

    git clone git@github.com:urbica/martin.git
    cd martin
    cargo build --release
    ./target/release/martin

## Usage

    DATABASE_URL=postgres://postgres:password@localhost:5432/test martin

## Using with Docker

    docker run -d —rm —name martin \
      -p 3000:3000 \
      -e DATABASE_URL=postgres://postgres:password@localhost:5432/test \
      urbica/martin

## Development

Install project dependencies and check that the tests run

    cargo test
    cargo run