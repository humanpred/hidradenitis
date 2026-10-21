# Calculates the HASI-R score for each patient and visit.

Calculates the HASI-R score for each patient and visit.

## Usage

``` r
hasi_r_num(
  bsa_percent_within_site = NULL,
  bsa_percent_total_body = NULL,
  bsa_ordinal = NULL,
  bodysite = NULL,
  inflam_color_chg,
  induration,
  open_skin_surface,
  tunnels
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

- inflam_color_chg:

  Integer vector representing inflammatory color change scores (0-3).

- induration:

  Integer vector representing induration scores (0-3).

- open_skin_surface:

  Integer vector representing open skin surface scores (0-3).

- tunnels:

  Integer vector representing tunnels scores (0-3).

## Value

A numeric vector of the calculated HASI-R score

## References

Goldfarb N, Lowes MA, Butt M, King T, Alavi A, Kirby JS. Hidradenitis
Suppurativa Area and Severity Index Revised (HASI-R): psychometric
property assessment. Br J Dermatol. 2021 May;184(5):905-912. doi:
10.1111/bjd.19565. Epub 2020 Dec 30. PMID: 32969027; PMCID: PMC8573730.

## See also

Other HASI:
[`hasi_bsa_to_ordinal()`](https://humanpred.github.io/hidradenitis/reference/hasi_bsa_to_ordinal.md)

## Examples

``` r
hasi_r_num(
  bsa_percent_within_site = c(0, 0, 0, 0, 5, 1, 4.3, 1.2, 6.8, 7.2),
  bodysite =
    c("Right Axilla", "Buttocks including Intergluteal Cleft",
      "Back", "Left Thigh", "Head & Neck", "Left Axilla",
      "Chest", "Pubis & Genitals", "Abdomen", "Right Thigh"),
  inflam_color_chg = c(0, 0, 0, 0, 2, 3, 1, 3, 2, 0),
  induration = c(0, 0, 0, 0, 2, 3, 1, 3, 2, 0),
  open_skin_surface = c(0, 0, 0, 0, 2, 3, 1, 3, 2, 0),
  tunnels = c(0, 0, 0, 0, 2, 3, 1, 3, 2, 0)
)
#> [1] 64
```
