@Library('piper-library-os') _


stage('RunUnitTest') 
    gctsExecuteABAPUnitTests(
      script: this,
      host: 'https://hcluks4hana.hcldigilabs.com:8001',
      client: '200',
      abapCredentialsId: 'AbapSystem',
      repository: 'OpenSAP'
)

stage('RollbackCommit') 
    gctsRollback(
      script: this,
      host: "https://hcluks4hana.hcldigilabs.com:8001/",
      client: "200",
      abapCredentialsId: 'AbapSystem',
      repository: "OpenSAP"
  )


