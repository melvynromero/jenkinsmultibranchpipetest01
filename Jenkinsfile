node {

    // properties([[$class: 'ParametersDefinitionProperty', parameterDefinitions: [[$class: 'StringParameterDefinition', defaultValue: '', description: 'Some Description', name : 'MY_PARAM'], [$class: 'StringParameterDefinition', defaultValue: '', description: 'Some Description', name: 'MY_PARAM2']]]])

    // hudson.model.StringParameterDefinition

    // properties([[$class: 'hudson.model.StringParameterDefinition', parameterDefinitions: [[$class: 'StringParameterDefinition', defaultValue: '', description: 'Some Description', name : 'MY_PARAM'], [$class: 'hudson.model.StringParameterDefinition', defaultValue: '', description: 'Some Description', name: 'MY_PARAM2']]]])

   // properties([[$class: 'hudson.model.ParametersDefinitionProperty', parameterDefinitions: [[$class: 'hudson.model.StringParameterDefinition', defaultValue: '', description: 'Some Description', name : 'MY_PARAM']]]])

 // properties([[$class: 'hudson.model.ParametersDefinitionProperty', parameterDefinitions: [[$class: 'hudson.model.ChoiceParameterDefinition', defaultValue: '', description: 'Param Choice Test', name : 'MY_PARAM_CHOICE']]]])

 // properties ([[$class: 'hudson.model.ParametersDefinitionProperty', parameterDefinitions: [[$class: 'hudson.model.ChoiceParameterDefinition', choices:  'Value1\nValue2' , description: '', name: 'unChoiceParameter']]]])

properties ([[$class: 'hudson.model.ParametersDefinitionProperty', parameterDefinitions: [[$class: 'hudson.model.ChoiceParameterDefinition', choices:  'Value1\nValue2' , description: '', name: 'unChoiceParameter'],
             [$class: 'hudson.model.ChoiceParameterDefinition', choices:  'Value1\nValue2' , description: '', name: 'otChoiceParameter']] ]])  


   stage 'Input and Parameters'

  // input message: 'Environment to Deploy', parameters: [[$class: 'hudson.model.ChoiceParameterDefinition', choices: 'local\nProduction', description: '', name: 'userinput01']]


def userInput = input(
 id: 'userInput', message: 'Let\'s promote?', parameters: [
 [$class: 'TextParameterDefinition', defaultValue: 'uat', description: 'Environment', name: 'env'],
 [$class: 'TextParameterDefinition', defaultValue: 'uat1', description: 'Target', name: 'target'],
 [$class: 'hudson.model.ChoiceParameterDefinition', choices: 'local\nProduction', description: '', name: 'userInput01']
]) 

/*
   def userInput =  input ( 
  id: 'userInput', message: 'Environment to Deploy', parameters: [
 // [$class: 'hudson.model.ChoiceParameterDefinition', choices: 'local\nProduction', description: '', name: 'userInput01']
  [$class: 'hudson.model.ChoiceParameterDefinition', choices: 'local\nProduction', description: '', name: 'userInput01']
])
*/
    echo "Choice ${unChoiceParameter}" 
    echo "Choice ${otChoiceParameter}" 
    echo ("Userinput01: "+userInput['userInput01'])

   
    stage 'Start Process ...'

    echo 'Hello from Multi Branch Pipeline with JenkinsFile'

    stage 'git my Proyect from GitHub .... '

    // git url: 'https://github.com/melvynromero/testjenkins01.git'

    stage 'Build and Show...'



   // build
    
    echo "Choice ${unChoiceParameter}" 
    echo "Choice ${otChoiceParameter}" 
    echo ("Userinput01: "+userInput['userInput01'])


   // echo "Choice ${userinput01}" 
  //  echo ("Print user input " + userInput['userInput01'])


}
