Download Link: https://assignmentchef.com/product/solved-cosc2452-week8-independent-investigative-effort-8
<br>
<table width="745">

 <tbody>

  <tr>

   <td width="745">5. This week’s programming task will cover concepts required by Assignment 3. You should aim to get the help of your tutors and make further revisions.<strong>Coding exercise steps (Hint: Need help? Ask your tutor via Canvas→Discussions→”IIE08″):</strong>Complete the 18/Jan/2021 solution first as this extends upon that work. Next follow Canvas→<a href="https://rmit.instructure.com/courses/70691/modules">Modules→Week 8</a> where the topics of creating multiple classes is explained. <strong>Your tutors will provide further explanations on these general topics and how they relate to this IIE during their weekly “tutor chats”</strong>. Please also follow the announcement ‘<a href="https://rmit.instructure.com/courses/70691/discussion_topics/1039805">How to debug large programs and get help on </a><a href="https://rmit.instructure.com/courses/70691/discussion_topics/1039805">debugging…</a>’a) In this week’s IIE, modify <u>your own adaptation</u> of the IIE07 student manager (which has to be different to the student manager) so that it has the same functionality but across several class files as follows.Start by creating the Application.java (do not modify its contents or even rename the class to anything else) which is the new entry point to your program. When run, it will allow a graphical interface and a console interface to the same program and records that you add from one interface should be visible across all interfaces (via manually invoking a refresh method).<strong>Application.java</strong></td>

  </tr>

  <tr>

   <td width="745">public class Application {    private BackEnd backEnd;    private FrontEndGTerm uiGT;    private FrontEndConsole uiConsole;public Application() {       this.backEnd = new BackEnd();this.uiGT = new FrontEndGTerm(this.backEnd);       this.uiConsole = new FrontEndConsole(this.backEnd);    }public static void main(String[] args) {       Application app = new Application();}</td>

  </tr>

 </tbody>

</table>




<table width="745">

 <tbody>

  <tr>

   <td width="745">}</td>

  </tr>

  <tr>

   <td width="745"><strong>BackEnd.java: </strong>This file should contain the primary data structures (arrays relating to records), methods to add/remove records, etc. It should not have any mentions of GTerm, System.in/out, JOptionPane, etc. It must not make any assumptions about there being a GTerm interface and/or a console interface. All values returned by its methods should use standard Java API classes (e.g. String or Strings[]) or primitive data types. There is no need to prefix the method names with “backEnd” as done in IIE07.<strong>FrontEndGTerm.java: </strong>This file should contain only the methods and object member variables related to the GTerm interface. It must not have any awareness of any other interface. It should use tables, buttons, text fields, etc. to present the information. There is no need to prefix the method names with “gui” as done in IIE07.<strong>FrontEndConsole.java: </strong>This file should contain only the methods and object member variables related to the Console interface. It must not have any awareness of any other interface. A user should be able to perform the same operations (e.g. adding, querying, removing, etc.) as they can do with the graphical one above. There is no need to prefix the method names with “console” as done in IIE07.<strong>An important note about Assignment 2: </strong>In Assignment 2, there must be only one interface (GTerm). This IIE08 is relevant to Assingnment 3 requirements. </td>

  </tr>

 </tbody>

</table>