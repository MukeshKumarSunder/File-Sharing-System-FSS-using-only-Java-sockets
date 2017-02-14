# File-Sharing-System-FSS-using-only-Java-sockets
To run the project from the command line, go to the dist folder and
type the following:

java -jar "ProgrammingAssignment1.jar" <role> <operation> <args[]>

# To set up client so it knows what server to talk to:
export PA1_SERVER=<computername:portnumber> # On Windows: set PA1_SERVER=.....


Possible syntaxes:

	->java -jar "ProgrammingAssignment1.jar" server start <portnumber>

	->java -jar "ProgrammingAssignment1.jar" client upload <path_on_client> </path/filename/on/server>

	->java -jar "ProgrammingAssignment1.jar" client download </path/existing_filename/on/server> <path_on_client>
	
	->java -jar "ProgrammingAssignment1.jar" client dir </path/existing_directory/on/server>
	
	->java -jar "ProgrammingAssignment1.jar" client mkdir </path/new_directory/on/server>

	->java -jar "ProgrammingAssignment1.jar" client rmdir </path/existing_directory/on/server>

	->java -jar "ProgrammingAssignment1.jar" client rm </path/existing_filename/on/server> 

	->java -jar "ProgrammingAssignment1.jar" client shutdown


F:\Mukesh\George Mason University\Subjects\SWE 622\assignment

pushd F:\Mukesh\George Mason University\Subjects\SWE 622\assignment

java -jar "ProgrammingAssignment1.jar" server start 8052

set PA1_SERVER=127.0.0.1:8052

java -jar "Mukesh.jar" client upload README.TXT abcd.TXT

java -jar "Mukesh.jar" client download README.TXT abcd.TXT

java -jar "Mukesh.jar" client dir "F:\Mukesh\George Mason University\Subjects\SWE 622\assignment"

java -jar "Mukesh.jar" client mkdir "F:\Mukesh\George Mason University\Subjects\SWE 622\assignment\test1"

java -jar "Mukesh.jar" client rmdir "F:\Mukesh\George Mason University\Subjects\SWE 622\assignment\test1"

java -jar "Mukesh.jar" client rm "F:\Mukesh\George Mason University\Subjects\SWE 622\assignment\dummy.txt"

java -jar "Mukesh.jar" client shutdown
