# CRF
Conditional Random Field for Spark

This reporsitory is the continuous work of https://github.com/apache/spark/pull/9794/files
It supports Linear-CRF and will support graphics model.

Setup the development and test enviroment

1. Git clone the files and copy files to Spark directory.

2. Create application in Run/Debug configuration. Set program arguments: "template file path" "feature file path to train the model" "verification file path". For example "file:///home/usr/git/CRFConfig/temp-bag" "file:///home/usr/git/CRFConfig/us50train" "file:///home/usr/git/CRFConfig/us50test"; VM options: -Dspark.master=local; Working directory: Spark home; Enviroment variables: MASTER=local
or submit a job to Spark: ./spark-submit --class org.apache.spark.examples.ml.ConditionalRandomFieldExample /home/hujiayin/git/spark/examples/target/spark-examples_2.10-1.6.0-SNAPSHOT.jar "file:///home/hujiayin/git/CRFConfig/temp-bag" "file:///home/hujiayin/git/CRFConfig/us50train" "file:///home/hujiayin/git/CRFConfig/us50test"

3. Run examples to check results.

Contact: jiayin.hu@intel.com
