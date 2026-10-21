# Converts HS-PGA numerical scores to character values.

Converts HS-PGA numerical scores to character values.

## Usage

``` r
hs_pga_char(hs_pga_scores)
```

## Arguments

- hs_pga_scores:

  Integer vector representing the HS-PGA scores (1: Clean, 2: Minimal,
  3: Mild, 4: Moderate, 5: Severe, 6: Very Severe).

## Value

A character vector representing the corresponding HS-PGA categories.

## References

Marzano, A V et al. “Creation of a severity index for hidradenitis
suppurativa that includes a validated quality-of-life measure: the
HIDRAscore.” Journal of the European Academy of Dermatology and
Venereology : JEADV vol. 34,8 (2020): 1815-1821. doi:10.1111/jdv.16328

## See also

Other HS-PGA:
[`hs_pga_num()`](https://humanpred.github.io/hidradenitis/reference/hs_pga_num.md)

## Examples

``` r
hs_pga_char(c(1, 2, 3, 4, 5, 6))
#> [1] "Clean"       "Minimal"     "Mild"        "Moderate"    "Severe"     
#> [6] "Very Severe"
```
