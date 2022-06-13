# NotesApp

Project Development


Our project consists on developing a Notes App through Java programming language. We have used the code in accordance with the topics discussed during lecture hours in Fundamentals of programming II. At first we have created three classes with the proper names : MainViewGUI which is the main class, Driver (which connects the code with DataBase) and AllNotesGUI. First, we create a Database with the name Notes, where we save all the information saved in this app. 
•	We start with the Driver class, which we use to connect the code with the database. We create a Query function which helps to add and get data in the database. We need three arguments for the database like url , user and password (all specified by string). We created some objects like Connection, Statement and Result to connect and query the database and get all the results from it. The results of the notes will be in a list.  When we execute the query we have two cases:”insert” where we add a data to the database and “select” where we get the data and then we save them. When we get the data we get the column “note” and we add them to the list we have declared above. In this class we have used the try-catch statement. If the DriverManager cannot connect to the database, method getConnection throws a SQLException. The catch statement will print this error. We close the objects (Connection, Statement, and Result) which we opened at the beginning, because Database requires it. Finally, the notes which we declared at the beginning of this class will be returned in a list with Strings.
•	 We continue with MainViewGUI class, which is the graphic that will appear when we run the code. We declare some objects for GUI specifications, for example: Text Area, Save Button, View All Button, and Frame. This class will implement interface ActionListener which determines where we clicked and generates the event to perform a specific task. By implementing we mean using the Override method in order to fully check later the code. After that we create 4 private variables named respectively JTextArea, Jbutton, Jbutton, and Jframe. We continue with the main method “public static void main (String [] rags” where the application gets executed. And, when it is executed it creates a new object, the MainGUI. To create the main object we have used different constructors. Initially, we have started with creating the frame by using the code “frame = new JFrame()”. After that, we have set some bounds for this frame like the position where it stands and also the width and the height. This can be changed as wanted by the code executer. By computing “ frame.setDefaultCloseOperation = (Jframe.EXIT_ON_CLOSE), means that when we press the button close, we exit from the frame too. We have written the codes for Jbutton “Save” and Jbutton “View All”. Besides that, we have also the JTextArea, where the code executes the command by allowing us to enter a certain Text in that area. In the end we have added “frame.setResizable(false) that makes impossible for the application to be resized. Otherwise, if it was true would make possible for the application to be resizable. 
After that, we continue with the Override() method where we have two cases. The first one is when we do not actually write any String in the text area and we want to save it. But actually, it appears a window where is written that we cannot save any null text. And the other case is when we write some Strings or characters, the note will be saved even in the database system. In the end, we use the try and catch method, in order for the system to catch any upcoming error during the execution of the application. 
Data Base has a problem where if you place double quotes, there are possibilities that database doesn’t recognize them which can be a problem to create data. Regex or regular expression is a sequence of characters that specifies a search pattern in text. Usually such patterns are used by string-searching algorithms for "find" or "find and replace" operations on strings, or for input validation. In our case we replaced the single quotes must be replaced with double quote in order for the information to be saved and to not deal with errors. If the case that we do not deal with error in the case of quotes the data will be added into database. 
Then we manipulate information by inserting into notes other values or called differently string contatinations. Then we call driver to execute the insertQuery query type. After this method will be executed it will do the connection… at the driver public class up to 3Execute SQL query. At this point if queryType is insert will execute update query and the note will be added.
Then NoteText.setText will empty the notes after previous notes are taken and saved.
And eventually message Note saved is returned. If we press viewall  command  we will create a new object which will have the same structure as the Driver driver = new Driver(); In this case we well create query where we will put the notes. Here is the execution of query to go next at Execute SQL query to get data which will be put in the Set (resultSet). 
We also use lambda expressions which is an object where object note will be added to all notes at the table. Than Frame initialization is done and is resize able, than Table initialization, Table parameters, JscrollPane in order to be scrollable.
