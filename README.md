flatpmb
=======

This repo converts the released version of the
[Parallel Meaning Bank](https://pmb.let.rug.nl) 4.0.0, which has a complex
directory hierarchy, to a small number of flat files, each containing multiple
documents. Specifically, you get one file per:

* **language**: English, German, Italian, or Dutch
* **status**: gold, silver, or bronze
* **portion**: train, dev (gold only), test (gold only), or eval (English gold
  only)
* **file type**: `drs.clf` or `parse.tags`. More file types may be supported in
  the future.

Usage
-----

Download PMB 4.0.0 and place the release in `data/pmb-4.0.0`.

Install [Produce](https://github.com/texttheater/produce) v0.6.0. Make sure the
`produce` executable ends up on your `PATH`.

To run the conversion, simply execute from this directory:

    produce

This will generate the following output files:

    out/pmb-4.0.0/en/gold/train.drs.clf
    out/pmb-4.0.0/en/gold/train.parse.tags
    out/pmb-4.0.0/en/gold/dev.drs.clf
    out/pmb-4.0.0/en/gold/dev.parse.tags
    out/pmb-4.0.0/en/gold/test.drs.clf
    out/pmb-4.0.0/en/gold/test.parse.tags
    out/pmb-4.0.0/en/gold/eval.drs.clf
    out/pmb-4.0.0/en/gold/eval.parse.tags
    out/pmb-4.0.0/de/gold/train.drs.clf
    out/pmb-4.0.0/de/gold/train.parse.tags
    out/pmb-4.0.0/de/gold/dev.drs.clf
    out/pmb-4.0.0/de/gold/dev.parse.tags
    out/pmb-4.0.0/de/gold/test.drs.clf
    out/pmb-4.0.0/de/gold/test.parse.tags
    out/pmb-4.0.0/it/gold/train.drs.clf
    out/pmb-4.0.0/it/gold/train.parse.tags
    out/pmb-4.0.0/it/gold/dev.drs.clf
    out/pmb-4.0.0/it/gold/dev.parse.tags
    out/pmb-4.0.0/it/gold/test.drs.clf
    out/pmb-4.0.0/it/gold/test.parse.tags
    out/pmb-4.0.0/nl/gold/train.drs.clf
    out/pmb-4.0.0/nl/gold/train.parse.tags
    out/pmb-4.0.0/nl/gold/dev.drs.clf
    out/pmb-4.0.0/nl/gold/dev.parse.tags
    out/pmb-4.0.0/nl/gold/test.drs.clf
    out/pmb-4.0.0/nl/gold/test.parse.tags
    out/pmb-4.0.0/en/bronze/train.drs.clf
    out/pmb-4.0.0/en/bronze/train.parse.tags
    out/pmb-4.0.0/en/silver/train.drs.clf
    out/pmb-4.0.0/en/silver/train.parse.tags
    out/pmb-4.0.0/de/bronze/train.drs.clf
    out/pmb-4.0.0/de/bronze/train.parse.tags
    out/pmb-4.0.0/de/silver/train.drs.clf
    out/pmb-4.0.0/de/silver/train.parse.tags
    out/pmb-4.0.0/it/bronze/train.drs.clf
    out/pmb-4.0.0/it/bronze/train.parse.tags
    out/pmb-4.0.0/it/silver/train.drs.clf
    out/pmb-4.0.0/it/silver/train.parse.tags
    out/pmb-4.0.0/nl/bronze/train.drs.clf
    out/pmb-4.0.0/nl/bronze/train.parse.tags
    out/pmb-4.0.0/nl/silver/train.drs.clf
    out/pmb-4.0.0/nl/silver/train.parse.tags
