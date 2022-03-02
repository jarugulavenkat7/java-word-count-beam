# java-word-count-beam
## Venkat Sai Jarugula
### Instructions
* Link to java quick start : [https://beam.apache.org/get-started/quickstart-java/](https://beam.apache.org/get-started/quickstart-java/)
* Start in your 44-517 folder. Right-click and open PS here as Admin. Use Maven archetype to fetch a project. <br>
 ```PS> mvn archetype:generate `
 -D archetypeGroupId=org.apache.beam `
 -D archetypeArtifactId=beam-sdks-java-maven-archetypes-examples `
 -D archetypeVersion=2.36.0 `
 -D groupId=org.example `
 -D artifactId=word-count-beam `
 -D version="0.1" `
 -D package=org.apache.beam.examples `
 -D interactiveMode=false ```
* Add the sample.txt file in the root. And copy the content from [Shakespeare's sonnets](https://00f74ba44b53e1a885e6b75f49feb942e14f609ae9-apidata.googleusercontent.com/download/storage/v1/b/apache-beam-samples/o/shakespeare%2Fsonnets.txt?jk=AFshE3VOFxl839jmhermqav03NJ7mSGNj0Z5FgfSCBLfbAgcMkviTqN7Mefwki7rlOrMu3bJFGZzaxcXYEqiVjJxiX3HXaxkbMuU0v4qTM-7XoMz9iWardkzMjU0Oed7owpE3qJsVa_h1zPQREJ1IQgEnu5B1njvQ7Q3zjiqUESaMeIdoHnbYn_V8RtIT6AXHYZJHJF6BR-qAdETndlCuDCai_HY-84FfYKkQqlNeNh3DLO-R4lYNEKEJucPA-GbEMPHysY4Qa4r94QaVesphvturO3gDckXPjlOY_mc-oPczq8o7nrwQBiWv9yE-TPxPbl5w607cHplxdicP81aFqA_O4RQGunYNih2pZNxJ4VDUoqIe4Ojk2cN5C0ziz4Xqf40pLhTH9_CvnKWrJTfIf96Z94ZtnuLX1vF21Har9_HYVnIiZJu8jL1usnTmMfWgpPhITISVUnStr5T8hgBy5gCh9bIq-mq_n2kvMAD_ZvxCjrXiU2zIFmbGf7XHkzSdVe4jC5NDvPGuAxpH0YlTA8UPHE3qD_7Msr-sx9JBOghGhwy4ySsfXgaDZx7oBLCSWLZCkQ39HYkWhAiic87UnQ_AfqUEKBNMg23Ex4PRVUo5YG_JskxG-yuQQ4vsgMZjL63ruKroCQIsZ9Me1ZtdEnVJkvvQpe3DU20MBi4UdaC_zqLbpV06t79POx36bp8hpJW98KEt2H4slIyE3d6c5cTrqJ2vNFgAHiQHXt-FOREAftCQ8JLsh1BwoataISO1pkNE422zZgElV8UFLO3N_mfI73kt32zSErRHrChObFVOVky50zCQ077_z34yIYDkkQ5BVWXjLNZk-wpgh8mdLkjnO7ywswRlIWRHN17kRPBqPOe797nUwfGShpKuDF620TgnGmyWhGUWYi5oJSgi9Bl3Nay24xj2tKMwbzqu_q3g6JGlmd-j5qE3xZte5v3o_qdpMJKfRU5Kgo5TLHwKbRVJI_EWw0&isca=1) <br>
 
* Run WordCount Using Maven
   ```
   PS> mvn compile exec:java -D exec.mainClass=org.apache.beam.examples.WordCount `
  -D exec.args="--inputFile=sample.txt --output=counts" -P direct-runner
   ```
