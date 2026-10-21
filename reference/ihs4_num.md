# Calculates IHS4 scores based on abscess, draining fistula, and inflammatory nodule counts.

Calculates IHS4 scores based on abscess, draining fistula, and
inflammatory nodule counts.

## Usage

``` r
ihs4_num(nodules, abscesses, draining_tunnels)
```

## Arguments

- nodules:

  Integer vector representing the nodule count

- abscesses:

  Integer vector representing the abscess count

- draining_tunnels:

  Integer vector representing the draining tunnel count

## Value

An integer vector representing the IHS4 scores (0-3: Mild, 4-10:
Moderate, 11- : Severe).

## References

Zouboulis, C C et al. “Development and validation of the International
Hidradenitis Suppurativa Severity Score System (IHS4), a novel dynamic
scoring system to assess HS severity.” The British journal of
dermatology vol. 177,5 (2017): 1401-1409. doi:10.1111/bjd.15748

## See also

Other IHS4:
[`ihs4_char()`](https://humanpred.github.io/hidradenitis/reference/ihs4_char.md)

## Examples

``` r
ihs4_num(
  nodules = c(5, 3, 2),
  abscesses = c(2, 1, 0),
  draining_tunnels = c(1, 2, 3)
)
#> [1] 13 13 14
```
