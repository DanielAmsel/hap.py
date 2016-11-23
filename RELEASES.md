# Hap.py Release Notes / Change Log   
   
## 0.2.12

HAP-214 fix Docker build error
HAP-238 fix escaping of spaces

## 0.2.11   
   
HAP-205 fix EVS feature support in som.py   
HAP-197 AF binning with arbitrary boundaries in som.py   
HAP-206  Fix header for BLT in hap.py output   
   
## 0.2.10   
   
HAP-184 check for empty query/ref vcf   
HAP-185 som.py --fix-chr-query does not fix MT appropriately   
HAP-187 som.py automatically resolve whether the --fix-chr-query switch is required   
HAP-192 Missing chromosomes cause fp.rate computation to fail in som.py   
HAP-201 hap.py integration tests failing because of trailing white space   
   
## v0.2.9   
   
HAP-149	Fix vcfeval integration via GA4GH interface   
HAP-154	ROC Support for Mutect2   
HAP-161	Output GT precision and FP counts for wrong GTs and wrong alleles separately   
HAP-166	Indel haplotype enumeration bug   
HAP-169	Change quantify/xcmp output be GA4GH compliant   
HAP-170	Som.py ROCs not correct in some cases   
HAP-171	ROC support using vcfeval   
HAP-176	One run for PASS and ALL to fix ROCs   
HAP-177	CNX doesn't extract caller name correctly for Mutect2   
HAP-179	Symmetric FP and FN for genotype mismatch   
HAP-183	Handling GATK gVCF \<NON\_REF\> alleles   
HAP-186	Update documentation and release notes   
   
   
## v0.2.8   
   
HAP-147 Normalisation problem where het-alts cancel each other out   
HAP-151 handle INDELs of undetermined length   
HAP-152 Implement Ti/Tv computation   
HAP-155 Improve support for GRC37 / non-chr-prefix references   
HAP-157 Calculate per-MB FP rate (as an "absolute" equivalent to precision)s   
HAP-162 Som.py outputs INF precision when FP and TP are 0   
HAP-163 Release notes and final test   
HAP-164 Sync up som.py empirical scoring features   
HAP-165 Speed improvements in quantify and upgrade to htslib 1.3   
   
## v0.2.7   
   
HAP-133 Parse platypus version strings correctly   
HAP-134 Calculate AFs from BAM for som.py feature table   
HAP-135 Som.py labels some variants twice in admixture comparisons   
HAP-136 Better Strelka feature extraction   
HAP-137 GT ordering makes unit test fail   
HAP-138 Add het/hom ratio to output table   
HAP-139 Document hap.py in Docker usage   
HAP-140 Misleading error messages when checkout headers in hap.py   
HAP-141 Remove / improve reference check error message   
HAP-142 Som.py -- stratify by AF brackets   
HAP-143 Empty VCF files cause failure   
HAP-144 Add filtered FN vs. absent FN to result table   
HAP-145 Hap.py -o switch doesn't accept prefix in current directory   
   
## v0.2.6   
   
HAP-83  premature exit when multimerging gvcfs   
HAP-123 Varscan2 DP rates are not calculated correctly   
HAP-124 Som.py --fix-chr-truth doesn't fix chr names in the ambi bed files   
HAP-126 Add VCF Validation Step   
HAP-127 Make -X the default behaviour (write extended metrics unless told otherwise)   
HAP-128 Hap.py ROCs for Freebayes and Platypus   
HAP-129 Som.py should support FP regions from Ambi file   
   
## v0.2.5   
   
HAP-119 ROCs should use TP variant types from query, not truth   
HAP-120 Write ROC data into JSON output   
HAP-122 Integrate VCFEval for matching   
HAP-121 Installer fails on some systems   
   
## v0.2.4   
   
HAP-103 Germline ROC curves   
HAP-115 --no-internal-* options are broken   
HAP-116 Quantify errors don't get printed   
HAP-117 Raw count quantify calls don't respect locations passed to hap.py   
   
## v0.2.3   
   
HAP-106 blocksplit / quantify segfault when reading faulty VCF   
HAP-107 Som.py tests fail in SD   
HAP-109 Hap.py fails for ambiguous bases in reference fasta   
HAP-111 Remove muscle dependency code and legacy stuff that depends on it   
HAP-112 Add option for hap.py to disable haplotype matching   
HAP-113 Check for output folder at start   
HAP-79  Well-formed vcf output file   
HAP-100 Clean up tests, fix platform-dependent sorting issues   
   
## v0.2.2   
   
HAP-23  Multi-sample variant graph implementation   
HAP-52  Create runner / wrapper script to run inside Docker   
HAP-78  Reference FASTA handling   
HAP-88  Refactor Cmake files to build included Boost, move build of dependencies to build folder   
HAP-90  Implement parallel graph enumeration   
HAP-92  Quantify should annotate the output VCF according to actual status   
HAP-94  Add allele counts by type (rather than per NT) back in   
HAP-95  Stratified feature output   
HAP-96  cnx aligners empty   
HAP-97  Hap.py does not quote or escape file path internally and fails on paths with spaces   
HAP-99  som.py should also be able to fix truth chr names   
HAP-102 Eliminate / clear up Locations.unknown   
HAP-104 Fix samtools build when using modules, add eb files   
   
## v0.2.1   
   
HAP-86  Not all vcfeval sites are matched   
HAP-87  auto chr naming detection broken   
HAP-89  Treatment of filtered variants should not be as optional   
HAP-93  GT mismatches are not counted as FP when no confident regions are specified.   
HAP-82  Print error (or at least warning) for bogus command-line arguments   
   
## v0.2.0   
   
HAP-39  Implement Allelic-primitive variant splitting   
HAP-72  QUAL misleading for type=missing records   
HAP-74  Remove setup.py   
HAP-75  Document the fact that bed files with tracks aren't supported.   
HAP-76  Add version information to output / simple output   
HAP-77  som.py should write puma metrics JSON file also   
HAP-80  Handle -P switch correctly for silver variants in PG 8.0   
HAP-81  Support VQSR ROCs in som.py   
HAP-84  no hap.py versions in output   
HAP-71  Hap.py fails on BED files with track information   
   
## v0.1.6   
   
HAP-8   Write user documentation   
HAP-54  Version number does not display   
HAP-59  Change som.py test to PG Admixture data   
HAP-62  hap.py non-verbose fail when FP regions file not found   
HAP-63  Add more comprehensive PG hap.py test (PGv7 vs. GATK 1.6 on chr21)   
   
## v0.1.5   
   
HAP-22  Split ref-match blocks into SNPs and indels   
HAP-44  Clean up + Migrate Dockerfile to Ubuntu 14.04   
HAP-46  Test + add GA4GH difficult indels to test set   
HAP-49  som.py should do ROC curves   
HAP-56  Define value in metrics.json   
HAP-57  -R option can make xcmp fail   
HAP-58  Add option for verbosity levels or to write message to log file   
HAP-54  Version number does not display   
HAP-62  hap.py non-verbose fail when FP regions file not found   
HAP-63  Add more comprehensive PG hap.py test (PGv7 vs. GATK 1.6 on chr21)   
   