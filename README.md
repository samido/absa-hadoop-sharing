# absa
share resources with ABSA teams 
In order to use avron with log4j in kafka, please follow the following steps

STEP1:
     --> Set environment viriable "AVRO_SCHEMA" and map it to "avro.schema" file provided 
STEP2:
     --> All all the 3 jars provided to you class path where you system is running
STEP3: 
     --> in your log4j.property file, change your layout to AVRO
     --> i.e: log4j.appender.{rootLogger}.layout=co.za.absa.avron.logs.layout.AvroLogLayout
              log4j.appender.{rootLogger}.layout.Type=json
              log4j.appender.{rootLogger}.layout.MDCKeys=mdcKey
STEP4: 
      --> Test and observe the results, let me know if you have any problem
