# Converts BSA percentage to the ordinal scale for HASI-R scoring.

Converts BSA percentage to the ordinal scale for HASI-R scoring.

## Usage

``` r
hasi_bsa_to_ordinal(
  bsa_percent_within_site = NULL,
  bsa_percent_total_body = NULL,
  bsa_ordinal = NULL,
  bodysite = NULL
)
```

## Arguments

- bsa_percent_within_site:

  Numeric vector representing BSA percentages (0-100)

- bsa_percent_total_body:

  Numeric vector representing BSA percentages (0-15, depending on site)

- bsa_ordinal:

  Numeric vector representing BSA values. (0-6)

- bodysite:

  Optional character vector representing body sites

## Value

Integer vector representing the ordinal scale values

## References

Goldfarb N, Lowes MA, Butt M, King T, Alavi A, Kirby JS. Hidradenitis
Suppurativa Area and Severity Index Revised (HASI-R): psychometric
property assessment. Br J Dermatol. 2021 May;184(5):905-912. doi:
10.1111/bjd.19565. Epub 2020 Dec 30. PMID: 32969027; PMCID: PMC8573730.

## See also

Other HASI:
[`hasi_r_num()`](https://humanpred.github.io/hidradenitis/reference/hasi_r_num.md)

## Examples

``` r
hasi_bsa_to_ordinal(c(0, 2, 5, 12, 25, 40, 75))
#> [1] 0 1 2 3 4 5 6
```
