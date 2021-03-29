# Extended structure factor file support for OneDep

onedep-extended-sf-support-examples
Examples of improved support for mmCIF/PDBx structure factor extensions

Extensions to the PDBx/mmCIF dictionary in reflection data with anisotropic diffraction limits, of unmerged reflection data, and of quality metrics for anomalous diffraction data are now supported in OneDep.

These extensions (over 50 dictionary items in total, complete with detailed descriptions) cover three main areas:
1.	scaled and merged reflection data that have been processed to take account of diffraction anisotropy, by providing descriptors for that anisotropy, in terms of (1) a parameter-free definition of a cut-off surface by means of a per-reflection “signal” and a threshold value for that signal, and (2) the ellipsoid providing the best fit to the resulting cut-off surface;
2.	scaled and unmerged reflection data, by providing extra item definitions aimed at ensuring that such data can be meaningfully re-analysed, and their quality assessed independently from the associated model, after retrieval from the archive;
3.	anomalous diffraction data, by adding descriptors for numerous relevant, but previously missing, statistics.
Although Global Phasing’s STARANISO program is the only one currently producing the new items describing anisotropic diffraction data, care has been taken in defining these items so that they be as generic as possible, so that developers of other software can make use of them or extend the present definitions to suit their applications.

Example files created by autoPROC and BUSTER that are compliant with the extended dictionary are contained in this repository.


