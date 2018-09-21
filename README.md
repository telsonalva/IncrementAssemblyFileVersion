How To

1) Take the 'IncrementFileVersion.exe' file from /package/ and copy it your solution directory
2) Right click on your project -> Properties
3) Click on 'Build Events'
4) In the prebuild even command line, paste the following
	$(SolutionDir)\IncrementFileVersion.exe "$(SolutionDir)\$(ProjectName)\Properties\AssemblyInfo.cs"

Build the project and check if AssemblyFileVersion actually increments
*Cross check the location of the AssemblyInfo.cs file in step 4.