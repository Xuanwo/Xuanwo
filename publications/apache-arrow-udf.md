## Abstract

Arrow UDF is a User-Defined Function Framework for Apache Arrow.

## Proposal

Arrow UDF allows user to easily create and run user-defined functions (UDF) in Rust, Python, Java or JavaScript based on Apache Arrow. The functions can be executed natively, or in WebAssembly, or in a remote server via Arrow Flight.

Arrow UDF was originally designed to be used by the RisingWave project but is now being used by Databend and several database startups.

We believe that the Arrow UDF project will provide diversity value to the entire Arrow community.

## Background 

Arrow UDF is being developed by an open-source community from day one and is owned by RisingWaveLabs. The project has been launched in December 2023.

## Initial Goals

By transferring ownership of the project to the Apache Arrow, Arrow UDF expects to ensure its neutrality and further encourage and facilitate the adoption of Arrow UDF by the community.

## Current Status

Contributors: 5

Users:

-   [RisingWave]: A Distributed SQL Database for Stream Processing.
-   [Databend]: An open-source cloud data warehouse that serves as a cost-effective alternative to Snowflake.



## Documentation

The document of Arrow UDF is hosted at https://docs.rs/arrow-udf/latest/arrow_udf/.

## Initial Source

The project currently holds a GitHub repository and multiple packages:

- https://github.com/risingwavelabs/arrow-udf

Rust:

- https://crates.io/crates/arrow-udf/
- https://crates.io/crates/arrow-udf-python/
- https://crates.io/crates/arrow-udf-js/
- https://crates.io/crates/arrow-udf-wasm/

Python:

- https://pypi.org/project/arrow-udf/


Those packge will retain its name, while the repository will be moved to apache org.

## Required Resources

### Mailing Lists

We can reuse the existing mailing lists that arrow have.

### Git Repositories

#### Option 1

Maintian all arrow udf implemantion in the same repo.

From

- https://github.com/risingwavelabs/arrow-udf

To

- https://gitbox.apache.org/asf/repos/arrow-udf
- https://github.com/apache/arrow-udf

#### Option 2

Add Arrow UDF implementation to the corresponding
 language repository.
 
For example:

From

- https://github.com/risingwavelabs/arrow-udf/tree/main/arrow-udf

To

- https://github.com/apache/arrow-rs/path/to/udf

### Issue Tracking

The project would like to continue using GitHub Issues.

### Other Resources

The project has already chosen GitHub actions as continuous integration tools.

## Initial Committers

- Runji Wang wangrunji0408@163.com
- Giovanny Gutiérrez
- sundy-li sundyli@apache.org
- Xuanwo xuanwo@apache.org
- Max Justus Spransy maxjustus@gmail.com

[RisingWave]: https://github.com/risingwavelabs/risingwave
[Databend]: https://github.com/datafuselabs/databend