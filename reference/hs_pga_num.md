# Calculates HS-PGA scores based on abscess, draining fistula, and inflammatory nodule counts.

Calculates HS-PGA scores based on abscess, draining fistula, and
inflammatory nodule counts.

## Usage

``` r
hs_pga_num(abscess_fistula, inflammatory_nodule, non_inflammatory_nodule)
```

## Arguments

- abscess_fistula:

  Integer vector representing the sum of abscess and draining fistula
  counts.

- inflammatory_nodule:

  Integer vector representing the inflammatory nodule count.

- non_inflammatory_nodule:

  Integer vector representing the non-inflammatory nodule count.

## Value

An integer vector representing the HS-PGA scores (1: Clean, 2: Minimal,
3: Mild, 4: Moderate, 5: Severe, 6: Very Severe)

## References

Marzano, A V et al. “Creation of a severity index for hidradenitis
suppurativa that includes a validated quality-of-life measure: the
HIDRAscore.” Journal of the European Academy of Dermatology and
Venereology : JEADV vol. 34,8 (2020): 1815-1821. doi:10.1111/jdv.16328

## See also

Other HS-PGA:
[`hs_pga_char()`](https://humanpred.github.io/hidradenitis/reference/hs_pga_char.md)

## Examples

``` r
hs_pga_num(
  abscess_fistula = c(0, 0, 1, 0, 1, 2, 6),
  inflammatory_nodule = c(0, 0, 0, 3, 5, 8, 12),
  non_inflammatory_nodule = c(0, 1, 0, 0, 0, 0, 0)
)
#> [1] 1 2 3 3 4 4 6
```
