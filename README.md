# Python Technical Test

## Problem Statement
Create a python3 program that:

Download a file from a given URL:
1. small (10k lines)
2. medium (100k lines)
3. large (1M lines)
4. huge (10M lines)

Then, split the downloaded file content by date from `delivery_datetime` and `destination_country_code` into different files of 10k lines maximum each.

> source: small.csv
> 
> expected outputs:
> 
> 20210210_DE.csv
> 
> 20210210_FR.csv
> 
> 20210210_UK.csv
> 
> ...

- `product_id` value **MUST** be an integer.
- `product_id` value **MUST** be 10001 (consider only this `product_id`)
- `destination_country_code` **MUST** be a valid Country ISO Code.

## What we expect:

1. A readable Python script
2. No alteration of the downloaded file, as it could be provided by customers, you **MUST NOT** edit it.
3. A pure-python solution: no external database engine (MySQL, Cassandra, etc...), no shell command executed from the Python script...
4. A scalable solution: the script should work with small (10k lines), a medium (100k lines), a large file (1M lines), and a huge file (10M lines).
5. A text file (Markdown, reStructured, text, ...)  explaining how the code works and why you implemented it that way, keep it short if possible.

## Bonus:

1. Your code will be compatible with PEP8
2. Writing Unit Test