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

    out/en/gold/train.drs.clf
    out/en/gold/train.parse.tags
    out/en/gold/dev.drs.clf
    out/en/gold/dev.parse.tags
    out/en/gold/test.drs.clf
    out/en/gold/test.parse.tags
    out/en/gold/eval.drs.clf
    out/en/gold/eval.parse.tags
    out/de/gold/train.drs.clf
    out/de/gold/train.parse.tags
    out/de/gold/dev.drs.clf
    out/de/gold/dev.parse.tags
    out/de/gold/test.drs.clf
    out/de/gold/test.parse.tags
    out/it/gold/train.drs.clf
    out/it/gold/train.parse.tags
    out/it/gold/dev.drs.clf
    out/it/gold/dev.parse.tags
    out/it/gold/test.drs.clf
    out/it/gold/test.parse.tags
    out/nl/gold/train.drs.clf
    out/nl/gold/train.parse.tags
    out/nl/gold/dev.drs.clf
    out/nl/gold/dev.parse.tags
    out/nl/gold/test.drs.clf
    out/nl/gold/test.parse.tags
    out/en/bronze/train.drs.clf
    out/en/bronze/train.parse.tags
    out/en/silver/train.drs.clf
    out/en/silver/train.parse.tags
    out/de/bronze/train.drs.clf
    out/de/bronze/train.parse.tags
    out/de/silver/train.drs.clf
    out/de/silver/train.parse.tags
    out/it/bronze/train.drs.clf
    out/it/bronze/train.parse.tags
    out/it/silver/train.drs.clf
    out/it/silver/train.parse.tags
    out/nl/bronze/train.drs.clf
    out/nl/bronze/train.parse.tags
    out/nl/silver/train.drs.clf
    out/nl/silver/train.parse.tags
