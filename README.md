Download Link: https://assignmentchef.com/product/solved-cpt120-tutorial-6
<br>
<ol start="3">

 <li>Follow the materials under Canvas→<a href="https://rmit.instructure.com/courses/56609/modules">Modules→Week 6</a><a href="https://rmit.instructure.com/courses/56609/modules">…</a></li>

</ol>

<table width="737">

 <tbody>

  <tr>

   <td width="737">5.1 (Hypothetical scenario) You turn up to your programming job one fine afternoon and find out that a programmer in your coding team has quit without giving any notice and all that the company has of the code that they were working on is the following “screenshot” (from which you would not normally be able to copy and paste):</td>

  </tr>

  <tr>

   <td width="737"><strong>import</strong> javax.swing.JOptionPane;<strong>public</strong> <strong>class</strong> RenovationProjectManager {    <strong>public</strong> <strong>static</strong> <strong>void</strong> main(String[] args) {<strong>double</strong> wallArea = 0, cost, height, length, costPerSqm;       <strong>int</strong> selection;String tempInput, wallNames;       String menu = “Menu:
”;menu += “1. Calculate paint required for a wall
”;       menu += “2. Calculate paint required for project”;       tempInput = JOptionPane.<em>showInputDialog</em>(menu);       <strong>while</strong> (tempInput != <strong>null</strong>) {selection = Integer.<em>parseInt</em>(tempInput);          <strong>if</strong> (selection == 1) {costPerSqm = Double.<em>parseDouble</em>(JOptionPane.<em>showInputDialog</em>(“Enter cost per sq.m ($)”));tempInput = JOptionPane.<em>showInputDialog</em>(“Enter a wall name”);height = Double.<em>parseDouble</em>(JOptionPane.<em>showInputDialog</em>(“Enter ” + tempInput + ” wall height (m)”));             length = Double.<em>parseDouble</em>(JOptionPane.<em>showInputDialog</em>(“Enter ” + tempInput + ” wall length (m)”));             wallArea = height * length;             cost = wallArea * costPerSqm;             JOptionPane.<em>showMessageDialog</em>(<strong>null</strong>,“Cost to paint ” + tempInput + ” wall of ” + wallArea + ” sq.m. is $” + cost);} <strong>else</strong> <strong>if</strong> (selection == 2) {costPerSqm = Double.<em>parseDouble</em>(JOptionPane.<em>showInputDialog</em>(“Enter cost per sq.m ($)”));             wallNames = “”;             wallArea = 0;             cost = 0;tempInput = JOptionPane.<em>showInputDialog</em>(“Enter a wall name (cancel to finish)”);             <strong>while</strong> (tempInput != <strong>null</strong>) {height = Double.<em>parseDouble</em>(JOptionPane.<em>showInputDialog</em>(“Enter ” + tempInput + ” wall height (m)”));                length = Double.<em>parseDouble</em>(JOptionPane.<em>showInputDialog</em>(“Enter ” + tempInput + ” wall length (m)”));wallArea += height * length;                wallNames += tempInput + “, “;tempInput = JOptionPane.<em>showInputDialog</em>(“Enter a wall name (cancel to finish)”);}             cost = wallArea * costPerSqm;             JOptionPane.<em>showMessageDialog</em>(<strong>null</strong>,                   “Cost to paint ” + wallNames + “wall(s) of ” + wallArea + ” sq.m. is $” + cost);          } <strong>else</strong> {JOptionPane.<em>showMessageDialog</em>(<strong>null</strong>, “Invalid choice!”);}tempInput = JOptionPane.<em>showInputDialog</em>(menu);}}}</td>

  </tr>

  <tr>

   <td width="737">Your first task is to run the code in Eclipse and add some high-level, plain-English comments, explaining what the different parts of the code are doing. <strong>Speak to your group tutors via forums/tutor chats for advice.</strong></td>

  </tr>

 </tbody>

</table>

Page 1 of 2

5.2. <strong>With the help of your group tutors via forums/tutor chats:</strong> Create a method for each of the (two) menu options and then move the code relevant to each menu option from the main method to the relevant methods that you created. In place of the original code that was moved, you must have a call to the method that would now do the work instead.

For this week, you must ensure that:

<ol>

 <li>Only method definitions are at the class level (e.g. do not create class/object member variables).</li>

 <li>Only the ‘main’ method definition has any mention of ‘static’. All method methods should be explicitly ‘public’ and not static.

  <ul>

   <li><strong>With the help of your group tutors via forums/tutor chats: </strong>Create a constructor method and then move all of the code in the ‘main’ method to the constructor method instead. Add comments to the code and explain what further changes you needed to make to the code in 5.2.</li>

   <li><strong>With the help of your group tutors via forums/tutor chats: </strong>Add a comment to your main method explaining what we should have in the main method and what we should not.</li>

   <li>Add comments in the style required by Assignment 2. See rubric in section 9 of the Assignment 2 PDF.</li>

  </ul></li>

</ol>


