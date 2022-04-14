# COM210ProgrammingAssignment
package programassignment;

import java.io.*;

import java.util.*;

import java.util.Stack;



class ProgramAssignment
{
     
    public static void main (String[] args)
	{
   String[] word = {"{","a", "b", "}"};       
 Stack < String > stack = new Stack < String > ();
 
 for (int i = 0; i<=word.length; i++)
 
 {
  
  if(word[i].equals("{")) 
  {   
  
 stack.push("{");
 
System.out.println("Open Delimiter in Stack: " + stack);

  }
  
 
 
  for (int j = 0; j<=word.length; j++)
  {
  
  if (word[j].equals("}"))
  
  {
  
  System.out.println("Closing Delimiter Found: " + stack.pop() + "}");

  }  
  else if(!word.equals("}")) 
  {
  
  System.out.println("Closing Delimiter Missing Here at word[" + j + "]" );
  
  
  }   
  
  } //for statement for closing delimiter   
   
     
 }//closing for statement open delimiter		
	
 }
	
}

