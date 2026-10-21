# Converts IHS4 numerical scores to character values.

Converts IHS4 numerical scores to character values.

## Usage

``` r
ihs4_char(ihs4_scores)
```

## Arguments

- ihs4_scores:

  Integer vector representing the IHS4 scores (0-3: Mild, 4-10:
  Moderate, \>=11: Severe).

## Value

A character vector representing the corresponding IHS4 categories

## References

Zouboulis, C C et al. “Development and validation of the International
Hidradenitis Suppurativa Severity Score System (IHS4), a novel dynamic
scoring system to assess HS severity.” The British journal of
dermatology vol. 177,5 (2017): 1401-1409. doi:10.1111/bjd.15748

## See also

Other IHS4:
[`ihs4_num()`](https://humanpred.github.io/hidradenitis/reference/ihs4_num.md)

## Examples

``` r
ihs4_char(c(2, 5, 12))
#> [1] "Mild"     "Moderate" "Severe"  
```
