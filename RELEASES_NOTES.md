# v1.2.0  [dev]
### Update notes:
This section contain actions to execute if you update a previous FROGS version to this version.

  * The repository structure has been changed: tools have been moved in sub-directories. It is necessary to re-do the following installation steps: '6. Add tools in galaxy' and '7. Set memory and parallelisation settings'.
  * The tool FROGS\_tsv\_to\_biom has been added. It is necessary to add the following line in galaxy tool_conf.xml: `<tool file="FROGS/tools/tsv_to_biom/tsv_to_biom.xml" />`.

### Bugs fixes:
  * Too large number of temp files in clustering tool.
  * Fix bug with BIOM without observation metadata in filters.
  * Fix bug with heatmap hover in affiliations_stat.

### Functions added:
  * Add tool to convert a TSV file in BIOM file.
  * Default BIOM becomes mono-line.
  * Reduce the BIOM file size (identation 4 -> 2 in pretty_print).
  * Change the repository structure (one directory by tool).
  * Use biomTools in normalisation.
  * Number of sampled sequences becomes required in normalisation tool.
  * Add better wrapping for sample name fields in preprocess.
  * Add check on minimum amplicon size value in preprocess.
  * Add vsearch version in remove chimera log.
  * Add cutadapt version in preprocess log.


# v1.1.0  [2015-11-30]
### Bugs fixes:
  * Fix bug with empty blast_taxonomy in BIOM.
  * Fix bug with checkall in chrome.
  * Fix bug with CSV extraction in HTML outputs.
  * Fix bug 'Exception in thread QueueFeederThread' in slow systems.

### Functions added:
  * Add '% kept' in preprocess.
  * Add checks on samples names in preprocess.
  * Add DenseData management in BIOM.
  * Add the biom1 datatype in tools.


# v1.0.0  [2015-09-18]
  First package.