## recount2 datasets for cola analysis

In this collection, *cola* analysis was applied to 223 recount2 datasets. Click following link to see how the data was processed and analyzed.

<details><summary>Data processing and analysis</summary>
<p></p>
 <p>Recount datasets were downloaded from <a href="https://jhubiostatistics.shinyapps.io/recount/" rel="nofollow">recount2 website</a> on 2018-11-13 (see the sample list <a href="https://github.com/jokergoo/cola_manuscript/blob/master/download/recount_selection_2018-11-13_14_42_40.csv">here</a>). Datasets with more than 500 samples or less than 50 samples were removed. Also GTEx and TCGA datasets separated by tissues were downloaded. Row counts were normamlized by TPM method. Only the protein coding genes (defined by Gencode v25) were used. Genes that have less than 2 reads in more than 50% samples were removed. <code>log2(tpm + 1)</code> were used for cola analysis.</p>
<ul>
<li><a href="https://github.com/jokergoo/cola_manuscript/tree/master/download">script for downloading and preprocessing</a></li>
<li><a href="https://github.com/jokergoo/cola_manuscript/tree/master/test_cohort">script for cola analysis</a></li>
</ul>
<p>The analysis were done with <a href='https://github.com/jokergoo/cola/releases/tag/1.3.2'>cola 1.3.2</a>. Users need to use R with version &gt;= 3.6.0 to read the <code>*.rds</code> files provided in the following table.</p>
<p></p>

</details>

<p></p>



|ID                                                                                |Title                                                                                                                                                                                                                                                  |Samples |Features |File                                                                                                          |
|:---------------------------------------------------------------------------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:-------|:--------|:-------------------------------------------------------------------------------------------------------------|
|<a href='http://trace.ncbi.nlm.nih.gov/Traces/sra/?study=DRP000987'>DRP000987</a> |<a href='https://cola-recount2.github.io/DRP000987/cola_report.html'>Interactive Transcriptome Analysis of Malaria Patients and Infecting Plasmodium falciparum in Indonesia</a>                                                                       |121     |58037    |<a href='https://cola-recount2.github.io/DRP000987/DRP000987_cola_all.rds'>rds_file</a>                       |
