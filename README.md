# word-count-beam



## Command To create template
`
mvn compile exec:java \
     -Dexec.mainClass=org.apache.beam.examples.WordCount \
     -Dexec.args="--runner=DataflowRunner \
                  --project=gcp-learning-342413 \
                  --stagingLocation=gs://gcp-learning-342413.appspot.com/staging \
                  --templateLocation=gs://gcp-learning-342413.appspot.com/templates/WordCount \
                  --region=asia-south1" \
     -P dataflow-runner
`
