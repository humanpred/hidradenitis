# Calculates HiSCR scores given a percentage parameter.

Calculates HiSCR scores given a percentage parameter.

## Usage

``` r
hiscr(
  baseline_abscess,
  baseline_nodule,
  baseline_fistula,
  timepoint_abscess,
  timepoint_nodule,
  timepoint_fistula,
  percentage
)
```

## Arguments

- baseline_abscess:

  Integer vector representing the abscess count at baseline.

- baseline_nodule:

  Integer vector representing the inflammatory nodule count at baseline.

- baseline_fistula:

  Integer vector representing the draining fistula count at baseline.

- timepoint_abscess:

  Integer vector representing the abscess count at the time point of
  interest.

- timepoint_nodule:

  Integer vector representing the inflammatory nodule count at the time
  point of interest.

- timepoint_fistula:

  Integer vector representing the draining fistula count at the time
  point of interest.

- percentage:

  Numeric value specifying the percentage required for HiSCR (e.g., 50
  for HiSCR50, 75 for HiSCR75, etc.).

## Value

A logical vector indicating whether the HiSCR response is achieved for
each set of input parameters.

## References

Kimball, A B et al. “HiSCR (Hidradenitis Suppurativa Clinical Response):
a novel clinical endpoint to evaluate therapeutic outcomes in patients
with hidradenitis suppurativa from the placebo-controlled portion of a
phase 2 adalimumab study.” Journal of the European Academy of
Dermatology and Venereology : JEADV vol. 30,6 (2016): 989-94.
doi:10.1111/jdv.13216

## Examples

``` r
hiscr(
  baseline_abscess = c(3, 2, 4),
  baseline_nodule = c(5, 4, 6),
  baseline_fistula = c(2, 1, 3),
  timepoint_abscess = c(1, 1, 2),
  timepoint_nodule = c(2, 3, 2),
  timepoint_fistula = c(2, 1, 3),
  percentage = 50
)
#> [1]  TRUE FALSE  TRUE
```
