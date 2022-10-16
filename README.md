# hl7v2spark
Processing HL7v2 messages using spark pipelines following the Delta Lake architecture to create Patient insights.

This example uses the [Databricks Smolder](https://github.com/databrickslabs/smolder) library to parse [HL7v2 messages](https://www.hl7.org/implement/standards/product_brief.cfm?product_id=185) (that are produced by the EHR/EMR systems in a clinical setting) and make it available as SQL datasource. The included Jar file (for Smolder) has been complied with Spark v3.1.0 and Scala v2.12.8. The Jar file can be added to the Spark cluster to leverage the Smolder capabilities. 

The example has been tested in [Azure Synapse Analytics Notebook](https://learn.microsoft.com/en-us/azure/synapse-analytics/spark/apache-spark-notebook-concept) and uses [ADLS Gen2 storage](https://learn.microsoft.com/en-us/azure/storage/blobs/data-lake-storage-introduction) both as the source of HL7v2 messages as well as the persistence for Delta lake tables that are created in the example flow.

