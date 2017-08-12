### Helper tool for generating API documentation in markdown format from Servoy javascript source file

*Requires that Node.js is installed.* All other dependencies will be automatically installed/updated as needed.

To generate markdown API document just execute the batch file *generate-api-doc.bat* and at the prompt specify the source .js file to use.
*Note:* Ensure that the directory where the *generate-api-doc.bat* file resides is the active/current directory before executing the batch file.

The resulting output *result-api-doc.md* file will be generated in the *output* directory along with a copy of the source file but with cleaned-up JSDoc comments which can be parsed by jsdoc-parse without errors.

The batch file can be executed from the command prompt as well specifying the source .js file as argument using:

`
> cd "--path of directory of generate-api-doc.bat file--" 
> generate-api-doc.bat file "--full path to .js source file--"
`

After the result output file is generated it will be opened so you can copy its contents and update the GitHub wiki page as needed. If a default program is not set for markdown *.md* you will be prompted to select an application to open the *.md* file with.