# hl7v2spark
Processing HL7v2 messages using spark pipelines following the Delta Lake architecture to create Patient insights.

This example uses the [Databricks Smolder](https://github.com/databrickslabs/smolder) library to parse HL7v2 messages (that are produced by the EHR/EMR systems in a clinical setting) and make it available as SQL datasource. The included Jar file (for Smolder) has been complied with Spark v3.1.0 and Scala v2.12.8. The Jar file can be added to the Spark cluster to leverage the Smolder capabilities. 

The example has been tested in Azure Synapse Analytics and uses ADLSGen2 storage as the source of HL7v2 messages.

