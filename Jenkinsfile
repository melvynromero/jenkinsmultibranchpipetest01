node {

    // properties([[$class: 'ParametersDefinitionProperty', parameterDefinitions: [[$class: 'StringParameterDefinition', defaultValue: '', description: 'Some Description', name : 'MY_PARAM'], [$class: 'StringParameterDefinition', defaultValue: '', description: 'Some Description', name: 'MY_PARAM2']]]])

    // hudson.model.StringParameterDefinition

    properties([[$class: 'hudson.model.StringParameterDefinition', parameterDefinitions: [[$class: 'StringParameterDefinition', defaultValue: '', description: 'Some Description', name : 'MY_PARAM'], [$class: 'hudson.model.StringParameterDefinition', defaultValue: '', description: 'Some Description', name: 'MY_PARAM2']]]])


    stage 'Start Process ...'

    echo 'Hello from Multi Branch Pipeline with JenkinsFile'

    stage 'git my Proyect from GitHub .... '

    // git url: 'https://github.com/melvynromero/testjenkins01.git'

    stage 'Build ...'



    build
    
}
